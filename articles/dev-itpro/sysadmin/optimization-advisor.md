---
title: "Optimizavimo patariamojo įrankio taisyklių kūrimas"
description: "Šioje temoje aptariama, kaip į optimizavimo patariamąjį įrankį įtraukti naujų taisyklių."
author: roxanadiaconu
manager: AnnBe
ms.date: 01/23/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: SelfHealingWorkspace
audience: Application User, IT Pro
ms.reviewer: yuyus
ms.search.scope: Core (Operations, Core)
ms.custom: 
ms.assetid: 
ms.search.region: global
ms.search.industry: 
ms.author: roxanad
ms.search.validFrom: 2017-12-01
ms.dyn365.ops.version: 7.3
ms.translationtype: HT
ms.sourcegitcommit: 9cb9343028acacc387370e1cdd2202b84919185e
ms.openlocfilehash: 88739298405343a36ae5bc11f51c666c414e7157
ms.contentlocale: lt-lt
ms.lasthandoff: 01/23/2018

---

# <a name="create-rules-for-optimization-advisor"></a>Optimizavimo patariamojo įrankio taisyklių kūrimas

[!include[banner](../includes/banner.md)]

Šioje temoje paaiškinama, kaip sukurti naujų **optimizavimo patariamojo įrankio** taisyklių. Pavyzdžiui, galite sukurti naują taisyklę, nustatančią, kurių pasiūlymų patvirtinimų (RFQ) atvejų pavadinimai yra tušti. Naudojant atvejų pavadinimus, juos lengva nustatyti ir jų ieškoti. Nors šis pavyzdys gana paprastas, juo parodoma, ko galima pasiekti optimizavimo taisyklėmis. 

*Taisyklė* yra programos duomenų patikra. Jei išpildoma sąlyga, kurią vertina taisyklė, sukuriama galimybių optimizuoti procesus ar patobulinti duomenis. Dėl galimybių galima imtis veiksmų ir (pasirenkama) galima matuoti veiksmų poveikį. 

Norėdami sukurti naują **optimizavimo patariamojo įrankio** taisyklę, įtraukite naują klasę, išplečiančią abstrakčią klasę **SelfHealingRule**, įdiegiančią **IDiagnosticsRule** sąsają ir kurią įformina atributas **DiagnosticRule**. Klasėje taip pat turi būti metodas, kurį įformina atributas **DiagnosticsRuleSubscription**. Paprastai tai daroma naudojant metodą **opportunityTitle**, kuris bus aptartas vėliau. Šią naująją klasę galima įtraukti į pasirinktinį modelį su priklausomybe modelyje **SelfHealingRules**. Tolesniame pavyzdyje įdiegiama taisyklė vadinama **RFQTitleSelfHealingRule**.

```
[DiagnosticsRule] 
public final class RFQTitleSelfHealingRule extends SelfHealingRule implements IDiagnosticsRule 
{ 
… 
} 
```

Abstrakčioje klasėje **SelfHealingRule** yra abstrakčių metodų, kuriuos reikia įdiegti paveldinčiose klasėse. Pagrindas yra metodas **įvertinti**, kuris pateikia taisyklės nustatytų galimybių sąrašą. Galimybės gali būti taikomos vienam juridiniam subjektui arba visai sistemai.

```
protected List evaluate() 
{ 
    List results = new List(Types::Record); 
    
    DataArea dataArea; 

    while select id from dataArea 
        where !dataArea.isVirtual 
    { 
        changecompany(dataArea.id) 
        { 
            container result = this.findRFQCasesWithEmptyTitle(); 

            if (conLen(result) > 0) 
            { 
                SelfHealingOpportunity opportunity = this.getOpportunityForCompany(dataArea.Id); 
                opportunity.EvaluationState = SelfHealingEvaluationState::Evaluated; 
                opportunity.Data = result; 
                opportunity.OpportunityDate = DateTimeUtil::utcNow(); 
                
                results.addEnd(opportunity); 
            } 
        } 
    } 
    
    return results; 
} 
```

Aukščiau parodytas metodas analizuoja įmones ir pasirenka RFQ atvejus su tuščiais pavadinimais metode **findRFQCasesWithEmptyTitle**. Jei randamas bent vienas toks atvejis, naudojant metodą **getOpportunityForCompany** sukuriama konkrečios įmonės galimybė. Atkreipkite dėmesį, kad lentelės **SelfHealingOpportunity** lauko **Duomenys** tipas yra **Konteineris**, todėl jame gali būti duomenų, susijusių su šiai taisyklei būdinga logika. Elemente **OpportunityDate** nustačius dabartinę laiko žymą, užregistruojamas vėliausio galimybės įvertinimo laikas.  

Galimybės taip pat gali būti taikomos visoje įmonėje. Tokiu atveju įmonių analizė nebūtina ir galimybę reikia kurti naudojant metodą **getOpportunityAcrossCompanies**. 

Tolesniame kode rodomas metodas **findRFQCasesWithEmptyTitle**, pateikiantis RFQ atvejų tuščiais pavadinimais ID.

```
private container findRFQCasesWithEmptyTitle() 
{ 
    container result; 

    PurchRFQCaseTable rfqCase; 
    while select RFQCaseId from rfqCase 
        where rfqCase.Name == '' 
    { 
        result += rfqCase.RFQCaseId; 
    } 
    
    return result; 
} 
```

Dar du įdiegtini metodai yra **opportunityTitle** ir **opportunityDetails**. Pirmasis pateikia trumpą galimybės pavadinimą, pastarasis pateikia išsamų galimybės aprašą, kuriame taip pat gali būti duomenų.

Pavadinimas, kurį pateikia **opportunityTitle**, rodomas darbo srities **Optimizavimo patariamasis įrankis** stulpelyje **Optimizavimo galimybė**. Jis taip pat rodomas kaip šoninės srities, kurioje apie galimybę rodoma daugiau informacijos, antraštė. Paprastai šį metodą įformina atributas **DiagnosticRuleSubscription**, su kuriuo galima naudoti tolesnius argumentus. 

* **Diagnostikos sritis** – tipo **DiagnosticArea** išvardijimas, apibrėžiantis, kuriai programos sričiai priklauso taisyklė, pvz., **DiagnosticArea::SCM**. 

* **Taisyklės pavadinimas** – eilutė su taisyklės pavadinimu. Ji bus rodoma formos **Diagnostikos tikrinimo taisyklė** stulpelyje **Taisyklės pavadinimas** (**DiagnosticsValidationRuleMaintain**). 

* **Vykdymo dažnis** – tipo **DiagnosticRunFrequency** išvardijimas, aprašantis, kaip dažnai taisyklę reikėtų vykdyti, pvz., **DiagnosticRunFrequency::Daily**. 

* **Taisyklės aprašas** – eilutė su išsamesniu taisyklės aprašu. Ji bus rodoma formos **Diagnostikos tikrinimo taisyklė** stulpelyje **Taisyklės aprašas** (**DiagnosticsValidationRuleMaintain**). 

> [!NOTE]
> Kad taisyklė veiktų, reikalingas atributas **DiagnosticRuleSubscription**. Paprastai jis naudojamas su **opportunityTitle**, tačiau gali įforminti bet kurį klasės metodą.

Toliau pateikiamas diegimo pavyzdys. Kad būtų paprasčiau, naudojamos neapdorotos eilutės, tačiau, norint diegti tinkamai, reikia naudoti žymas. 

```
[DiagnosticsRuleSubscription(DiagnosticsArea::SCM, 
                             'Assign titles to Request for Quotation cases', 
                             DiagnosticsRunFrequency::Daily,  
                             'This rule detects Requests for Quotation with empty titles.')] 
public str opportunityTitle() 
{ 
    return 'Assign titles to Request for Quotation cases'; 
} 
```

Aprašas, kurį pateikia **opportunityDetails**, rodomas šoninėje srityje, kurioje apie galimybę rodoma daugiau informacijos. Su juo galima naudoti argumentą **SelfHealingOpportunity**, kuris yra laukas **Duomenys** ir kurį naudojant apie galimybę galima pateikti daugiau informacijos. Pavyzdyje metodas pateikia RFQ atvejų tuščiu pavadinimu ID. 

```
public str opportunityDetails(SelfHealingOpportunity _opportunity) 
{ 
    str details = ''; 
    container opportunityData = _opportunity.Data; 
    int affectedRFQCasesCount = conLen(opportunityData); 

    if (affectedRFQCasesCount != 0) 
    { 
        details = 'The following Request for Quotation cases have an empty title:\n'; 
        for (int i = 1; i <= affectedRFQCasesCount ; i++) 
        { 
            PurchRFQCaseId rfqCaseId = conPeek(opportunityData, i); 
            details += rfqCaseId + '\n'; 
        } 
    } 

    return details; 
}
```

Du likę įgyvendinti abstraktūs metodai yra **provideHealingAction** ir **securityMenuItem**. 

Jei nurodomas atkūrimo veiksmas, **provideHealingAction** pateikia true, kitu atveju pateikiama false. Jei pateikiama true, turi būti įdiegtas metodas **performAction**, kitaip bus pateikta klaida. Su metodu **performAction** galima naudoti argumentą **SelfHealingOpportunity**, kuriame su veiksmu galima naudoti duomenis. Pavyzdyje veiksmas atidaro **PurchRFQCaseTableListPage**, kad būtų galima koreguoti rankiniu būdu. 

```
public boolean providesHealingAction() 
{ 
    return true; 
} 

protected void performAction(SelfHealingOpportunity _opportunity) 
{ 
    new MenuFunction(menuItemDisplayStr(PurchRFQCaseTableListPage), MenuItemType::Display).run(); 
} 
```

Gali būti įmanoma naudojant galimybės duomenis imtis automatinių veiksmų – tai priklauso nuo konkrečių taisyklės duomenų. Šiame pavyzdyje sistema galėtų automatiškai generuoti RFQ atvejų pavadinimus. 

**securityMenuItem** pateikia veiksmų meniu elemento pavadinimą, kad taisyklę galėtų matyti tik veiksmų meniu elementą galintys pasiekti vartotojai. Saugos sumetimais gali būti reikalaujama, kad konkrečias taisykles ir galimybes galėtų pasiekti tik įgaliotieji vartotojai. Pavyzdyje peržiūrėti galimybę gali tik prieigą prie **PurchRFQCaseTitleAction** turintys vartotojai. Atkreipkite dėmesį, kad šis veiksmų meniu elementas buvo sukurtas šiam pavyzdžiui ir buvo įtrauktas kaip saugos teisės **PurchRFQCaseTableMaintain** įvesties taškas. 

```
public MenuName securityMenuItem() 
{ 
    return menuItemActionStr(PurchRFQCaseTitleAction); 
}
```

Sukompiliavę taisyklę, vykdykite tolesnę užduotį, kad ji būtų rodoma vartotojo sąsajoje (UI).

```
class ScanNewRulesJob 
{         
    public static void main(Args _args) 
    {         
        SysExtensionCache::clearAllScopes(); 
        var controller = new DiagnosticsRuleController(); 
        controller.runOperation(); 
    } 
} 
```

Taisyklė bus rodoma formoje **Diagnostikos tikrinimo taisyklė**, kurią galima rasti dalyje **Sistemos administravimas** > **Periodinės užduotys** > **Tvarkyti diagnostikos tikrinimo taisyklę**. Norėdami ją įvertinti, eikite į **Sistemos administravimas** > **Periodinės užduotys** > **Planuoti diagnostikos tikrinimo taisyklę**, pasirinkite taisyklės dažnį, pvz., **Kasdien**. Spustelėkite **Gerai**. Norėdami peržiūrėti naująją galimybę, eikite į **Sistemos administravimas** > **Optimizavimo patariamasis įrankis**. 

Norėdami gauti daugiau informacijos, peržiūrėkite trumpą „YouTube“ vaizdo įrašą:

> [!Video https://www.youtube.com/embed/MRsAzgFCUSQ]

