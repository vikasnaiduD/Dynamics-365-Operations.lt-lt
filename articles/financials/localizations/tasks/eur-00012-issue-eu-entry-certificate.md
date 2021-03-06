--- 
title: "Išduoti ES įrašo sertifikatą"
description: "Ši procedūra padės įgalinti ES įrašo sertifikatą, konfigūruoti kliento sąskaitą, kad būtų galima naudoti įrašų sertifikatus ir išduoti sertifikatą."
author: mrolecki
manager: AnnBe
ms.date: 02/26/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Operations
ms.search.region: Austria, Belgium, Czech Republic, Denmark, Estonia, Finland, France, Germany, Hungary, Ireland, Italy, Latvia, Lithuania, Netherlands, Poland, Spain, Sweden, United Kingdom
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: ff00ff0df3835ee2cbf21219ad6f07bfeba6e7ac
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="issue-an-eu-entry-certificate"></a>Išduoti ES įrašo sertifikatą

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ši procedūra padės įgalinti ES įrašo sertifikatą, konfigūruoti kliento sąskaitą, kad būtų galima naudoti įrašų sertifikatus ir išduoti sertifikatą. Ši procedūra buvo sukurta naudojant demonstracinių duomenų įmonės DEMF.


## <a name="enable-entry-certificate-management"></a>Įgalinti įrašo sertifikato valdymo funkciją
1. Pasirinkite Gautinos sumos > Nustatymai > Gautinų sumų parametrai.
2. Spustelėkite skirtuką Siuntos.
3. Išplėskite skyrių Įrašo sertifikatas.
4. Lauke Įgalinti įrašo sertifikato valdymą pasirinkite Taip.
5. Lauke Įgalinti įrašo sertifikato išdavimą pasirinkite Taip.
6. Spustelėkite skirtuką Numeracijos.
7. Sąraše raskite ir pasirinkite Įrašo sertifikato eilutė.
8. Lauke Numeracijos kodas įveskite arba pasirinkite vertę.

## <a name="set-up-a-customer"></a>Kliento nustatymas
1. Pasirinkite Gautinos sumos > Klientai > Visi klientai.
2. Norėdami rasti įrašus, naudokite spartųjį filtrą. Pvz., filtruokite lauką Sąskaita naudodami vertę „DE-015“.
3. Atidarykite kliento sąskaitos informaciją.
4. Spustelėkite Redaguoti.
5. Išplėskite skyrių SF ir pristatymas.
6. Lauke Įrašo sertifikatas būtinas pasirinkite Taip.
7. Lauke Išduoti įrašo sertifikatą pasirinkite Taip.
8. Spustelėkite Įrašyti.

## <a name="create-an-eu-entry-certificate-automatically"></a>ES įrašo sertifikato automatinis kūrimas
1. Pasirinkite Gautinos sumos > Užsakymai > Visi pardavimo užsakymai.
2. Spustelėkite Naujas.
3. Lauke Kliento sąskaita įveskite arba pasirinkite reikšmę.
4. Spustelėkite Gerai.
5. Lauke Prekės numeris įveskite arba pasirinkite reikšmę.
6. Spustelėkite Įrašyti.
7. Veiksmų srityje spustelėkite Paimti ir pakuoti.
8. Spustelėkite Registruoti važtaraštį.
9. Išplėskite skyrių Parametrai.
10. Lauke Kiekis pasirinkite Visi.
11. Išvalykite žymės langelį Išduoti įrašo sertifikatą.
    * Įrašo sertifikatas gali būti išduotas registruojant važtaraštį arba išrašant užsakymo SF. Palikite atžymėtą žymės langelį Išduoti įrašo sertifikatą, jei norite, kad jis būtų išduotas vėliau.  
12. Spustelėkite GERAI.
13. Spustelėkite GERAI.
14. Veiksmų srityje spustelėkite Sąskaita faktūra.
15. Spustelėkite Sąskaita faktūra.
    * Patikrinkite, ar skyriuje Apžvalga pažymėti žymės langeliai Įrašo sertifikatas būtinas ir Išduoti įrašo sertifikatą.  Taip pat galite pažymėti žymės langelį Spausdinti įrašo sertifikatą, kad galėtumėte sertifikatą atsispausdinti.  
16. Spustelėkite GERAI.
17. Spustelėkite GERAI.
18. Veiksmų srityje spustelėkite Sąskaita faktūra.
19. Spustelėkite Sąskaita faktūra.
20. Veiksmų srityje spustelėkite Sąskaita faktūra.
21. Spustelėkite Rodyti išduotus įrašų sertifikatus.
22. Spustelėkite Spausdinti.
23. Uždarykite puslapį.
24. Spustelėkite keisti būseną.
25. Lauke Nauja būsena pasirinkite parinktį.
26. Spustelėkite GERAI.
27. Uždarykite puslapį.

## <a name="create-an-eu-entry-certificate-manually"></a>ES įrašo sertifikato kūrimas rankiniu būdu
1. Veiksmų srityje spustelėkite Sąskaita faktūra.
2. Spustelėkite Kurti įrašo sertifikatą.
3. Spustelėkite Gerai.
4. Veiksmų srityje spustelėkite Sąskaita faktūra.
5. Spustelėkite Rodyti išduotus įrašų sertifikatus.


