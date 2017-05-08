---
title: "Standartinių išlaidų atnaujinimas ne gamybos aplinkoje"
description: "Šiame straipsnyje patariama, kaip standartines išlaidas atnaujinti ne gamybos aplinkoje."
author: YuyuScheller
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: CostingVersion, InventItemPrice
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 79723
ms.assetid: 7ba0c408-2450-4042-9542-6fdf83c12e6c
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: mguada
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 9ccbe5815ebb54e00265e130be9c82491aebabce
ms.openlocfilehash: be3e5417341094caf0565c1c5ee4f9cbc40f8e76
ms.lasthandoff: 03/31/2017


---

# <a name="update-standard-costs-in-a-non-manufacturing-environment"></a>Standartinių išlaidų atnaujinimas ne gamybos aplinkoje

[!include[banner](../includes/banner.md)]


Šiame straipsnyje patariama, kaip standartines išlaidas atnaujinti ne gamybos aplinkoje.

Šios rekomendacijos taikomos, jei naudojate dviejų versijų standartinių išlaidų naujinimo būdą. Naudojant šį būdą, viena įkainojimo versija turi iš pradžių nustatytas standartines įšaldyto laikotarpio išlaidas, o antra įkainojimo versija turi papildančiuosius naujinimus. Kiekvienas naujinimas įvedamas kaip išlaidų įrašas antroje įkainojimo versijoje ir galiausiai jis suaktyvinamas. Alternatyvus būdas yra vienos versijos įkainojimas, naudojant iš pradžių apibrėžtų standartinių išlaidų rinkinį. Dviejų versijų būdui reikalingas antros įkainojimo versijos apibrėžimas. Toliau pateikti patarimai, kaip apibrėžti šią įkainojimo versiją.

-   Priskirkite įkainojimo tipą **Standartinės išlaidos**.
-   Priskirkite reikšmingą identifikatorių, kuris nurodo įkainojimo versijos turinį, pvz., **2016-NAUJINIMAI**.
-   Įsitikinkite, kad turinyje yra išlaidų įrašai.
-   Leiskite įvesti visų vietų išlaidų įrašus. Jei nurodote vietą, galima įvesti tik tos vietos išlaidų įrašus.
-   Nurodykite atsarginį principą **Nėra**. Atsarginis principas taikomas tik pagamintų prekių išlaidų skaičiavimams.

Norėdami patikslinti, pakoreguoti arba atnaujinti standartines naujų prekių išlaidas, atlikite šiuos veiksmus.

1.  Naudodami puslapį **Įkainojimo versijos** **nustatymas**, galite išlaidų duomenis leisti įvesti į antrą įkainojimo versiją. Nebūtina: neleiskite suaktyvinti laukiančių išlaidų, kad suaktyvinti būtų leista tik išsamiai ir tiksliai apibrėžus laukiančias išlaidas. Nebūtina: taip pat galite įvesti datą lauke **Pradžios data**. Bendra gairė – datą naudoti ketinant įgalinti papildančiuosius naujinimus. Taip pat įkainojimo versijos lauką **Pradžios data** galite palikti tuščią, o datą įvesti kiekvieno išlaidų įrašo lauke **Pradžios data**.
2.  Naudodami puslapį **Prekės kaina**, naujinimus galite įvesti kaip prekių išlaidų įrašus antrojoje įkainojimo versijoje.
3.  Naudodami ataskaitą **Prekių kainos** galite tikrinti prekių išlaidų įrašų antrojoje įkainojimo versijoje užbaigtumą ir tikslumą.
4.  Naudodami puslapį **Įkainojimo versijos tvarkymas**, galite pakeisti blokavimo vėliavėlę, kad leistumėte aktyvinti laukiančius išlaidų įrašus antrojoje įkainojimo versijoje.
5.  Naudodami puslapį **Aktyvinti kainas** (kurį galite atidaryti iš puslapio **Įkainojimo versijos tvarkymas**), galite aktyvinti laukiančius išlaidų įrašus antrojoje įkainojimo versijoje. Aktyvinti atskirų prekių laukiančių išlaidų įrašus taip pat galite puslapyje **Prekės kaina** spustelėdami mygtuką **Aktyvinti laukiančią kainą**.
6.  Kad nereikėtų papildomai tvarkyti duomenų, naudokite puslapį **Įkainojimo versijos nustatymas**, kad pakeistumėte blokavimo vėliavėles antrojoje įkainojimo versijoje. Blokavimo strategija apsaugos nuo naujų laukiančių išlaidų įvedimo ir laukiančių išlaidų aktyvinimo.




