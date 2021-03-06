--- 
title: "Kompensavimo tinklelių nustatymas"
description: "Kompensavimo tinkleliai naudojami nustatyti ir prižiūrėti pastoviųjų atlyginimo dalių planų mokėjimo struktūras."
author: kherr75
manager: AnnBe
ms.date: 03/02/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-365-talent
ms.technology: 
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Operations, Talent
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 258149dbd610dafb8daacaf54c61e69898ca35d6
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="set-up-compensation-grids"></a>Kompensavimo tinklelių nustatymas

[!include[task guide banner](../../includes/task-guide-banner.md)]

Kompensavimo tinkleliai naudojami nustatyti ir prižiūrėti pastoviųjų atlyginimo dalių planų mokėjimo struktūras. Kompensacijos tinklelius galima bendrai naudoti keliems planams arba nukopijuoti kuriant naują kompensavimo planą.  Prieš kuriant kompensacijos tinklelį, Lygiai ir Nuorodos taškai turi būti nustatyti. Šiame pavyzdyje bus sukurtas naujas kompensacijos tinklelio Klasės tipas naudojant demonstracinius duomenis Lygiams ir Nuorodos taškams. Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.


## <a name="set-up-information-about-the-compensation-grid"></a>Nustatyti informaciją apie kompensacijos tinklelį
1. Pasirinkite Personalas > Kompensacija > Pastovioji atlyginimo dalis > Kompensacijos tinkleliai.
2. Spustelėkite Naujas.
3. Lauke Tinklelis įveskite vertę.
4. Lauke Aprašas įveskite reikšmę.
5. Lauke „Tipas“ pasirinkite parinktį.
6. Lauke Nuorodos nustatymas įveskite arba pasirinkite vertę.
7. Lauke Valiuta įveskite arba pasirinkite vertę.
8. Lauke Valiuta surinkite reikšmę.
9. Lauke Įsigaliojimo data įveskite datą.

## <a name="add-levels-to-the-compensation-structure"></a>Įtraukti lygius į kompensacijos struktūrą
1. Spustelėkite Kompensacijos struktūra.
2. Sąraše pažymėkite pasirinktą eilutę.
3. Lauke Lygis įveskite arba pasirinkite vertę.
4. Spustelėkite Naujas.
5. Sąraše pažymėkite pasirinktą eilutę.
6. Lauke Lygis įveskite arba pasirinkite vertę.
7. Spustelėkite Naujas.
8. Sąraše pažymėkite pasirinktą eilutę.
9. Lauke Lygis įveskite arba pasirinkite vertę.
10. Spustelėkite Naujas.
11. Sąraše pažymėkite pasirinktą eilutę.
12. Lauke Lygis įveskite arba pasirinkite vertę.
13. Spustelėkite Naujas.
14. Sąraše pažymėkite pasirinktą eilutę.
15. Lauke Lygis įveskite arba pasirinkite vertę.

## <a name="fill-in-the-compensation-structure-with-values"></a>Užpildyti kompensacijos struktūrą vertėmis
1. Sąraše pažymėkite pasirinktą eilutę.
    * Šiuo momentu kompensacijų vertes galima įvesti rankiniu būdu į kiekvieną lentelės lauką arba galima naudoti Masinio keitimo funkciją norint lengvai užpildyti kelis laukus ir atlikti pagrindinius skaičiavimus.  
2. Spustelėkite Masinis keitimas.
    * Šiam tinkleliui pirmiausia pritaikysime pirmojo lygio vidurio taško vertę visuose lentelės laukuose. Tai bus kompensavimo matricos pagrindas.  
3. Lauke Koregavimo tipas pasirinkite pasirinktį.
4. Lauke Koregavimo suma įveskite skaičių.
5. Pažymėkite arba atžymėkite visas sąrašo eilutes.
6. Spustelėkite Taikyti tinkleliui.
    * Dabar naudojame masinio keitimo funkciją sumai padidinti kiekviename tolesniame lygyje pagal tam tikrą procentą arba sumą. Šiame pavyzdyje kiekvienas lygis turės 12,5 % paplitimą tarp jų vidurio taškų.  
7. Lauke Koregavimo tipas pasirinkite pasirinktį.
8. Lauke Koregavimo suma įveskite skaičių.
9. Sąraše raskite ir pasirinkite norimą įrašą.
10. Sąraše raskite ir pasirinkite norimą įrašą.
11. Sąraše raskite ir pasirinkite norimą įrašą.
12. Sąraše raskite ir pasirinkite norimą įrašą.
13. Spustelėkite Taikyti tinkleliui.
14. Sąraše raskite ir pasirinkite norimą įrašą.
15. Sąraše raskite ir pasirinkite norimą įrašą.
16. Sąraše raskite ir pasirinkite norimą įrašą.
17. Spustelėkite Taikyti tinkleliui.
18. Sąraše raskite ir pasirinkite norimą įrašą.
19. Sąraše raskite ir pasirinkite norimą įrašą.
20. Spustelėkite Taikyti tinkleliui.
21. Sąraše raskite ir pasirinkite norimą įrašą.
22. Spustelėkite Taikyti tinkleliui.
    * Dabar naudosime masinio keitimo funkciją kiekvieno lygio minimaliam ir maksimaliam nuorodos taškams koreguoti. Šiame pavyzdyje naudosime 50 % paplitimą, kad Minimalus atskaitos taškas būtų pakoreguotas -20 %, o Maksimalus – pakoreguotas +20 %.  
23. Lauke Koregavimo suma įveskite skaičių.
24. Lauke Nuorodos taškas įveskite arba pasirinkite vertę.
25. Pažymėkite arba atžymėkite visas sąrašo eilutes.
26. Spustelėkite Taikyti tinkleliui.
27. Lauke Koregavimo suma įveskite skaičių.
28. Lauke Nuorodos taškas įveskite arba pasirinkite vertę.
29. Pažymėkite arba atžymėkite visas sąrašo eilutes.
30. Spustelėkite Taikyti tinkleliui.


