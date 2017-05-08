---
title: "Produktų dimensijos"
description: "Produktų dimensijos yra keturios – Spalva, Konfigūracija, Dydis ir Stilius. Produktų dimensijos jungiamos į dimensijų grupes, o dimensijų grupės priskiriamos bendriesiems produktams. Produktų dimensijų kombinacijomis nustatoma, kaip apibrėžiami produktų variantai."
author: YuyuScheller
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: EcoResProductDimension, EcoResProductDimensionGroup, EcoResProductMasterDimension, RetailEcoResColor, RetailEcoResSize, RetailEcoResStyle
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 19171
ms.assetid: 81fa3709-4ab8-4fbf-9806-359892a05985
ms.search.region: Global
ms.search.industry: Retail
ms.author: yuyus
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 9ccbe5815ebb54e00265e130be9c82491aebabce
ms.openlocfilehash: 8854ab94a71cc363bcd073d2df47bc01a243b6cd
ms.lasthandoff: 03/31/2017


---

# <a name="product-dimensions"></a>Produktų dimensijos

[!include[banner](../includes/banner.md)]


Produktų dimensijos yra keturios – Spalva, Konfigūracija, Dydis ir Stilius. Produktų dimensijos jungiamos į dimensijų grupes, o dimensijų grupės priskiriamos bendriesiems produktams. Produktų dimensijų kombinacijomis nustatoma, kaip apibrėžiami produktų variantai.

Produkto dimensijos – tai charakteristikos, naudojamos produkto variantui nustatyti. Galite naudoti produkto dimensijų derinius produkto variantams nustatyti. Norėdami sukurti produkto variantą, turite nustatyti bent vieną bendrojo produkto dimensiją.
Produkto variantai
----------------

Produkto variantai taip pat vadinami prekėmis. Prekė – tai materialus produktas, kuris nėra apibūdinamas visiškai taip pat, kaip paslauga. Taip pat galima nustatyti bendrąjį produktą naudojant tipą Paslauga. Naudodami tipą Paslauga, galite nurodyti produkto variantus, kuriuose yra paslaugų. Pavyzdžiui, galite nurodyti konsultacinio darbo bendrąjį produktą bei vyresniųjų ir jaunesniųjų konsultantų atliekamo darbo produkto variantus.

## <a name="product-dimensions"></a>Produktų dimensijos
Galimos šios produktų dimensijos: Konfigūracija, Spalva, Dydis ir Stilius. Produkto variantas gali būti kuriamas pagal produkto dimensijų reikšmes.

Produkto dimensijų vertes, pvz., Dydis, Spalva ir Stilius, galima sukurti puslapiuose **Dydis**, **Spalva** ir **Stilius**, kuriuos galima pasiekti iš šių vietų: **Produkto informacijos valdymas** &gt; **Sąranka** &gt; **Dimensijų ir variantų grupės** &gt; **Dydžiai / Spalvos / Stiliai**. Konfigūracijos dimensijos produkto dimensijų vertės paprastai kuriamos naudojant produkto konfigūratorių arba dimensijomis pagrįstą konfigūratorių. Produkto dimensijos taip pat gali būti kuriamos ir tvarkomos puslapyje **Produktų dimensijos**, kurį galima pasiekti šiose vietose:
-   Spustelėkite **Produkto informacijos valdymas** &gt; **Produktai** &gt; **Bendrieji produktai**. Dalyje **Veiksmų sritis** spustelėkite **Produktų dimensijos**.
-   Spustelėkite **Produkto informacijos valdymas** &gt; **Produktai** &gt; **Visi produktai ir bendrieji produktai**. Pasirinkite bendrąjį produktą. Dalyje **Veiksmų sritis** spustelėkite **Produktų dimensijos**.
-   Spustelėkite **Produkto informacijos valdymas** &gt; **Patvirtinti produktai**. Pasirinkite bendrąjį produktą. Dalyje **Veiksmų sritis** spustelėkite **Produktas**. Grupėje **Bendrasis produktas** spustelėkite **Produktų dimensijos**.

Variantų, kuriuos galite sukurti prekei, kiekis ribojamas pagal galimų produkto dimensijų derinių kiekį.
| **Patarimas **                                                                                                                                              |
|------------------------------------------------------------------------------------------------------------------------------------------------------|
| Pavyzdžiui, užsakymo eilutėje naudodami produktą, pasirinkę produkto dimensijas identifikuosite norimą naudoti produkto variantą. |

## <a name="example"></a>Pavyzdys
Įmonė parduoda džinsus. Prekei (džinsams) apibūdinti naudojamos produktų dimensijos Spalva ir Dydis. Parduodami trijų skirtingų spalvų ir šešių skirtingų dydžių džinsai. Spalvos: mėlyna, juoda, ruda Dydžiai: XS, S, M, L, XL, XXL Ne visi dydžiai galimi visų trijų spalvų. Jei būtų galimi visi deriniai, būtų sukurta 18 skirtingų tipų džinsų. Šiame pavyzdyje sukurti tik šie devyni produkto variantų deriniai.

| Spalva | Dydis |
|-------|------|
| Mėlyna  | XS   |
| Mėlyna  | Š.    |
| Mėlyna  | P    |
| Juoda | P    |
| Juoda | L    |
| Juoda | XL   |
| Ruda | L    |
| Ruda | XL   |
| Ruda | XXL  |





