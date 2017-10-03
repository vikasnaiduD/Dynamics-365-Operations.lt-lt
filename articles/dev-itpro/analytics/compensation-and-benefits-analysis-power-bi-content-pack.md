---
title: "Kompensacijų ir išmokų „Power BI“ turinys"
description: "Šioje temoje aprašytas „Finance and Operations“ kompetencijų ir išmokų „Power BI“ turinys. Paaiškinama, kaip pasiekti į turinio paketą įtrauktas ataskaitas, ir pateikiama informacija apie duomenų modelį ir objektus, naudojamus turinio paketui kurti."
author: jcart1106
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Operations, UnifiedOperations
ms.custom: 263914
ms.assetid: 18634bb5-3341-42f2-9cc9-7b04708b506b
ms.search.region: Global
ms.author: jcart
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: 869151f2486b7a481e4694cfb6992d0ee2cfc008
ms.openlocfilehash: 70e35a33e06fe7c89dd64d17703f19a71d4a157e
ms.contentlocale: lt-lt
ms.lasthandoff: 06/13/2017

---

# <a name="compensation-and-benefits-power-bi-content"></a>Kompensacijų ir išmokų „Power BI“ turinys

[!include[banner](../includes/banner.md)]


Šioje temoje aprašytas „Finance and Operations“ kompetencijų ir išmokų „Power BI“ turinys. Paaiškinama, kaip pasiekti į turinio paketą įtrauktas ataskaitas, ir pateikiama informacija apie duomenų modelį ir objektus, naudojamus turinio paketui kurti.

<a name="accessing-the-content-pack"></a>Prieiga prie turinio paketo
--------------------------

Kompetencijų ir išmokų turinio paketą galite rasti bendrai naudojamo turto bibliotekoje „Microsoft Dynamics Lifecycle Services“ (LCS). Daugiau informacijos apie tai, kaip atsisiųsti turinio paketą ir prijungti jį prie „Microsoft Dynamics 365 for Finance and Operations“ duomenų, žr. [„Power BI“ turinys LCS iš „Microsoft“ ir jūsų partnerių](power-bi-content-microsoft-partners.md).

## <a name="reports-that-are-included-in-the-content-pack"></a>Į turinio paketą įtrauktos ataskaitos
Prijungus turinio paketą prie „Finance and Operations“ duomenų, ataskaitose rodomi jūsų organizacijos duomenys. Jei niekada nenaudojote „Microsoft Power BI“, daugiau apie tai galite sužinoti temoje [„Power BI“ mokymosi vedlio puslapis](https://powerbi.microsoft.com/en-us/guided-learning/?WT.mc_id=PBIService_GetData). Į turinio paketą įtrauktose ataskaitose yra diagramos ir lentelės, kuriose pateikiama papildoma informacija. Tolesnėje lentelėje aprašomos ataskaitos.

| Ataskaita                     | Turinys                                                                                                                              |
|----------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Kompensacijų ir išmokų analizė | Valandinį ir fiksuotą užmokestį gaunantys darbuotojai pagal įmonę, vidutinis valandinis užmokestis, vidutinis fiksuotas užmokestis, darbuotojai pagal įdarbinimo tipą ir plano registracija |
| Darbuotojų išmokos          | Darbuotojo registravimas pagal pasirinktą išmoką                                                                                               |

Šių ataskaitų diagramas ir plyteles galima filtruoti ir prisegti prie ataskaitų srities. Daugiau informacijos apie tai, kaip „Power BI“ filtruoti ir prisegti, žr. [Ataskaitų srities kūrimas ir konfigūravimas](https://powerbi.microsoft.com/en-us/guided-learning/powerbi-learning-4-2-create-configure-dashboards).

## <a name="understanding-the-data-model-and-entities"></a>Duomenų modelio ir objektų supratimas
„Finance and Operations“ duomenys naudojami ataskaitoms kompetencijų ir išmokų turinio pakete užpildyti. Toliau pateiktoje lentelėje nurodomi objektai, kuriais turinio paketas pagrįstas.

| Objektas                            | Turinys                                                                                                   | Ryšiai su kitais objektais                                                                                                                                                                                                                                                                                                |
|-----------------------------------|------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Workforce\_CalendarOffset         | Kalendoriaus poslinkiai ataskaitoms skaidyti                                                                          | Workforce\_PastPositionAssignment Workforce\_PositionTrend Workorce\_WorkerTrend Workforce\_TerminatedWorker                                                                                                                                                                                                                     |
| Workforce\_Company                | Įmonės, pagal kurias filtruojamos ataskaitos                                                                             | Workforce\_CurrentCompensation Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                        |
| Workforce\_Compensation           | Užmokesčio tarifas ir dažnis per tam tikrą laikotarpį                                                                           | Workforce\_CurrentCompensation Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                        |
| Workforce\_CurrentCompensation    | Užmokesčio tarifas ir dažnis dabartinę dieną                                                              | Workforce\_Company Workforce\_Compensation Workforce\_Demographics Workforce\_Job Workforce\_Position                                                                                                                                                                                                                            |
| Workforce\_CurrentPosition        | Pareigos dabartinę datą, viso etato ekvivalentas (FTE), laisvos darbo vietos ir laisvos / užimtos darbo vietos | Workforce\_Job Workforce\_Position                                                                                                                                                                                                                                                                                               |
| Workforce\_CurrentWorker          | Darbuotojai dabartinę dieną, amžius ir darbuotojų skaičius                                                         | Workforce\_Company Workforce\_Compensation Workforce\_GeographicLocation Workforce\_Performance Workforce\_WorkerName Workforce\_ReportsToWorkerName Workforce\_WorkerTitle Workforce\_Demographics Workforce\_Job Workforce\_Employment Workforce\_Position Workforce\_WorkerBenefit                                            |
| Workforce\_Date                   | Dienos, savaitės, mėnesiai ir metai                                                                             | Workforce\_PastPositionAssignment Workforce\_PositionTrend Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                     |
| Workforce\_Demographics           | Gimimo data, lytis etninė kilmė ir šeimyninė padėtis                                                   | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workforce\_Employment             | Pradžios data, pabaigos data ir perėjimo data                                                                  | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workforce\_GeographicLocation     | Miestas, seniūnija, pašto kodas ir šalis arba regionas                                                           | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workforce\_Job                    | Funkcija, tipas ir pareigos                                                                                  | Workforce\_CurrentPosition Workforce\_CurrentWorker                                                                                                                                                                                                                                                                              |
| Workforce\_PastPositionAssignment | Priskyrimo priežastis, pradžios data, pabaigos data ir užduotis                                                           | Workforce\_CalendarOffset Workforce\_Date Workforce\_Job Workforce\_Position                                                                                                                                                                                                                                                     |
| Workforce\_Performance            | Įvertinimas, aprašas ir įvertinimo modelis                                                                      | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workforce\_Position               | Padalinys, FTE, pareigos, pareigų tipas ir pareigos                                                        | Workforce\_CurrentPosition Workforce\_CurrentWorker                                                                                                                                                                                                                                                                              |
| Workforce\_PositionTrend          | Pareigos per tam tikrą laikotarpį, FTE ir užduotis                                                                          | Workforce\_CalendarOffset Workforce\_Date Workforce\_Job Workforce\_Position                                                                                                                                                                                                                                                     |
| Workforce\_ReportsToWorkerName    | Vardas, pavardė ir vardas bei pavardė                                                                       | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workforce\_Skill                  | Įgūdis, įgūdžio tipas ir įvertinimas                                                                              |                                                                                                                                                                                                                                                                                                                                  |
| Workforce\_TerminatedWorker       | Atleisti darbuotojai, atleidimo data, pareigos ir užduotis                                             | Workforce\_Company Workforce\_Compensation Workforce\_GeographicLocation Workforce\_Performance Workforce\_WorkerName Workforce\_ReportsToWorkerName Workforce\_CalendarOffset Workforces\_Date Workforce\_WorkerTitle Workforce\_Demographics Workforce\_Employment Workforce\_Job Workforce\_Position Workforce\_WorkerBenefit |
| Workforce\_WorkerBenefit          | Galiojimo data, išmokos parinktis, išmokos planas ir išmokos tipas                                             | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workforce\_WorkerName             | Vardas, pavardė ir vardas bei pavardė                                                                       | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workforce\_WorkerTitle            | Pareigos ir paaukštinimo data                                                                                   | Workforce\_CurrentWorker Workforce\_TerminatedWorker Workorce\_WorkerTrend                                                                                                                                                                                                                                                       |
| Workorce\_WorkerTrend             | Darbuotojai per tam tikrą laiką, darbuotojų skaičius, įmonė ir pareigos                                                        | Workforce\_Company Workforce\_Compensation Workforce\_GeographicLocation Workforce\_Performance Workforce\_WorkerName Workforce\_ReportsToWorkerName Workforce\_CalendarOffset Workforces\_Date Workforce\_WorkerTitle Workforce\_Demographics Workforce\_Employment Workforce\_Job Workforce\_WorkerBenefit                     |

Šie objektai buvo naudojami skaičiuojamiems matams duomenų modelyje sukurti. Tada šie skaičiuojami matai naudojami skaičiuojant pagrindinius efektyvumo indikatorius (KPI) ir ataskaitas, naudojamas turinio pakete. Jei norite į ataskaitas ir ataskaitų sritį įtraukti papildomų skaičiavimų, galite iš LCS atsisiųsti ir modifikuoti failą CompensationandBenefits.pbix. Šis failas yra numatytasis duomenų modelis, kuris buvo naudojamas turinio paketui kurti. Atlikę keitimus, galite kurti organizacinį turinio paketą ir ataskaitų sritį, kuriuose yra jūsų įtraukta informacija.

## <a name="additional-resources"></a>Papildomi ištekliai
Toliau pateikti keli naudingi saitai, susiję su objektais ir „Power BI“ turinio kūrimu.

-   [Duomenų objektai](https://blogs.msdn.microsoft.com/dynamicsaxbi/2016/06/09/power-bi-integration-with-entity-store-in-dynamics-ax-7-may-update/)
-   [Organizacinių turinio paketų kūrimas](https://powerbi.microsoft.com/en-us/documentation/powerbi-service-organizational-content-packs-introduction/)
-   [Duomenų modeliavimas naudojant „Power BI“](https://powerbi.microsoft.com/en-us/guided-learning/powerbi-learning-2-1-intro-modeling-data)
-   [„Power BI“ plytelių įtraukimas į darbo sritis](https://blogs.msdn.microsoft.com/dynamicsaxbi/2016/07/06/pinning-power-bi-reports-to-dynamics-ax-client/)




