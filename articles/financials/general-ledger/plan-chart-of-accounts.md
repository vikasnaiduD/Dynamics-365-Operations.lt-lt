---
title: "Savo sąskaitų plano sudarymas"
description: "Šiame straipsnyje pateikta informacija, kuri padės jums suplanuoti jūsų organizacijos sąskaitų planą."
author: aprilolson
manager: AnnBe
ms.date: 01/04/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: DimensionConfigureAccountStructure, LedgerChartOfAccounts
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.custom: 14051
ms.assetid: 10edb129-33f0-4cf9-b2a7-4b7ffa09b229
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: ad55dd57483de4351c8501c5e226180fc73606aa
ms.openlocfilehash: 3d2cdeaf2fdeb2f587f82c97249886fb8db49154
ms.contentlocale: lt-lt
ms.lasthandoff: 01/11/2018

---

# <a name="plan-your-chart-of-accounts"></a>Savo sąskaitų plano sudarymas

[!include[banner](../includes/banner.md)]


Šiame straipsnyje pateikta informacija, kuri padės jums suplanuoti jūsų organizacijos sąskaitų planą.

Norėdami sekti ir prižiūrėti finansinę informaciją organizacijoje, galite nustatyti sąskaitų planą. Sąskaitų planas yra sąskaitų rinkinys, kuris apibrėžia finansinę sistemą. Norėdami toliau sekti šių sąskaitų operacijas, galite pridėti segmentus, kurie žinomi kaip finansinės dimensijos. Pavyzdžiui, išlaidų sąskaita gali apimti finansines dimensijas, pavadintas „Padalinys“, „Išlaidų centras“ ir „Paskirtis“. Vartotojo nustatytos taisyklės, žinomos kaip sąskaitos struktūros ir išplėstinės taisyklės, nurodo, kaip šios finansinės dimensijos yra susietos su pagrindinėmis sąskaitomis ir kitomis finansinėmis dimensijomis ir kaip įvedamos operacijos. 

Sąskaitų planas yra susistemintas juridinio subjekto DK sąskaitų sąrašas. Sąrašas naudojamas norint parengti finansines ataskaitas institucijoms ir savininkams. Sąskaitos grupuojamos į sąskaitų tipus, o toliau sujungiamos į didesnes kategorijas. Žvelgiant bendrai, sąskaitos grupuojamos kaip įplaukos ir išlaidos (operacijų sąskaitos) bei turtas ir įsipareigojimai (balanso sąskaitos). 

Sąskaitų planu galima dalintis ir juo naudotis gali bet kuris juridinis subjektas organizacijoje. Sąskaitų planas, kurį naudoja juridinis subjektas, nurodomas puslapyje **Didžioji knyga**. 

Toliau pateikiami kai kurie veiksniai, į kuriuos privalote atsižvelgti, kai planuojate savo organizacijos sąskaitų plano struktūrą:

-   Ataskaitų kūrimo reikalavimai šalyje / regione, kuriame yra jūsų organizacija.
-   Jūsų juridinio subjekto ataskaitų kūrimo reikalavimai
-   Išorinėms organizacijoms ir jūsų organizacijai reikalingas specifikacijų laipsnis

Sukurkite sąskaitų planą puslapyje **Sąskaitų planas**. Pagrindines sąskaitas galima sukurti puslapyje **Sąskaitų planas** arba puslapyje **Pagrindinės sąskaitos**. Pagrindinėse sąskaitose nereikėtų naudoti jokių specialių simbolių, kurie naudojami kaip sąskaitų plano skyrikliai. Jei turite specialų simbolį, kurs yra toks pats, kaip ir jūsų sąskaitų plano skyriklis, gali kilti nestabilumų arba poreikis visada naudoti peržvalgas arba iškeliamąjį objektą, įvedant sąskaitos ir dimensijų kombinacijas. Daugiau informacijos žr. [Kurti pagrindinę sąskaitą](tasks/create-main-account.md).


Tikslinga susieti pagrindines sąskaitas su pagrindinių sąskaitų kategorijomis, kad galėtumėte išnaudoti numatytąsias finansines ataskaitas nedarydami jokių modifikacijų. Todėl jūs galite greičiau ir lengviau kurti ir prižiūrėti ataskaitas. 

Naudokite puslapį **Konfigūruoti sąskaitų struktūras**, kad sukurtumėte sąskaitų struktūras. Sąskaitų struktūros apibrėžia galiojančias kombinacijas. Kombinacijos, kartu su pagrindinėmis sąskaitomis, formuoja sąskaitų planą.  Daugiau informacijos žr. [Kurti sąskaitos struktūrą](tasks/create-account-structures.md).

**Juridinio subjekto nepaisymai** 

Ne visos pagrindinės sąskaitos tinkamos visiems juridiniams subjektams, o kai kurios gali būti aktualios tik tam tikrą laikotarpį. Tokiu atveju skyrius „Juridinio subjekto nepaisymas“ gali būti naudojamas nustatyti, kurių įmonių pagrindinė sąskaita turi būti sustabdyta, kas jų savininkas ir kiek laiko dimensija yra aktyvi. Nepaisymai bendrame lygyje negali būti labiau ribojantys nei nepaisymai juridinio subjekto lygyje.

Daugiau informacijos žr. temose: [Finansinės dimensijos](financial-dimensions.md)
[Kurti ir priskirti išplėstinės taisyklės struktūras](tasks/create-assign-advanced-rule-structures.md)




