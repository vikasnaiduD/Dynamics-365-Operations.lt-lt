---
title: "Finansinės veiklos „Power BI“ turinys"
description: "Šioje temoje aprašomas „Power BI‟ turinys Finansinės veiklos rezultatai."
author: kweekley
manager: AnnBe
ms.date: 02/02/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.custom: 106233
ms.assetid: 517e6a88-e7a1-4398-9971-b22fa83306ba
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: b167d7577823bbc88d8e64952333110f9a652b64
ms.openlocfilehash: 53d0654608e99aa85a5911d76397fbc7fadbf26e
ms.contentlocale: lt-lt
ms.lasthandoff: 02/02/2018

---

# <a name="financial-performance-power-bi-content"></a>Finansinės veiklos „Power BI“ turinys

[!include[banner](../includes/banner.md)]

> [Pastaba] Šis turinio paketas nebenaudojamas, kaip nurodyta dalyje [Svetainėje PowerBI.com publikuojami „Power BI“ turinio paketai](https://docs.microsoft.com/en-us/dynamics365/unified-operations/dev-itpro/migration-upgrade/deprecated-features#power-bi-content-packs-published-to-powerbicom).

Šioje temoje aprašomas „Microsoft Power BI‟ turinys **Finansinės veiklos rezultatai**. Joje aprašoma ataskaitų sritis ir į turinį įtrauktos ataskaitos ir pateikiama informacija apie duomenų modelį ir objektus, naudotus turiniui kurti.

## <a name="main-account-setup"></a>Pagrindinių sąskaitų sąranka
Kadangi organizacijos nori, jog įsipareigojimai ir įplaukų sumos ataskaitose būtų rodomos kaip teigiamos sumos, svarbu nustatyti pagrindines sąskaitas. Tam, kad šios pagrindinės sąskaitos būtų rodomos kaip teigiamos sumos, turi būti nustatytas pagrindinės sąskaitos tipas **Įsipareigojimas** arba **Įplaukos**. Kai naudojami šie sąskaitų tipai, ataskaitas teikiant per „Power BI“ ženklai pakeičiami ir rodomos teigiamos sumos.

## <a name="dashboard-and-reports-that-are-included-in-the-power-bi-content"></a>Į „Power BI‟ turinio paketą įtrauktos ataskaitų sritys ir ataskaitos
Ataskaitų srityje pateikiamos apibendrintos esamomis ataskaitomis pagrįstų duomenų plytelės. Kiekvienoje plytelėje pateikiama apibendrinta šių metų informacija apie visas įmones organizacijoje. Toliau pateikiamos kai kurios plytelės.

- Grynieji pinigai
- Visos įplaukos šiais metais
- Visos išlaidos šiais metais
- Grynosios pajamos šiais metais
- Spartusis koeficientas
- Bendrosios išlaidos šiais metais pagal sąskaitos kategoriją
- Dabartinis koeficientas
- Skola, palyginus su visu turtu
- Faktinės ir prognozuojamos įplaukos
- Šių metų įplaukos, kurioms išrašyta sąskaita
- Veiklos išlaidų koeficientas šiais metais
- Pelno marža šiais metais
- Faktinės ir biudžeto išlaidos – visos įmonės

Kiekviena plytelė yra pagrindžiama papildoma ataskaita. Šiose ataskaitose yra diagramos ir lentelės, kurios teikia daugiau informacijos. Tolesnėje lentelėje aprašomos ataskaitos.

| Ataskaita                      | Ataskaitoje pateikiama informacija |
|-----------------------------|--------------------------------------|
| Grynųjų pinigų analizė               | Grynieji pinigai pagal juridinį subjektą, grynieji pinigai pagal ketvirtį, visa grynųjų pinigų suma ir grynieji pinigai pagal sąskaitą<blockquote>[!NOTE]<br>Grynųjų pinigų ketvirčio informacija neapima pradžios likučių bendrosios sumos pirmajam ketvirčiui. Joje rodoma naujų operacijų, užregistruotų kiekvieną ketvirtį, bendra suma.</blockquote> |
| Dabartinio koeficiento analizė      | Dabartinis koeficientas pagal juridinį subjektą, dabartinis koeficientas pagal ketvirtį ir trumpalaikio turto bei trumpalaikių įsipareigojimų balansai |
| Sparčiojo koeficiento analizė        | Spartusis koeficientas pagal juridinį subjektą, spartusis koeficientas pagal ketvirtį ir grynųjų pinigų, gautinų sumų bei trumpalaikių įsipareigojimų balansai |
| Parduotų prekių savikainos analizė | Parduotų prekių savikaina (PPK) pagal juridinį subjektą, PPK šiais metais ir praėjusiais metais pagal ketvirtį, PPK ir pardavimas pagal juridinį subjektą, bendroji PPK bei PPK ir pardavimo procentas |
| Apyvartinio kapitalo analizė    | Apyvartinis kapitalas pagal juridinį subjektą, apyvartinis kapitalas pagal ketvirtį, trumpalaikis turtas, trumpalaikiai įsipareigojimai ir visas apyvartinis kapitalas |
| Turto ir skolos analizė     | Bendro turto grąža ir skola, palyginti su bendru turtu, pagal juridinį subjektą, skola, palyginti su bendru turtu, ir bendro turto grąža ketvirtį iki dienos, turtas ir įsipareigojimai |
| Pelno maržos analizė      | Faktinė ir biudžeto pelno marža pagal juridinį subjektą, pelno žymėjimas pagal ketvirtį, pelno maržos procentas ir pelno marža |
| Grynųjų pinigų analizė         | Faktinės ir biudžeto grynosios pajamos pagal juridinį subjektą, grynosios pajamos šiais metais ir praėjusiais metais bei išlaidos ir grynųjų pinigų procentas |
| Pajamų analizė           | Faktinės ir biudžeto pajamos prieš palūkanas ir mokesčius (EBIT) pagal juridinį subjektą, EBIT šiais metais ir praėjusiais metais, išlaidos ir įplaukų procentas, faktinės bei biudžeto išlaidos ir įplaukos |
| Įplaukų analizė            | Bendrosios įplaukos, faktinės ir biudžeto bendrosios įplaukos pagal juridinį subjektą, bendrosios įplaukos šiais metais ir praėjusiais metais, įplaukų biudžeto nuokrypis pagal juridinį subjektą ir bendrosios įplaukos šį laikotarpį ir paskutinįjį laikotarpį |
| Išlaidų analizė            | Bendrosios išlaidos, faktinės ir biudžeto bendrosios išlaidos pagal juridinį subjektą, faktinės ir biudžeto bendrosios išlaidos pagal ketvirtį, bendrosios išlaidos pagal sąskaitos kategoriją ir veiklos išlaidų koeficientas |
| Įplaukų, kurioms išrašyta sąskaita, analizė     | Bendrosios gautinos sumos, bendrosios gautinos sumos pagal juridinį subjektą, bendrosios gautinos sumos pagal ketvirtį ir gautinų sumų sąskaitų balansai<blockquote>[!NOTE]<br>Informacija neapima gautinų sumų DK sąskaitų pradžios likučių. Joje rodoma naujų operacijų, užregistruotų gautinose sumose, bendra suma.</blockquote> |

Šių ataskaitų diagramas ir plyteles galima filtruoti ir prisegti prie ataskaitų srities. Daugiau informacijos apie tai, kaip „Power BI“ filtruoti ir prisegti, žr. [Ataskaitų srities kūrimas ir konfigūravimas](https://powerbi.microsoft.com/en-us/guided-learning/powerbi-learning-4-2-create-configure-dashboards).

## <a name="understanding-the-data-model-and-entities"></a>Duomenų modelio ir objektų supratimas
Toliau pateikti objektai buvo naudojami kaip „Power BI‟ turinio **Finansinės veiklos rezultatai** pagrindas.

**Duomenų objektų sujungimas**

- **GeneralLedgerActivities** – šis įrašas sujungia DK balansus pagal sąskaitos kategoriją.
- **BudgetActivities** – šis įrašas sujungia biudžeto balansus pagal sąskaitos kategoriją.

**Duomenų objektai**

- FiscalCalendars
- MainAccounts
- LegalEntities
- Didžiosios knygos
- ChartofAccounts

Šie objektai buvo naudojami skaičiuojamiems matams duomenų modelyje sukurti. Skaičiuojami matai naudojami skaičiuojant pagrindinius efektyvumo indikatorius (KPI) ir ataskaitas, naudojamas turinyje. Pagal numatytuosius parametrus turinyje pastarųjų trejų metų duomenys sutelkti į vienerius būsimus metus. Norėdami ataskaitas ir ataskaitų sritį įtraukti papildomų skaičiavimų, galite modifikuoti [„Microsoft Excel“ darbaknygę](https://mbs.microsoft.com/customersource/global/AX/downloads/reports/msdaxfinpercontentpowerbi). Ši darbaknygė yra numatytasis duomenų modelis, kuris buvo naudojamas turiniui kurti. 

