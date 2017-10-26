---
title: "Darbo jėgos metrikos „Power BI“ turinys"
description: "Šioje temoje aprašomas darbo jėgos metrikos „Power BI‟ turinys. Jame paaiškinta, kaip pasiekti ataskaitas, ir pateikta informacija apie duomenų modelį ir objektus, naudojamus turinio paketui kurti."
author: jcart1106
manager: AnnBe
ms.date: 06/16/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Operations, UnifiedOperations, Talent, Core
ms.custom: 264084
ms.assetid: 8e700583-3a7d-4f5f-9ac8-58c4feed1a02
ms.search.region: Global
ms.author: jcart
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: a5b680b406f9be3e80b43259993a3e441391ec60
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---

# <a name="workforce-metrics-power-bi-content"></a>Darbo jėgos metrikos „Power BI“ turinys

[!include[banner](../includes/banner.md)]

Šioje temoje aprašomas **Darbo jėgos metrikos** „Microsoft Power BI‟ turinys. Jame paaiškinta, kaip pasiekti „Power BI“ ataskaitas, ir pateikta informacija apie duomenų modelį ir objektus, naudojamus turinio paketui kurti.

## <a name="accessing-the-power-bi-content"></a>Prieiga prie „Power BI“ turinio
**Darbo jėgos metrikos** „Power BI“ turinys pasirodo **Personalo valdymo** darbo srityje, jei naudojate vieną iš šių produktų:

- „Microsoft Dynamics 365 for Finance and Operations, Enterprise edition“ (2017 m. liepos mėn.)
- „Microsoft Dynamics 365 for Talent“

## <a name="metrics-that-are-included-in-the-power-bi-content"></a>Į „Power BI“ turinį įtrauktos metrikos
Šioje lentelėje išvardijamos metrikos, kurios bus rodomos kiekvienoje ataskaitoje.

| Ataskaita                                           | Metrika                                                                                                                                                                                                            |
|--------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Žmonių metrika                                   | Kitų ataskaitų suvestinė                                                                                                                           |
| Įmonės, padalinio, vietos darbuotojų skaičiaus analizė | Darbuotojų skaičius pagal įmonę, padalinį, vietą ir bendras darbuotojų skaičius                                                                                                                           |
| Užduotis atliekančių, veiksmą vykdančių, vadovams priskirtų darbuotojų skaičiaus analizė            | Darbuotojų skaičius pagal užduotį, veiksmą, vadovą ir bendras darbuotojų skaičius                                                                                                                                      |
| Darbuotojų skaičiaus tendencijų analizė                         | Darbuotojų skaičius šiais metais palyginus su praėjusiais pagal įmonę ir darbuotojų skaičiaus pokytis per pastaruosius 12 mėnesių                                                                                                                        |
| FTE analizė                                     | Bendras viso etato atitikmuo (FTE), bendras priskirtas FTE, FTE pagal padalinį, FTE per pastaruosius 12 mėnesių ir FTE pagal užduotį |
| Darbo jėgos demografiniai rodikliai                           | Darbuotojų skaičius pagal amžių, lytį, etninę kilmę, šeimyninę padėtį, seniai dirbančiųjų skaičius, visu etatu dirbančių studentų skaičius, vidutinis pareigų ėjimo laikas, vidutinis amžius, darbuotojų moterų bei vyrų santykis ir darbuotojų vartojamos kalbos |
| Pareigų analizė                                | Atviros pareigos pagal padalinį, laisvos / užimtos pareigos, aktyvios / neaktyvios pareigos ir pareigos pagal padalinį                                                                                                   |
| Praradimo analizė                               | Skaičiaus sumažėjimas šiais metais, palyginti su praėjusiais metais, skaičiaus sumažėjimas, išeinantys darbuotojai pagal amžių ir lytį, vidutinis išeinančių darbuotojų tarnybos laikas, šį mėnesį išeinantys darbuotojai, darbuotojų išėjimo priežastis                                                                   |
| Žmonės pagal padalinį                             | Darbuotojai pagal padalinio, pareigų darbuotojo numerį ir priskyrimo pradžios bei pabaigos datas                                                                                                                       |
| Paaukštinimo analizė                               | Vidutinis tarnybos laikas, vidutiniai tarnybos metai pagal įmonę ir darbo stažo sąrašas                                                                                                                                                              |
| Darbuotojų metinės                           | Metinės šį mėnesį, metinės kitą mėnesį, darbuotojai pagal tarnybos metus, tarnybos metai pagal padalinį                                                                                                                                                                    |
| Darbuotojų gimtadieniai                               | Gimtadieniai šį mėnesį, gimtadieniai kitą mėnesį, darbuotojų gimtadieniai ir gimtadieniai pagal mėnesį ir padalinį                                                                                                                                                                    |
| Masinės samdos projektai                               | Bendri masinės samdos projektai, masinės samdos projektai pagal būseną, masinės samdos projektai pagal padalinį ir savininką, masinės samdos projektai pagal užduotį ir masinės samdos projektai                                                                                                                                                                    |

Šių ataskaitų diagramas ir plyteles galima filtruoti ir prisegti prie ataskaitų srities. Daugiau informacijos apie tai, kaip „Power BI“ filtruoti ir prisegti, žr. [Ataskaitų srities kūrimas ir konfigūravimas](https://powerbi.microsoft.com/en-us/guided-learning/powerbi-learning-4-2-create-configure-dashboards).

## <a name="extending-the-power-bi-content"></a>„Power BI“ turinio išplėtimas
Naudodami turinio paketus, kurie pateikiami „Microsoft Dynamics Lifecycle Services“ (LCS), žmonėms, kurie neprisijungia prie „Finance and Operations“ galite pateikti didžiąją analizę. Galite keisti šiuos turinio paketus, kad į juos įtrauktumėte kitas ataskaitas arba vaizdinius, o po to paskelbti turinio paketus savo Power BI.com nuomotojui analizei.

**Darbo jėgos metrikos** „Power BI“ turinį galite rasti LCS Bendrai naudojamo turto bibliotekoje. Norėdami gauti daugiau informacijos apie tai, kaip atsisiųsti turinį ir įdiegti jį savo organizacijoje, žr. [„Power BI“ turinys LCS iš „Microsoft“ ir jūsų partnerių](power-bi-content-microsoft-partners.md). Norėdami peržiūrėti demonstracinius duomenis, kuriuose parodoma, kaip diegti „Power BI“ turinį, žr. „Office Mix“ [„Power BI“ turinys iš „Microsoft“ ir partnerių „Dynamics Lifecycle Services“](https://mix.office.com/watch/9puyb1b2xs1w).

Įsitikinkite, kad atsisiunčiate **Darbo jėgos metrikos** „Power BI“ turinį, kuris taikomas jūsų naudojamai „Microsoft Dynamics 365‟ versijai.

>[!NOTE]
>.pbix failai, kurie pateikiami „Lifecycle Services“, taikomi tik „Finance and Operations“.

## <a name="understanding-the-data-model-and-entities"></a>Duomenų modelio ir objektų supratimas
Toliau pateiktoje lentelėje nurodomi objektai, kuriais pagrįstas turinys.

| Objektas                   | Turinys                                                                            | Ryšiai su kitais objektais |
|--------------------------|-------------------------------------------------------------------------------------|-----------------------------------|
| Kalendoriaus poslinkis          | Kalendoriaus poslinkiai ataskaitoms skaidyti                                                   | Buvusių pareigų priskyrimas, pareigų tendencija, darbuotojo tendencija, atleistas darbuotojas |
| Įmonė                  | Įmonės, pagal kurias filtruojamos ataskaitos                                                      | Dabartinis darbuotojas, atleistas darbuotojas, darbuotojo tendencija |
| Dabartinės pareigos         | Pareigos dabartinę datą, FTE, laisvos darbo vietos ir laisvos / užimtos darbo vietos | Darbas, pareigos |
| Dabartinis darbuotojas         | Darbuotojai dabartinę dieną, amžius ir darbuotojų skaičius                                  | Įmonė, geografinė vieta, darbuotojo vardas ir pavardė, atskaitingas (kam), darbuotojo pareigos, demografiniai duomenys, užduotis, darbas, pareigos |
| Data                     | Dienos, savaitės, mėnesiai ir metai                                                      | Buvusių pareigų priskyrimas, pareigų tendencija, atleistas darbuotojas, darbuotojo tendencija |
| Demografiniai duomenys             | Gimimo data, lytis etninė kilmė ir šeimyninė padėtis                            | Dabartinis darbuotojas, atleistas darbuotojas, darbuotojo tendencija |
| Užimtumas               | Pradžios data, pabaigos data ir perėjimo data                                           | Dabartinis darbuotojas, atleistas darbuotojas, darbuotojo tendencija |
| Geografinė vieta      | Miestas, seniūnija, pašto kodas ir šalis arba regionas                                    | Dabartinis darbuotojas, atleistas darbuotojas, darbuotojo tendencija |
| Darbas                      | Funkcija, tipas ir pareigos                                                           | Dabartinės pareigos, dabartinis darbuotojas |
| Ankstesnis pareigų priskyrimas | Priskyrimo priežastis, pradžios data, pabaigos data ir užduotis                                    | Kalendoriaus poslinkis, data, darbas, pareigos |
| Pozicija                 | Padalinys, FTE, pareigos, pareigų tipas ir pareigos                                 | Dabartinės pareigos, dabartinis darbuotojas |
| Pareigų tendencija           | Pareigos per tam tikrą laikotarpį, FTE ir užduotis                                                   | Kalendoriaus poslinkis, data, darbas, pareigos |
| Ataskaitos               | Vardas, pavardė ir vardas bei pavardė                                                | Dabartinis darbuotojas, atleistas darbuotojas, darbuotojo tendencija |
| Atleistas darbuotojas      | Atleisti darbuotojai, atleidimo data, pareigos ir užduotis                      | Įmonė, kompensacija, geografinė vieta, darbuotojo vardas ir pavardė, atskaitingas (kam), kalendoriaus poslinkis, data, darbuotojo pareigos, demografiniai duomenys, darbas, užduotis, pareigos |
| Darbuotojo vardas ir pavardė            | Vardas, pavardė ir vardas bei pavardė                                                | Dabartinis darbuotojas, atleistas darbuotojas, darbuotojo tendencija |
| Darbuotojo pareigos           | Pareigos ir paaukštinimo data                                                            | Dabartinis darbuotojas, atleistas darbuotojas, darbuotojo tendencija |
| Darbuotojų tendencija           | Darbuotojai per tam tikrą laiką, darbuotojų skaičius, įmonė ir pareigos                                 | Įmonė, kompensacija, geografinė vieta, darbuotojo vardas ir pavardė, atskaitingas (kam), kalendoriaus poslinkis, data, darbuotojo pareigos, demografiniai duomenys, darbas, užduotis |
| Masinės samdos projektas        | Masinės samdos projektų skaičius, projekto savininkas ir projekto būsena                     | Įmonė, masinės samdos eilutė |
| Masinės samdos eilutė           | Padalinys, įdarbinimo tipas ir pareigos                                           | Data, darbas, masinės samdos projektas |

Šie objektai buvo naudojami skaičiuojamiems matams duomenų modelyje sukurti. Tada šie skaičiuojami matai naudojami skaičiuojant pagrindinius efektyvumo indikatorius (KPI) ir „Power BI‟ turinyje naudojamas ataskaitas. Jei norite į ataskaitas ir ataskaitų sritį įtraukti papildomų skaičiavimų, galite iš LCS atsisiųsti ir modifikuoti failą .pbix. Šis failas yra numatytasis duomenų modelis, kuris buvo naudojamas „Power BI‟ turiniui kurti. Atlikę keitimus, galite kurti organizacinį turinio paketą ir ataskaitų sritį, kuriuose yra jūsų įtraukta informacija.
