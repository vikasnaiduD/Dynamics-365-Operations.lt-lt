---
title: "KS versijos išskleidimas"
description: "Šiame straipsnyje paaiškinamas bendrojo planavimo scenarijus, apimantis KS versijos išskleidimą."
author: roxanadiaconu
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: ReqTransExplosion
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, Operations
ms.custom: 19211
ms.assetid: fe08c2e6-9cc5-4e34-bbb2-cd07843403b5
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 0f852c8d100c91d055e58c4594106aedf6fe5afb
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="explosion-of-a-bom-version"></a>KS versijos išskleidimas

[!include[banner](../includes/banner.md)]


Šiame straipsnyje paaiškinamas bendrojo planavimo scenarijus, apimantis KS versijos išskleidimą.

Komplektavimo specifikacijos (KS) versijos poreikio išskleidimas sukuria kiekvienos KS eilutės poreikį tam tikroje teritorijoje ir, galbūt, tam tikrame sandėlyje. Teritorijai būdingoje KS galima nustatyti konkretų kiekvienos KS eilutės sandėlį. Taip pat kiekvienos KS eilutės prekės dimensijos parametrai nurodo, ar sandėlis būtinas. Gautas kiekvienos KS eilutės prekės poreikis savo ruožtu tampa papildomo poreikio išskleidimo pradžios tašku. Į šį bendrojo planavimo scenarijų įeina toliau nurodytos sąlygos.

-   Teritorijos dimensija yra privaloma ir turi būti įvesta poreikio operacijoje.
-   Teritorijos dimensija yra nuosekli. Todėl teritorija žemesnio lygio poreikiui yra ta pati, kaip pradinio poreikio operacijos teritorija.

Tolesniame paveikslėlyje parodyta, kaip vyksta bendrojo planavimo poreikio išskleidimas. ![Poreikio išplėtimas naudojantis KS versija](./media/multisitedemandexplosionscenariousingbomversion.gif)

<a name="see-also"></a>Taip pat žiūrėkite
--------

[Bendrasis planavimas – kaip nustatoma KS versija](master-plan-bom-version-determined.md)

[Bendrasis planavimas ir kelių teritorijų funkcija](master-plan-multisite-functionality.md)




