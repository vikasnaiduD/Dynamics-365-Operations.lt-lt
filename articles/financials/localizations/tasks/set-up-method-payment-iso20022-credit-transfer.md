--- 
title: "Nustatyti ISO20022 kredito pervedimo mokėjimo būdą"
description: "Šioje procedūroje parodoma, kaip nustatyti tiekėjo mokėjimo būdą, skirtą atlikti ISO20022 kredito pervedimą arba kito tipo mokėjimą, naudojant elektronines ataskaitas failui generuoti."
author: mrolecki
manager: AnnBe
ms.date: 10/24/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: bed51f8749dfa0264ad39f51f9ceb295ac46fe93
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="set-up-method-of-payment-for-iso20022-credit-transfer"></a>Nustatyti ISO20022 kredito pervedimo mokėjimo būdą

[!include[task guide banner](../../includes/task-guide-banner.md)]

Šioje procedūroje parodoma, kaip nustatyti tiekėjo mokėjimo būdą, skirtą atlikti ISO20022 kredito pervedimą arba kito tipo mokėjimą, naudojant elektronines ataskaitas failui generuoti. 

Prieš atlikdami šią užduotį, turite nustatyti eksporto formato konfigūracijas ir mokėjimo sąskaitas.

Ši užduotis buvo sukurta naudojant demonstracinių duomenų įmonę DEMF.

Tai yra trečioji iš penkių procedūrų, kuriose aprašomas kliento mokėjimo naudojant elektroninių ataskaitų konfigūracijas procesas. Ši procedūra yra skirta funkcijai, įtrauktai į „Dynamics 365 for Operations“ 1611 versiją.

1. Pasirinkite Mokėtinos sumos > Mokėjimų sąranka > Mokėjimo būdai.
2. Norėdami rasti įrašus, naudokite spartųjį filtrą. Pvz., filtruokite lauką Mokėjimo būdas reikšme „SEPA CT“.
3. Spustelėkite Redaguoti.
4. Lauke Laikotarpis pasirinkite „Iš viso‟.
5. Lauke Mokėjimo tipas pasirinkite „Elektroninis mokėjimas“.
6. Išplėskite dalį Failo formatai.
7. Lauke Bendrosios elektroninės ataskaitos pasirinkite Taip.
8. Lauke Eksportuoti formato konfigūraciją įveskite arba pasirinkite reikšmę.
    * Sąraše pasirinkite reikšmę ISO20022 kredito pervedimas (DE). Jei sąrašas yra tuščias, nėra importuotos ir aktyvios tiekėjo mokėjimų eksporto formato konfigūracijos.  
9. Lauke Kliento sąskaita pasirinkite „Bankas‟.
10. Lauke Mokėjimo sąskaita nurodykite reikšmes „DEMF OPER‟.
11. Spustelėkite Įrašyti.


