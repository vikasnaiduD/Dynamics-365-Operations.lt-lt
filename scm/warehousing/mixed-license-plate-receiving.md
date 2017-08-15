---
title: "Mišrių numerio lentelių gavimas"
description: "Šioje temoje aprašoma, kaip naudoti mišrių numerio lentelių gavimą, norint užregistruoti ir sukurti kelių prekių darbą su mobiliuoju įrenginiu."
author: Mirzaab
manager: AnnBe
ms.date: 05/26/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 269384
ms.search.region: Global
ms.author: mirzaab
ms.search.validFrom: 2016-02-28T00:00:00.000Z
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 08c38aada355583c5a6872f75b57db95d9b81786
ms.openlocfilehash: 0e785d71e7ae3c5f60d36d8b190001b5e356c626
ms.contentlocale: lt-lt
ms.lasthandoff: 07/27/2017

---

# <a name="mixed-license-plate-receiving"></a>Mišrių numerio lentelių gavimas

[!include[banner](../includes/banner.md)]

Mišrių numerio lentelių gavimas leidžia sukurti numerio lentelę, sudarytą iš kelių prekių, prieš registruojant ir kuriant atidėjimo darbą. 

Numerio lentelė, sudaryta iš kelių prekių, gavimo rampoje neturi būti padalyta tam, kad užregistruotumėte kiekvieną prekę. 

Naudodami su preke susijusį srautą, kad nustatytumėte šaltinio dokumento eilutes, galite nuskaityti brūkšninius kodus prekės valdiklyje. Jei brūkšniniame kode sukonfigūruoti kiekis ir matavimo vienetas (MV), prekė ir kiekis bus automatiškai pridėti į mišrią numerio lentelę, ir jūs būsite grąžinti į ekraną, skirtą nuskaityti kitą prekę. Tai leidžia greitai nuskaityti visas prekes neatliekant patvirtinimo kiekviename veiksme. 

Mišrios numerio lentelės gavimo sraute gali būti rodomas į mišrią numerio lentelę jau nuskaitytų prekių sąrašas, čia galite modifikuoti arba koreguoti prekės kiekį.

## <a name="where-it-applies"></a>Kai taikoma

Mišrios numerio lentelės gavimas yra mobiliojo įrenginio gavimo srautas, skirtas užregistruoti ir sukurti kelių eilučių / prekių darbą tuo pačiu metu. Tai naudinga, jei gaunate gavimo numerio lenteles su keliomis prekėmis. 

## <a name="how-to-set-up-mixed-license-plate-receiving"></a>Kaip nustatyti mišrių numerio lentelių gavimą
Mišrių numerio lentelių gavimas nustatomas kaip mobiliojo įrenginio meniu elementas.

Turite sukurti naują meniu elementą režimu Darbas, kuriame nenaudojamas esamas darbas, ir naudojamas vienas iš nurodytų metodų.

- Mišrių numerio lentelių gavimas
- Mišrių numerio lentelių gavimas ir padėjimas

Parinktys, skirtos identifikuoti šaltinio dokumento eilutes, yra pirkimo užsakymo prekė, pirkimo užsakymo eilutė, grąžinimo užsakymas, perkėlimo užsakymo prekė ir perkėlimo užsakymo eilutė. Šios parinktys gali pakeisti gavimo užsakymą vienoje numerio lentelėje. Paskutinė parinktis yra pagal krovinio prekę. Į numerio lentelę galite pridėti kelias prekes, tačiau negalite keisti vieno krovinio į kitą.
