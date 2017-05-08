---
title: Padengimo parametrai
description: "Bendrasis planavimas naudoja padengimo parametrus prekės poreikiui apskaičiuoti."
author: YuyuScheller
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ReqGroup, ReqItemTable, ReqItemTableWizard
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 2494
ms.assetid: 5a95ae4f-ca75-47d9-a1c3-68c97b42f166
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 9ccbe5815ebb54e00265e130be9c82491aebabce
ms.openlocfilehash: c1c5654afa6b592e178af052e3e4a7e246a94c9f
ms.lasthandoff: 03/31/2017


---

# <a name="coverage-settings"></a>Padengimo parametrai

[!include[banner](../includes/banner.md)]


Bendrasis planavimas naudoja padengimo parametrus prekės poreikiui apskaičiuoti. 

Galite nurodyti padengimo parametrus keliais būdais:

-   Nurodykite padengimo grupės padengimo parametrus. Galite sukurti padengimo grupę, kurioje būtų visų su padengimo grupe susijusių produktų parametrai. Norėdami sukurti padengimo grupę spustelėkite **Bendrasis planavimas &gt; Sąranka &gt; Padengimas &gt; Padengimo grupės**. Padengimo grupę galite susieti su produktu. Jei saitas yra konkrečios teritorijos, sandėlio ar produkto dimensijos, naudokite puslapio **Prekės padengimas** lauką **Padengimo grupė**. Jei saitas yra bendrasis, neatsižvelgdami į produkto dimensijas, naudokite puslapio **Produkto informacija** „FastTab“ skirtuke **Planas** esančią parinktį **Padengimo grupė**. Jei padengimo grupės nesusiejate su produktu, bendrojo planavimo funkcija kaip numatytąją naudoja puslapyje **Bendrojo planavimo parametrai** nurodytą parinktį **Bendroji padengimo grupė**.

-   Nurodykite produkto padengimo parametrus. Galite sukurti konkretaus produkto padengimo parametrus. Spustelėkite **Produkto informacijos valdymas &gt; Produktai &gt; Išleisti produktai**. Pasirinkite produktą, dalyje **Veiksmų sritis** esančio skirtuko **Planas** lauke **Padengimo grupė** spustelėkite **Prekės padengimas**, kad būtų atidarytas puslapis **Prekės padengimas**. Jei produktas jau susietas su padengimo grupe, galite nepaisyti padengimo grupės parametrų, naudodami lauką **Nepaisyti**. Padengimo parametrams puslapyje** Prekės padengimas** teikiama pirmenybė prieš parametrus puslapyje **Padengimo grupė**.

<!-- -->

-   Nurodykite produkto padengimo parametrus naudodami vedlį. Vedlys yra išsamus instruktorius, padedantis nustatyti pirminius prekės padengimo parametrus. Puslapyje **Prekės padengimas** spustelėkite **Vedlys**, kad būtų atidarytas **Prekės padengimo vedlys**.

<!-- -->

-   Nurodykite dimensijos grupės padengimo parametrus. Spustelėkite **Produkto informacijos valdymas &gt; Bendra &gt; Patvirtinti produktai**. Puslapio **Patvirtinto produkto informacija** skirtuke **Bendra** esančioje grupėje **Administravimas** spustelėkite saitą **Saugojimo dimensijų grupė**. Puslapyje **Saugojimo dimensijų grupė** pasirinkite lauką **Padengimo planas dimensijomis**, kad sukurtumėte saugojimo dimensijų grupės dimensijos padengimo nustatymus. Visose produkto dimensijose, pvz., konfigūracijos, spalvos, dydžio, stiliaus, turi būti pasirinktas laukas **Padengimo planas pagal dimensiją**.



<a name="see-also"></a>Taip pat žiūrėkite
--------

[Bendrieji planai](master-plans.md)



