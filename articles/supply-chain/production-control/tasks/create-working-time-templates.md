--- 
title: "Darbo laiko šablonų kūrimas"
description: "Darbo laiko šablonai nustato savaitės darbo valandas ir yra naudojami generuoti darbo laikus tam tikram laikotarpiui."
author: sorenva
manager: AnnBe
ms.date: 03/02/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: sorenand
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 2df37747601618fc3d45734152a05aedd39500a6
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="create-working-time-templates"></a>Darbo laiko šablonų kūrimas

[!include[task guide banner](../../includes/task-guide-banner.md)]

Darbo laiko šablonai nustato savaitės darbo valandas ir yra naudojami generuoti darbo laikus tam tikram laikotarpiui. Ši procedūra nurodo, kaip nustatyti darbo laiko šabloną, naudojant darbo laiko planavimo ypatybes, skirtas darbo laiko intervalas skirstyti. Šią procedūrą galite atlikti naudodami demonstracinių duomenų įmonę USMF arba savo duomenis.

1. Pasirinkite Visos darbo sritys > Išteklių naudojimo ciklo valdymas.
2. Spustelėkite Darbo laiko šablonai.

## <a name="create-working-time-template"></a>Kurti darbo laiko šabloną
1. Spustelėkite Naujas.
2. Šablono lauke Darbo laikas įveskite vertę.
3. Lauke Pavadinimas surinkite reikšmę.
4. Išplėskite skyrių Pirmadienis.
5. Spustelėkite Pridėti.
6. Lauke Nuo įveskite laiką.
    * Nurodykite laiką, kada darbas prasideda ryte.  
7. Lauke Iki įveskite laiką.
    * Nurodykite laiką, kada būna darbuotojų pietų pertrauka.  
8. Spustelėkite Pridėti.
9. Lauke Nuo įveskite laiką.
    * Nurodykite laiką, kada darbas tęsiamas po pietų.  
10. Lauke Iki įveskite laiką.
    * Nurodykite darbo dienos pabaigą.  

## <a name="replicate-working-times-to-all-week-days"></a>Dubliuoti visos savaitės dienų darbo laikus
1. Spustelėkite Kopijuoti dieną.
    * Kopijuokite darbo laiko apibrėžimus iš pirmadienio į antradienį.  
2. Spustelėkite GERAI.
3. Spustelėkite Kopijuoti dieną.
    * Kopijuokite darbo laiko apibrėžimus iš pirmadienio į trečiadienį.  
4. Lauke Į dieną pasirinkite pasirinktį.
5. Spustelėkite GERAI.
6. Spustelėkite Kopijuoti dieną.
    * Kopijuokite darbo laiko apibrėžimus iš pirmadienio į ketvirtadienį.  
7. Lauke Į dieną pasirinkite pasirinktį.
8. Spustelėkite GERAI.
9. Spustelėkite Kopijuoti dieną.
    * Kopijuokite darbo laiko apibrėžimus iš pirmadienio į penktadienį.  
10. Lauke Į dieną pasirinkite pasirinktį.
11. Spustelėkite GERAI.

## <a name="define-time-slots-for-special-operations"></a>Nurodyti specialiųjų operacijų laiko atkarpas
1. Išplėskite skyrių Penktadienis.
2. Sąraše raskite ir pasirinkite norimą įrašą.
3. Lauke Ypatybė įveskite arba pasirinkite vertę.
4. Sąraše raskite ir pasirinkite norimą įrašą.
5. Lauke Ypatybė įveskite arba pasirinkite vertę.

## <a name="mark-weekend-days-as-closed-for-pickup"></a>Pažymėti savaitgalio dienas kaip uždarytas, kada negalima paimti
1. Išplėskite skyrių Šeštadienis.
2. Lauke Uždaryta paimti pasirinkite Taip.
3. Išplėskite skyrių Sekmadienis.
4. Lauke Uždaryta paimti pasirinkite Taip.


