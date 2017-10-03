---
title: Bendrosios savikainos paskirstymo metodas
description: "Šiame straipsnyje pateikiama patarimų, kaip naudoti bendrosios savikainos paskirstymą (TCA). TCA yra paketinio užsakymo pagrindinės sudėtinės prekės ir apibrėžtų formulės sudėtinių produktų savikainos apskaičiavimo metodas."
author: YuyuScheller
manager: AnnBe
ms.date: 04/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: BOMConsistOf, PmfFormulaCoBy
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 83852
ms.assetid: 7c14c3e5-9476-4a79-a210-e77fc91cc7fc
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: mguada
ms.search.validFrom: 2016-02-28T00:00:00.000Z
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 0abcb421eed20f1bca3b39b7d43abd9928f33eb2
ms.contentlocale: lt-lt
ms.lasthandoff: 05/25/2017

---

# <a name="total-cost-allocation-method"></a>Bendrosios savikainos paskirstymo metodas

[!include[banner](../includes/banner.md)]


Šiame straipsnyje pateikiama patarimų, kaip naudoti bendrosios savikainos paskirstymą (TCA). TCA yra paketinio užsakymo pagrindinės sudėtinės prekės ir apibrėžtų formulės sudėtinių produktų savikainos apskaičiavimo metodas.

Bendrosios savikainos paskirstymas (TCA) yra paketinio užsakymo pagrindinės sudėtinės prekės ir apibrėžtų formulės sudėtinių produktų savikainos apskaičiavimo metodas. Šis metodas yra dinamiškas. Juo savikaina apskaičiuojama kaip svertinis baigtais paskelbtų sudėtinės prekės ir sudėtinių produktų kiekių vidurkis. Kai naudojamas TCA, nebūtina peržiūrėti kiekvieno paketinio užsakymo savikainos paskirstymų. Jei TCA nenaudojamas, skaičiuojant formulę naudojamos esamos funkcijos.

## <a name="using-tca-for-coproducts"></a>TCA naudojimas su sudėtiniais produktais
Toliau pateikta keletas nurodymų, kaip TCA naudoti su sudėtiniais produktais.

-   Jei formulės versijos šliaužiklį **Bendrosios savikainos paskirstymas** nustatote į **Taip**, sudėtinių produktų savikaina turi būti didesnė nei 0 (nulis). Reikšmę galima gauti iš tos pačios arba pirmosios nuo vietos nepriklausančios formulės vietos aktyvios savikainos versijos. Ši sąlyga tikrinama tvirtinant formulę.

    -   Jums nereikia neautomatiniu būdu įvesti sudėtinių produktų išlaidų paskirstymo procentų. Sistema automatiškai sukuria išlaidų paskirstymo procentą kaip aktyvių sudėtinių produktų išlaidų vidurkį. 
    -   Jums nereikia įvesti nestandartinių išlaidų prekių, kurios yra sudėtiniai produktai, standartinių išlaidų. Sistemoje pateikiamos dviejų tipų įkainojimo versijos: standartinių išlaidų ir planuojamų išlaidų 
    -   Jei prekė nėra vertinama pagal standartinių išlaidų vertinimo būdą, rekomenduojama naudoti suplanuotų išlaidų versijos aktyvią savikainą. Ši kaina naudojama išlaidoms įvertinti, pvz., KS apskaičiuoti, gamybos išlaidoms įvertinti ir atsargų vertinimo proceso atsarginei kainai nustatyti. 

-   Jei formulės versijos šliaužiklį **Bendrosios savikainos paskirstymas** nustatote į **Taip** ir yra teisingos tolesnės sąlygos, savikainos paskirstymo metodas yra **TCA**, o savikainos paskirstymo procentas nepakinta.
    -   Įtraukėte sudėtinių produktų.
    -   Su sudėtiniais produktais naudojote kitą savikainos paskirstymo metodą.
-   Jei formulės versijos šliaužiklį **Bendrosios savikainos paskirstymas** nustatote į **Ne** ir yra teisingos tolesnės sąlygos, savikainos paskirstymo metodas pakeičiamas į **Rankinis**, o savikainos paskirstymo procentas nepakinta.
    -   Įtraukėte sudėtinių produktų.
    -   Savikainos paskirstymo procentas yra didesnis nei 0 (nulis).
-   Sėkmingai apskaičiuoti formulės negalėsite tol, kol neįvertinsite savikainos paskirstymo procentų. Atlikti šį veiksmą galite rankiniu būdu arba naudodami parinktį **Įvertinti savikainą**, esančią puslapyje **Sudėtiniai produktai**. **Pastaba.** Parinktį **Įvertinti savikainą** galima naudoti tik tada, kai formulės versijos šliaužiklis **Bendrosios savikainos paskirstymas** nustatytas į **Taip**. Peržiūrėti numatomą paskirstymą galite, jei baigtais paskelbti paketinio užsakymo kiekiai atitinka formulėje rodomus kiekius.
-   Kai paketinis užsakymas sukuriamas rankiniu būdu arba patvirtinamas suplanuotas paketinis užsakymas, formulės versijos šliaužiklio **Bendrosios savikainos paskirstymas** reikšmė nukopijuojama į paketinį užsakymą. Tačiau šį parametrą galite pakeisti paketiniame užsakyme. Jei formulės versijos šliaužiklis **Bendrosios savikainos paskirstymas** nustatytas į **Ne**, o tada tas pats paketinio užsakymo šliaužiklis pakeičiamas į **Taip**, kiekvienos eilutės savikainos paskirstymo metodas, nustatytas į **Rankinis**, pakeičiamas į **TCA**. Savikainos paskirstymo metodas **Nėra** nekeičiamas. Jei formulės versijos šliaužiklis **Bendrosios savikainos paskirstymas** nustatytas į **Taip**, o tada tas pats paketinio užsakymo šliaužiklis pakeičiamas į **Ne**, kiekvieno tipo **Gamyba** sudėtinio produkto savikainos paskirstymo metodas pakeičiamas į **Rankinis**. Nekeičiamas joks įvertintas savikainos paskirstymo procentas.
-   Puslapyje **Sudėtinių produktų savikainos paskirstymas** rodomas apskaičiuotas savikainos paskirstymo procentas. Šį puslapį galite atidaryti iš puslapio **Paketinis užsakymas**. Ši informacija yra naudinga, kai paskelbti produktai ir kiekiai skiriasi nuo paketiniame užsakyme esančių suplanuotų arba pradėtų kiekių. Kai savikaina baigta, šie naujieji procentų paskirstymai iš TCA rodomi puslapyje **Sudėtinių produktų savikainos paskirstymas**.

## <a name="calculating-the-burden-for-byproducts"></a>Šalutinių produktų neefektyvių valandų skaičiavimas
Laukas **Šalutinių produktų savikainos paskirstymas**, esantis puslapyje **Sudėtiniai produktai**, yra surašytuvo laukas, naudojamas tik su šalutiniais produktais. Šio sudėtinių produktų lauko reikšmė visada yra **Nėra**. Šiame šalutinių produktų eilučių lauke nustatoma, kaip šalutinio produkto eilutės savikainos suma įtraukiama į bendrąją gamybos savikainą. Galimos toliau nurodytos pasirinktys:

-   **Nėra** ─ į bendrąją gamybos savikainą neįtraukiama jokia šalutinio produkto eilutės suma.
-   **Procentas** ─ savikainos suma apskaičiuojama kaip bendrosios gamyboje sunaudojamų žaliavų savikainos procentas. Lauke įvedamas skaičiuojant naudojamas procentas.
-   **Gaminių kiekiui** ─ savikainos suma apskaičiuojama kaip vieno standartinio gamybos užsakymo paketo dydžio suma. Ši suma nepriklauso nuo paskelbto gamybos kiekio. Lauke įvedama skaičiuojant naudojama suma.
-   **Pagal kiekį** ─ savikainos suma apskaičiuojama pagal paskelbtą gamybos sudėtinės prekės kiekį. Lauke įvedama skaičiuojant naudojama suma.




