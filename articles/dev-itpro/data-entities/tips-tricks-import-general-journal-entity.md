---
title: "Geriausios kvitų importavimo naudojant objektą Bendrasis žurnalas praktikos"
description: "Šioje temoje pateikiama patarimų, kaip į bendrąjį žurnalą importuoti duomenų naudojant objektą Bendrasis žurnalas."
author: twheeloc
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.custom: 94363
ms.assetid: 0b8149b5-32c5-4518-9ebd-09c9fd7f4cfc
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 688fa17072cb340d6d02be31528339fb98601825
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="best-practices-for-importing-vouchers-using-the-general-journal-entity"></a>Geriausios kvitų importavimo naudojant objektą Bendrasis žurnalas praktikos

[!include[banner](../includes/banner.md)]


Šioje temoje pateikiama patarimų, kaip į bendrąjį žurnalą importuoti duomenų naudojant objektą Bendrasis žurnalas.  

Naudodami objektą Bendrasis žurnalas galite importuoti kvitus, kurių sąskaitos ar korespondentinės sąskaitos tipas yra **Didžioji knyga, Klientas, Tiekėjas arba Bankas**. Kvito duomenis galima įvesti vienoje eilutėje naudojant laukus **Sąskaita** ir **Korespondentinė sąskaita** arba keliose eilutėse, kuriose naudojamas tik laukas **Sąskaita**, o kiekvienoje eilutėje laukas **Korespondentinė sąskaita** paliekamas tuščias. Objekte Bendrasis žurnalas nepalaikomi visi sąskaitos tipai. Jeigu reikalingi skirtingi sąskaitų tipų deriniai, geriau naudoti kitus objektus. Pavyzdžiui, naudokite objektą Projekto išlaidų žurnalas projekto operacijai importuoti. Kiekvienas objektas sukurtas konkretiems scenarijams palaikyti, todėl papildomi laukai gali būti pasiekiami konkrečiuose objektuose naudojant tam tikrus scenarijus, tačiau papildomų laukų nebus konkrečiuose objektuose naudojant kitus scenarijus.

## <a name="setup"></a>Sąranka
Kol dar neimportavote naudodami objektą Bendrasis žurnalas, patikrinkite toliau nurodytą sąranką.

-   **Žurnalo paketo numerio numeracijos sąranka** – pagal numatytuosius parametrus importuojant ir naudojant objektą Bendrasis žurnalas, žurnalo paketo numeryje naudojama numeracija, nurodyta DK parametruose. Jei nustatysite žurnalo paketo numerio numeracijos parinktį **Neautomatinis**, numatytasis numeris nebus taikomas. Šis nustatymas nepalaikomas.
-   **Finansinių dimensijų konfigūracija** – kiekviena organizacija turi nurodyti finansinių dimensijų tvarką, skirtą operacijoms importuoti naudojant objektus. Formato **DK dimensijų integracija** tvarka nustatoma dalyje **DK** &gt; **Sąskaitų planas** &gt; **Dimensijos** &gt; **Finansinių dimensijų konfigūravimas, kad būtų galima integruoti programas** &gt; **Pasirinkti duomenų objektus**. Importuojamos DK sąskaitos segmentų tvarka turi būti ta tokia pati. Kitaip importavimo metu įvyks klaida.

## <a name="general-journal-entity-setup"></a>Objekto Bendrasis žurnalas nustatymas
Du toliau pateikti duomenų valdymo parametrai nulemia numatytojo žurnalo paketo numerio arba kvito numerio pritaikymo pobūdį.

-   **Apdorojimas pagal rinkinį** (duomenų objekte)
-   **Automatiškai sugeneruotas** (laukų susiejime)

Tolesniuose skyriuose apibūdinama, kaip šie parametrai veikia, ir paaiškinama, kaip generuojami žurnalo paketo numeriai ir kvitų numeriai.

### <a name="journal-batch-number"></a>Žurnalų paketo numeris

-   Objekto Bendrasis žurnalas nustatymas **Rinkiniu pagrįstas apdorojimas** generuojant žurnalo paketo numerius įtakos neturi.
-   Jei laukas **Žurnalo paketo numeris** nustatytas į parinktį **Automatiškai sugeneruotas**, sukuriamas naujas kiekvienos importuojamos eilutės žurnalo paketo numeris. Taip daryti nerekomenduojama. Nustatymą **Automatiškai sugeneruotas** galima rasti importavimo projekto dalie **Peržiūrėti schemą** skirtuke **Susiejimo informacija**.
-   Jei laukas **Žurnalo paketo numeris** nėra nustatytas į parinktį **Automatiškai sugeneruotas**, žurnalo paketo numeris, kaip nurodyta toliau.
    -   Jei importuoto failo žurnalo paketo numeris atitinka esamą neregistruoto kasdieninio žurnalo numerį, į esamą žurnalą importuojamos visos eilutės, kurių žurnalo paketo numeris atitinka. Eilutės niekada neimportuojamos į užregistruotą žurnalo paketo numerį. Vietoj to sukuriamas naujas numeris.
    -   Jei importuoto failo žurnalo paketo numeris neatitinka esamo neregistruoto kasdieninio žurnalo numerio, visos eilutės, kurių žurnalo paketo numeris toks pat, įtraukiamos į naują žurnalą. Pvz., visos eilutės, kurių žurnalo paketo numeris yra 1, importuojamos į naują žurnalą, o visos eilutės, kurių žurnalo paketo numeris yra 2, importuojamos į antrą naują žurnalą. Žurnalo paketo numeris sukuriamas naudojant numeraciją, kuri nurodyta DK parametruose.

### <a name="voucher-number"></a>Kvito numeris

-   Kai naudojate objekto Bendrasis žurnalas nustatymą **Rinkiniu pagrįstas apdorojimas**, kvito numeris turi būti nurodytas importuojamame faile. Kiekvienai bendrojo žurnalo operacijai priskiriamas kvito numeris, nurodytas importuojamame faile, net jei kvitas nėra subalansuotas. Jei norite naudoti apdorojimo pagal rinkinį parametrą bei nustatytą kvitų numerių numeraciją, 2016 m. vasario mėn. leidime pateikiamos karštosios pataisos. Karštosios pataisos numeris yra 3170316 ir ją galima atsisiųsti iš „Lifecycle services“ (LCS). Daugiau informacijos žr. [Karštųjų pataisų atsisiuntimas iš „Lifecycle services“](..\migration-upgrade\download-hotfix-lcs.md).
    -   Norėdami įgalinti šią funkciją, žurnalo pavadinime, kuris naudojamas importavimo operacijoms atlikti, nustatykite parinktį **Numerių paskirstymas registruojant** kaip **Taip**.
    -   Kvito numeris vis tiek turi būti nurodytas importuojamame faile. Tačiau šis numeris yra laikinas ir registruojant žurnalą jis bus perrašytas naudojant kvito numerį. Įsitikinkite, kad visos žurnalo eilutės yra tinkamai sugrupuotos pagal laikiną kvito numerį. Pavyzdžiui, registruojant surandamos trys eilutės, kurių laikinas kvito numeris – 1. Laikinas visų trijų eilučių kvito numeris perrašomas naudojant paskesnį numeracijos numerį. Jei šios trys eilutės nėra subalansuotas įrašas, kvitas nėra registruojamas. Tada, jei rasta eilučių, kurių laikino kvito numeris yra 2, šis numeris yra perrašomas naudojant paskesnį numeracijos kvito numerį, ir t. t.

<!-- -->

-   Kai parametro **Apdorojimas pagal rinkinį** nenaudojate, importuojamame faile neturite pateikti kvito numerio. Kvitų numeriai sukuriami importavimo metu pagal žurnalo pavadinimo nustatymą (**Tik vienas kvitas**, **Pagal balansą**, ir t. t.). Pavyzdžiui, jei žurnalo pavadinimo nustatymas yra **Pagal balansą**, pirmai eilutei priskiriamas naujas numatytasis kvito numeris. Tada sistema vertina eilutę, siekdama nustatyti, ar debeto sumos lygios kredito sumoms. Jei eilutėje nurodyta korespondentinė sąskaita, kitai importuojamai eilutei priskiriamas naujas kvito numeris. Jei korespondentinė sąskaita nenurodyta, sistema įvertina, ar debeto sumos lygios kredito sumoms, kai importuojama kiekviena nauja eilutė.
-   Jei laukas **Kvito numeris** nustatytas į parinktį **Automatiškai sugeneruotas**, importuoti nepavyks. Lauko **Kvito numeris** nustatymas **Automatiškai sugeneruotas** nepalaikomas.

Pagal numatytuosius parametrus objektas Bendrasis žurnalas naudoja rinkiniu pagrįstą apdorojimą. Įvertinę savo organizacijos verslo poreikius, nustatymą **Rinkiniu pagrįstas apdorojimas** galite pakeisti, darbo srityje **Duomenų valdymas** spustelėdami **Duomenų objektai**. Rinkiniu pagrįstas apdorojimas yra naudojamas importavimo procesui pagreitinti. Jeigu naudojate rinkiniu pagrįsto apdorojimo, importavimo procesas naudojant objektą Bendrasis žurnalas bus lėtesnis.




