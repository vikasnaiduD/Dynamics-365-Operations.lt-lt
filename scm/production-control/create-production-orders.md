---
title: "Kurti gamybos užsakymus"
description: "Kai gamybos užsakymas sukurtas, inicijuojamas prašymas pradėti gaminti prekę. Gamybos užsakyme yra informacijos apie tai, kas bus gaminama, norimas gaminti kiekis ir kokia yra numatyta baigimo data. Taip pat pateikiama informacija apie tai, kurios medžiagos naudojamos ir kurio proceso laikytis gaminant prekę."
author: YuyuScheller
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ProdTable, ProdTableCreate
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 19741
ms.assetid: bbb6e69d-479c-45fc-a0a8-66da5df16c7f
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: johanho
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 9ccbe5815ebb54e00265e130be9c82491aebabce
ms.openlocfilehash: 33d2e4f1a6bc8bc28e43b4c985d9a780a9481e97
ms.lasthandoff: 03/31/2017


---

# <a name="create-production-orders"></a>Kurti gamybos užsakymus

[!include[banner](../includes/banner.md)]


Kai gamybos užsakymas sukurtas, inicijuojamas prašymas pradėti gaminti prekę. Gamybos užsakyme yra informacijos apie tai, kas bus gaminama, norimas gaminti kiekis ir kokia yra numatyta baigimo data. Taip pat pateikiama informacija apie tai, kurios medžiagos naudojamos ir kurio proceso laikytis gaminant prekę.

Gamybos užsakymas pereina gamybos ciklo etapus. Kai užsakymas sukurtas, jam priskiriama būsena **Sukurtas**. Kai užsakymas baigtas, jam priskiriama būsena **Baigtas**. Parametro nuostata kiekviename etape leidžia naudotojui konfigūruoti kiekvieną veiksmą. Nuostatą galima nustatyti vienam naudotojui arba visiems naudotojams.

Gamybos komplektavimo specifikacija ir gamybos maršrutas yra pagrindiniai gamybos užsakymo objektai. Jie į gamybos užsakymą kopijuojami pagal pasirinktą prekę ir kiekį, kurį ketinama gaminti. Prieš pradedant gamybos užsakymą, galima redaguoti gamybos komplektavimo specifikaciją ir maršrutą.

Gamybos užsakymą galima kurti pagal toliau pateiktus scenarijus.

-   Sukurtas vykdant bendrąjį planavimą pagal medžiagų poreikį.
-   Sukurtas tiesiai iš pardavimo užsakymo eilutės arba sukūrus ir įvertinus aukštesnio lygio gamybos užsakymą (iškviestas tiekimas).
-   Sukurtas rankiniu būdu.




