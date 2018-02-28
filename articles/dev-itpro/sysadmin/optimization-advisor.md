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

# <a name="create-rules-for-optimization-advisor"></a><span data-ttu-id="18d4d-103">Optimizavimo patariamojo įrankio taisyklių kūrimas</span><span class="sxs-lookup"><span data-stu-id="18d4d-103">Create rules for Optimization advisor</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="18d4d-104">Šioje temoje paaiškinama, kaip sukurti naujų **optimizavimo patariamojo įrankio** taisyklių.</span><span class="sxs-lookup"><span data-stu-id="18d4d-104">This topic explains how to create new rules for **Optimization advisor**.</span></span> <span data-ttu-id="18d4d-105">Pavyzdžiui, galite sukurti naują taisyklę, nustatančią, kurių pasiūlymų patvirtinimų (RFQ) atvejų pavadinimai yra tušti.</span><span class="sxs-lookup"><span data-stu-id="18d4d-105">For example, you can create a new rule that identifies which Request for Quotations (RFQ) cases have an empty title.</span></span> <span data-ttu-id="18d4d-106">Naudojant atvejų pavadinimus, juos lengva nustatyti ir jų ieškoti.</span><span class="sxs-lookup"><span data-stu-id="18d4d-106">Using titles on cases makes them easily identifiable and searchable.</span></span> <span data-ttu-id="18d4d-107">Nors šis pavyzdys gana paprastas, juo parodoma, ko galima pasiekti optimizavimo taisyklėmis.</span><span class="sxs-lookup"><span data-stu-id="18d4d-107">While quite simple, this example shows what can be achieved with optimization rules.</span></span> 

<span data-ttu-id="18d4d-108">*Taisyklė* yra programos duomenų patikra.</span><span class="sxs-lookup"><span data-stu-id="18d4d-108">A *rule* is a check on application data.</span></span> <span data-ttu-id="18d4d-109">Jei išpildoma sąlyga, kurią vertina taisyklė, sukuriama galimybių optimizuoti procesus ar patobulinti duomenis.</span><span class="sxs-lookup"><span data-stu-id="18d4d-109">If the condition that the rule evaluates is met, opportunities to optimize processes or improve data are created.</span></span> <span data-ttu-id="18d4d-110">Dėl galimybių galima imtis veiksmų ir (pasirenkama) galima matuoti veiksmų poveikį.</span><span class="sxs-lookup"><span data-stu-id="18d4d-110">The opportunities can be acted upon and, optionally, the impact of the actions can be measured.</span></span> 

<span data-ttu-id="18d4d-111">Norėdami sukurti naują **optimizavimo patariamojo įrankio** taisyklę, įtraukite naują klasę, išplečiančią abstrakčią klasę **SelfHealingRule**, įdiegiančią **IDiagnosticsRule** sąsają ir kurią įformina atributas **DiagnosticRule**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-111">To create a new rule for the **Optimization advisor**, add a new class that extends the **SelfHealingRule** abstract class, implements the **IDiagnosticsRule** interface, and is decorated by the **DiagnosticRule** attribute.</span></span> <span data-ttu-id="18d4d-112">Klasėje taip pat turi būti metodas, kurį įformina atributas **DiagnosticsRuleSubscription**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-112">The class must also have a method decorated with the **DiagnosticsRuleSubscription** attribute.</span></span> <span data-ttu-id="18d4d-113">Paprastai tai daroma naudojant metodą **opportunityTitle**, kuris bus aptartas vėliau.</span><span class="sxs-lookup"><span data-stu-id="18d4d-113">By convention, that is done on the **opportunityTitle** method, which will be discussed later.</span></span> <span data-ttu-id="18d4d-114">Šią naująją klasę galima įtraukti į pasirinktinį modelį su priklausomybe modelyje **SelfHealingRules**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-114">This new class can be added to a custom model with a dependency on the **SelfHealingRules** model.</span></span> <span data-ttu-id="18d4d-115">Tolesniame pavyzdyje įdiegiama taisyklė vadinama **RFQTitleSelfHealingRule**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-115">In the following example, the rule being implemented is called **RFQTitleSelfHealingRule**.</span></span>

```
[DiagnosticsRule] 
public final class RFQTitleSelfHealingRule extends SelfHealingRule implements IDiagnosticsRule 
{ 
… 
} 
```

<span data-ttu-id="18d4d-116">Abstrakčioje klasėje **SelfHealingRule** yra abstrakčių metodų, kuriuos reikia įdiegti paveldinčiose klasėse.</span><span class="sxs-lookup"><span data-stu-id="18d4d-116">The **SelfHealingRule** abstract class has abstract methods that must be implemented in inheriting classes.</span></span> <span data-ttu-id="18d4d-117">Pagrindas yra metodas **įvertinti**, kuris pateikia taisyklės nustatytų galimybių sąrašą.</span><span class="sxs-lookup"><span data-stu-id="18d4d-117">The core is the **evaluate** method, which returns a list of the opportunities identified by the rule.</span></span> <span data-ttu-id="18d4d-118">Galimybės gali būti taikomos vienam juridiniam subjektui arba visai sistemai.</span><span class="sxs-lookup"><span data-stu-id="18d4d-118">Opportunities can be per legal entity or can apply to the whole system.</span></span>

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

<span data-ttu-id="18d4d-119">Aukščiau parodytas metodas analizuoja įmones ir pasirenka RFQ atvejus su tuščiais pavadinimais metode **findRFQCasesWithEmptyTitle**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-119">The method shown above loops over companies and selects RFQ cases with empty titles in the **findRFQCasesWithEmptyTitle** method.</span></span> <span data-ttu-id="18d4d-120">Jei randamas bent vienas toks atvejis, naudojant metodą **getOpportunityForCompany** sukuriama konkrečios įmonės galimybė.</span><span class="sxs-lookup"><span data-stu-id="18d4d-120">If at least one such case is found, then a company-specific opportunity is created with the **getOpportunityForCompany** method.</span></span> <span data-ttu-id="18d4d-121">Atkreipkite dėmesį, kad lentelės **SelfHealingOpportunity** lauko **Duomenys** tipas yra **Konteineris**, todėl jame gali būti duomenų, susijusių su šiai taisyklei būdinga logika.</span><span class="sxs-lookup"><span data-stu-id="18d4d-121">Notice that the field **Data** in the **SelfHealingOpportunity** table is of type **Container**, and can therefore contain any data relevant to the logic specific to this rule.</span></span> <span data-ttu-id="18d4d-122">Elemente **OpportunityDate** nustačius dabartinę laiko žymą, užregistruojamas vėliausio galimybės įvertinimo laikas.</span><span class="sxs-lookup"><span data-stu-id="18d4d-122">Setting **OpportunityDate** with the current timestamp registers the time of the latest evaluation of the opportunity.</span></span>  

<span data-ttu-id="18d4d-123">Galimybės taip pat gali būti taikomos visoje įmonėje.</span><span class="sxs-lookup"><span data-stu-id="18d4d-123">Opportunities can also be cross-company.</span></span> <span data-ttu-id="18d4d-124">Tokiu atveju įmonių analizė nebūtina ir galimybę reikia kurti naudojant metodą **getOpportunityAcrossCompanies**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-124">In this case, the loop over companies is not necessary and the opportunity must be created with the **getOpportunityAcrossCompanies** method.</span></span> 

<span data-ttu-id="18d4d-125">Tolesniame kode rodomas metodas **findRFQCasesWithEmptyTitle**, pateikiantis RFQ atvejų tuščiais pavadinimais ID.</span><span class="sxs-lookup"><span data-stu-id="18d4d-125">The following code shows the **findRFQCasesWithEmptyTitle** method, which returns the IDs of the RFQ cases that have empty titles.</span></span>

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

<span data-ttu-id="18d4d-126">Dar du įdiegtini metodai yra **opportunityTitle** ir **opportunityDetails**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-126">Two more methods that must be implemented are **opportunityTitle** and **opportunityDetails**.</span></span> <span data-ttu-id="18d4d-127">Pirmasis pateikia trumpą galimybės pavadinimą, pastarasis pateikia išsamų galimybės aprašą, kuriame taip pat gali būti duomenų.</span><span class="sxs-lookup"><span data-stu-id="18d4d-127">The former returns a short title for the opportunity, the latter returns a detailed description of the opportunity, which can also include data.</span></span>

<span data-ttu-id="18d4d-128">Pavadinimas, kurį pateikia **opportunityTitle**, rodomas darbo srities **Optimizavimo patariamasis įrankis** stulpelyje **Optimizavimo galimybė**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-128">The title returned by **opportunityTitle** appears under the **Optimization opportunity** column in the **Optimization advisor** workspace.</span></span> <span data-ttu-id="18d4d-129">Jis taip pat rodomas kaip šoninės srities, kurioje apie galimybę rodoma daugiau informacijos, antraštė.</span><span class="sxs-lookup"><span data-stu-id="18d4d-129">It also appears as the header of the side pane showing more information about the opportunity.</span></span> <span data-ttu-id="18d4d-130">Paprastai šį metodą įformina atributas **DiagnosticRuleSubscription**, su kuriuo galima naudoti tolesnius argumentus.</span><span class="sxs-lookup"><span data-stu-id="18d4d-130">By convention, this method is decorated with the **DiagnosticRuleSubscription** attribute, which takes the following arguments:</span></span> 

* <span data-ttu-id="18d4d-131">**Diagnostikos sritis** – tipo **DiagnosticArea** išvardijimas, apibrėžiantis, kuriai programos sričiai priklauso taisyklė, pvz., **DiagnosticArea::SCM**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-131">**Diagnostic area** – An enum of type **DiagnosticArea** that describes what area of the application the rule belongs to, such as **DiagnosticArea::SCM**.</span></span> 

* <span data-ttu-id="18d4d-132">**Taisyklės pavadinimas** – eilutė su taisyklės pavadinimu.</span><span class="sxs-lookup"><span data-stu-id="18d4d-132">**Rule name** – A string with the rule name.</span></span> <span data-ttu-id="18d4d-133">Ji bus rodoma formos **Diagnostikos tikrinimo taisyklė** stulpelyje **Taisyklės pavadinimas** (**DiagnosticsValidationRuleMaintain**).</span><span class="sxs-lookup"><span data-stu-id="18d4d-133">This will appear under the **Rule name** column in the **Dianostics validation rule** form (**DiagnosticsValidationRuleMaintain**).</span></span> 

* <span data-ttu-id="18d4d-134">**Vykdymo dažnis** – tipo **DiagnosticRunFrequency** išvardijimas, aprašantis, kaip dažnai taisyklę reikėtų vykdyti, pvz., **DiagnosticRunFrequency::Daily**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-134">**Run frequency** – An enum of type **DiagnosticRunFrequency** that describes how often the rule should be run, such as **DiagnosticRunFrequency::Daily**.</span></span> 

* <span data-ttu-id="18d4d-135">**Taisyklės aprašas** – eilutė su išsamesniu taisyklės aprašu.</span><span class="sxs-lookup"><span data-stu-id="18d4d-135">**Rule description** – A string with a more detailed description of the rule.</span></span> <span data-ttu-id="18d4d-136">Ji bus rodoma formos **Diagnostikos tikrinimo taisyklė** stulpelyje **Taisyklės aprašas** (**DiagnosticsValidationRuleMaintain**).</span><span class="sxs-lookup"><span data-stu-id="18d4d-136">This will appear under the **Rule description** column in the **Dianostics validation rule** form (**DiagnosticsValidationRuleMaintain**).</span></span> 

> [!NOTE]
> <span data-ttu-id="18d4d-137">Kad taisyklė veiktų, reikalingas atributas **DiagnosticRuleSubscription**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-137">The **DiagnosticRuleSubscription** attribute is required for the rule to work.</span></span> <span data-ttu-id="18d4d-138">Paprastai jis naudojamas su **opportunityTitle**, tačiau gali įforminti bet kurį klasės metodą.</span><span class="sxs-lookup"><span data-stu-id="18d4d-138">Typically, it is used on **opportunityTitle**, but it can decorate any method of the class.</span></span>

<span data-ttu-id="18d4d-139">Toliau pateikiamas diegimo pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="18d4d-139">The following is an example implementation.</span></span> <span data-ttu-id="18d4d-140">Kad būtų paprasčiau, naudojamos neapdorotos eilutės, tačiau, norint diegti tinkamai, reikia naudoti žymas.</span><span class="sxs-lookup"><span data-stu-id="18d4d-140">Raw strings are used for simplicity, but a correct implementation requires labels.</span></span> 

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

<span data-ttu-id="18d4d-141">Aprašas, kurį pateikia **opportunityDetails**, rodomas šoninėje srityje, kurioje apie galimybę rodoma daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="18d4d-141">The description returned by **opportunityDetails** appears on the side pane showing more information about the opportunity.</span></span> <span data-ttu-id="18d4d-142">Su juo galima naudoti argumentą **SelfHealingOpportunity**, kuris yra laukas **Duomenys** ir kurį naudojant apie galimybę galima pateikti daugiau informacijos.</span><span class="sxs-lookup"><span data-stu-id="18d4d-142">This takes the **SelfHealingOpportunity** argument, which is **Data** field that can be used to provide more details about the opportunity.</span></span> <span data-ttu-id="18d4d-143">Pavyzdyje metodas pateikia RFQ atvejų tuščiu pavadinimu ID.</span><span class="sxs-lookup"><span data-stu-id="18d4d-143">In the example, the method returns the IDs of the RFQ cases with an empty title.</span></span> 

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

<span data-ttu-id="18d4d-144">Du likę įgyvendinti abstraktūs metodai yra **provideHealingAction** ir **securityMenuItem**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-144">The two remaining abstract methods to implement are **provideHealingAction** and **securityMenuItem**.</span></span> 

<span data-ttu-id="18d4d-145">Jei nurodomas atkūrimo veiksmas, **provideHealingAction** pateikia true, kitu atveju pateikiama false.</span><span class="sxs-lookup"><span data-stu-id="18d4d-145">**provideHealingAction** returns true if a healing action is provided, otherwise, it returns false.</span></span> <span data-ttu-id="18d4d-146">Jei pateikiama true, turi būti įdiegtas metodas **performAction**, kitaip bus pateikta klaida.</span><span class="sxs-lookup"><span data-stu-id="18d4d-146">If true is returned, the method **performAction** must be implemented, or an error will be thrown.</span></span> <span data-ttu-id="18d4d-147">Su metodu **performAction** galima naudoti argumentą **SelfHealingOpportunity**, kuriame su veiksmu galima naudoti duomenis.</span><span class="sxs-lookup"><span data-stu-id="18d4d-147">The **performAction** method takes a **SelfHealingOpportunity** argument, in which the data can be used for the action.</span></span> <span data-ttu-id="18d4d-148">Pavyzdyje veiksmas atidaro **PurchRFQCaseTableListPage**, kad būtų galima koreguoti rankiniu būdu.</span><span class="sxs-lookup"><span data-stu-id="18d4d-148">In the example, the action opens the **PurchRFQCaseTableListPage**, for manual correction.</span></span> 

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

<span data-ttu-id="18d4d-149">Gali būti įmanoma naudojant galimybės duomenis imtis automatinių veiksmų – tai priklauso nuo konkrečių taisyklės duomenų.</span><span class="sxs-lookup"><span data-stu-id="18d4d-149">Depending on the specifics of the rule, it might be possible to take an automatic action using the opportunity data.</span></span> <span data-ttu-id="18d4d-150">Šiame pavyzdyje sistema galėtų automatiškai generuoti RFQ atvejų pavadinimus.</span><span class="sxs-lookup"><span data-stu-id="18d4d-150">In this example, the system could generate titles for RFQ cases automatically.</span></span> 

<span data-ttu-id="18d4d-151">**securityMenuItem** pateikia veiksmų meniu elemento pavadinimą, kad taisyklę galėtų matyti tik veiksmų meniu elementą galintys pasiekti vartotojai.</span><span class="sxs-lookup"><span data-stu-id="18d4d-151">**securityMenuItem** returns the name of an action menu item such that the rule is only visible to users who can access the action menu item.</span></span> <span data-ttu-id="18d4d-152">Saugos sumetimais gali būti reikalaujama, kad konkrečias taisykles ir galimybes galėtų pasiekti tik įgaliotieji vartotojai.</span><span class="sxs-lookup"><span data-stu-id="18d4d-152">Security might require that specific rules and opportunities are accessible only to authorized users.</span></span> <span data-ttu-id="18d4d-153">Pavyzdyje peržiūrėti galimybę gali tik prieigą prie **PurchRFQCaseTitleAction** turintys vartotojai.</span><span class="sxs-lookup"><span data-stu-id="18d4d-153">In the example, only users with access to **PurchRFQCaseTitleAction** can view the opportunity.</span></span> <span data-ttu-id="18d4d-154">Atkreipkite dėmesį, kad šis veiksmų meniu elementas buvo sukurtas šiam pavyzdžiui ir buvo įtrauktas kaip saugos teisės **PurchRFQCaseTableMaintain** įvesties taškas.</span><span class="sxs-lookup"><span data-stu-id="18d4d-154">Notice that this action menu item was created for this example, and was added as an entry point for the **PurchRFQCaseTableMaintain** security privilege.</span></span> 

```
public MenuName securityMenuItem() 
{ 
    return menuItemActionStr(PurchRFQCaseTitleAction); 
}
```

<span data-ttu-id="18d4d-155">Sukompiliavę taisyklę, vykdykite tolesnę užduotį, kad ji būtų rodoma vartotojo sąsajoje (UI).</span><span class="sxs-lookup"><span data-stu-id="18d4d-155">After the rule has compiled, execute the following job to have it display in the user interface (UI).</span></span>

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

<span data-ttu-id="18d4d-156">Taisyklė bus rodoma formoje **Diagnostikos tikrinimo taisyklė**, kurią galima rasti dalyje **Sistemos administravimas** > **Periodinės užduotys** > **Tvarkyti diagnostikos tikrinimo taisyklę**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-156">The rule will display in the **Diagnostics validation rule** form, available from **System administration** > **Periodic tasks** > **Maintain diagnostics validation rule**.</span></span> <span data-ttu-id="18d4d-157">Norėdami ją įvertinti, eikite į **Sistemos administravimas** > **Periodinės užduotys** > **Planuoti diagnostikos tikrinimo taisyklę**, pasirinkite taisyklės dažnį, pvz., **Kasdien**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-157">To have it evaluated, go to **System administration** > **Periodic tasks** > **Schedule diagnostics validation rule**, select the frequency of the rule, such as **Daily**.</span></span> <span data-ttu-id="18d4d-158">Spustelėkite **Gerai**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-158">Click **OK**.</span></span> <span data-ttu-id="18d4d-159">Norėdami peržiūrėti naująją galimybę, eikite į **Sistemos administravimas** > **Optimizavimo patariamasis įrankis**.</span><span class="sxs-lookup"><span data-stu-id="18d4d-159">Go to **System administration** > **Optimization advisor** to view the new opportunity.</span></span> 

<span data-ttu-id="18d4d-160">Norėdami gauti daugiau informacijos, peržiūrėkite trumpą „YouTube“ vaizdo įrašą:</span><span class="sxs-lookup"><span data-stu-id="18d4d-160">For more information, watch the short YouTube video:</span></span>

> [!Video https://www.youtube.com/embed/MRsAzgFCUSQ]
