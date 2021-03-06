---
title: "Įtraukti faktinę vertę"
description: "Puslapio Prekių modelių grupės „FastTab‟ skirtuko Atsargų modelis žymės langelis Įtraukti faktinę vertę naudojamas nurodyti, ar, skaičiuojant prekės einamąją vidutinę savikainą, atsižvelgiama į faktiškai atnaujintas operacijas."
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: InventModelGroup
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, Operations
ms.custom: 79033
ms.assetid: 1928c145-bf82-436d-87ca-e7a173e31923
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: mguada
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 4ea8fe31588dd0768e0651c9e1e332212a00cde2
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="include-physical-value"></a>Įtraukti faktinę vertę

[!include[banner](../includes/banner.md)]


Puslapio Prekių modelių grupės „FastTab‟ skirtuko Atsargų modelis žymės langelis Įtraukti faktinę vertę naudojamas nurodyti, ar, skaičiuojant prekės einamąją vidutinę savikainą, atsižvelgiama į faktiškai atnaujintas operacijas.

Žymės langelyje **Įtraukti faktinę vertę** yra tolesnės reikšmės.

| Vertė    | Rezultatas                                                                                                                          |
|----------|---------------------------------------------------------------------------------------------------------------------------------|
| Pasirinkta | Savikainai apskaičiuoti naudojamos tiek fiziškai, tiek finansiškai atnaujintos operacijos. |
| Apmokėta  | Skaičiuoti einamajai vidutinei savikainai naudojamos tik finansiškai atnaujintos operacijos.                                     |

Žymės langelio poveikis šiek tiek skiriasi – jis priklauso nuo jūsų naudojamo atsargų modelio.

-   Jei, naudodami atsargų modelį FIFO (pirmiausiai gaunama, pirmiausiai išduodama), LIFO (vėliausiai gaunama, pirmiausiai išduodama) arba LIFO data, pasirenkate žymės langelį **Įtraukti faktinę vertę**, uždarant atsargas taip pat pakoreguojamos faktiškai atnaujintos operacijos.
-   Jei, naudodami šiuos atsargų modelius, žymės langelio **Įtraukti faktinę vertę** nepasirenkante, uždarant atsargas sudengiamos tik finansiškai atnaujintos operacijos.
-   Kai naudojate svertinį vidurkį arba svertinio vidurkio datos atsargų modelį, atsargų uždarymas sudengia tik finansiškai atnaujintas operacijas, nesvarbu, ar pažymėjote žymės langelį **Įtraukti fizinę vertę**.

**1 pavyzdys** Pažymėjote žymės langelį **Įtraukti faktinę vertę** ir gaunate tolesnius pirkimo užsakymus.

-   Pirkimo užsakymą, kurio kiekis – 2, o savikaina – 10,00 USD, kurio važtaraštis atnaujintas.
-   Pirkimo užsakymą, kurio kiekis – 3, o savikaina – 12,00 USD, kurio sąskaita faktūra atnaujinta.

Šiuo atveju einamoji vidutinė savikaina bus 11,20 USD, nes tiek fiziškai, tiek finansiškai atnaujintos operacijos naudojamos savikainai apskaičiuoti. **2 pavyzdys** Žymės langelio **Įtraukti faktinę vertę** nepažymėjote ir, nustatant prekes, savikaina yra 10,00 USD. Gaunate pirkimo užsakymą, kurio kiekis – 20, o savikaina – 12,00 USD, kurio važtaraštis atnaujintas. Kai pardavimo užsakymas užregistruojamas, užregistruotoji savikaina yra 10,00 USD, nes į einamąją vidutinę savikainą neįtrauktos faktiškai užregistruotos operacijos. **Pastaba.** Palyginimui, jei šios prekės žymės langelį **Įtraukti faktinę vertę** pažymėsite, kai registruojamas pardavimo užsakymas, užregistruotoji savikaina bus 12,00 USD.




