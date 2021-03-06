---
title: "Vienetų paėmimo patvirtinimas"
description: "Šioje temoje aprašoma, kaip nustatyti ir taikyti vienetų paėmimo patvirtinimą iš mobiliojo įrenginio."
author: Mirzaab
manager: AnnBe
ms.date: 05/26/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: WHSRFAutoConfirm, WHSRFMenuItem
audience: Application User
ms.reviewer: bis
ms.search.scope: Core, Operations
ms.custom: 269384
ms.search.region: Global
ms.author: mirzaab
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 5ef9ab68c20ae095de03b0a0e05aa15ef5bf8a5d
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="piece-picking-confirmation"></a>Vienetų paėmimo patvirtinimas

[!include[banner](../includes/banner.md)]

Vienetų paėmimas suteikia galimybę patvirtinti kiekvieną atsargų vienetą naudojant paėmimo ir skaičiavimo darbą mobiliajame įrenginyje. Paėmimų atveju galite patvirtinti darbo kiekį, kuris bus atliktas neviršijant kiekio, nurodyto paimtinam darbui. Skaičiavimo darbo atveju galite nuskaityti atsargas, kurias skaičiuojate, ir sekti bendrą sumą.

Kai įgalinate vienetų paėmimą, automatiškai pasirenkamas produkto patvirtinimas. Darbo tipo paėmimų atveju įgalinamas maksimalus vienetų skaičius. Tai leidžia nustatyti maksimalų skaičių vienetų, kurie turi būti patvirtinti darbo proceso metu. Didžiausias kiekis paremtas dabartiniu darbo vienetu, kuris yra vykdomas. Skaičiavimo darbo tipo atveju negalima nustatyti maksimalaus skaičiaus.

Taip pat galite naudoti kiekį ir matavimo vienetą (MV), susietą su nuskaitytu brūkšniniu kodu. Tai veiks gaunant gavimo srautus, įskaitant mišraus numerio lentelių gavimą, pirkimo užsakymo prekę, perkėlimo užsakymo prekę ir krovinio prekę. Tai taip pat veikia dalių paėmimo atveju, kai nuskaičius brūkšninį kodą prie patvirtintų vienetų bendro skaičiaus bus pridėtas kiekis bei konvertuojami brūkšninio kodo MV ir darbo vienetas. Jei skaičiuojant brūkšninio kodo MV patvirtinama, kad sekų grupės skaičiavimui kiekis leidžiamas, kiekis pridedamas prie bendros sumos.

## <a name="where-it-applies"></a>Kai taikoma

Vienetų paėmimas veikia visų skaičiavimo darbų atveju ir pradinio bet kurio tipo darbo paėmimo atveju. Vienetų paėmimas netaikomas, jei prekė kontroliuojama pagal serijos numerius arba jei tai yra gamybos, arba „kanban“ paėmimas iš numerio lentelės (LP) vietos ir prekė nustatyta išdėstyti.

## <a name="set-up-piece-picking"></a>Nustatyti vienetų paėmimą

1.  Mobiliojo įrenginio meniu elemente atidarykite darbo patvirtinimo sąrankos formą: Sandėlio valdymas > **Sandėlio valdymas** > **Sąranka** > **Mobilusis įrenginys** > **Mobiliojo įrenginio meniu elementai**. 
2. Mobiliojo įrenginio meniu elemente atidarykite Darbo patvirtinimo sąranka.

Kai darbo tipas yra paėmimas arba skaičiavimas, galima pasirinkti šias parinktis.

| Parinktis        | aprašymas   | 
| ------------- | ------------- |
| Vienetų paėmimo patvirtinimas   | Pasiekiama paėmimo ir skaičiavimo darbo tipų atveju. Automatiškai pasirenkamas produkto patvirtinimas. Suteikia galimybę mobiliuoju įrenginiu patvirtinti kiekvieną atsargų vienetą. | 
| Maksimalus vienetų skaičius     | Pasiekiama paėmimo darbo atveju, jei įgalintas vienetų paėmimo patvirtinimas. Nustato vienetų, kuriuos turite patvirtinti, skaičiaus apribojimus. |  

