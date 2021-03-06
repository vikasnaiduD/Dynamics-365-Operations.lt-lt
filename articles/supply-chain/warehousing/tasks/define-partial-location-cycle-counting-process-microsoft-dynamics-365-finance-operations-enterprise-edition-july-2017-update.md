--- 
title: "Nustatyti dalinį vietos ciklų skaičiavimo procesą "
description: "Kai naudojate ciklo skaičiavimo planus skaičiavimo darbui sukurti, galite nukreipti faktines skaičiavimo operacijas, nurodydami, kad būtų skaičiuojami tik konkretūs produktai ir produkto variantai vietoj visų turimų atsargų vietoje inventorizavimo."
author: YuyuScheller
manager: AnnBe
ms.date: 06/23/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.author: yuyus
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 030f0f75d64c97f1109f36c9fd38283c2d1fa7b0
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="define-partial-location-cycle-counting-process"></a>Nustatyti dalinį vietos ciklų skaičiavimo procesą  

[!include[task guide banner](../../includes/task-guide-banner.md)]

Kai naudojate ciklo skaičiavimo planus skaičiavimo darbui sukurti, galite nukreipti faktines skaičiavimo operacijas, nurodydami, kad būtų skaičiuojami tik konkretūs produktai ir produkto variantai vietoj visų turimų atsargų vietoje inventorizavimo. Filtruodamas konkrečius produktus, sandėlio vadovas gali sumažinti peržiūros pridėtines išlaidas, padėti išvengti konsolidavimo klaidų ir sutaupyti laiko. Sąrankos užduotis paprastai atlieka sandėlio vadovas. Šią procedūrą galite atlikti naudodami demonstracinių duomenų įmonę USMF arba savo duomenis.


## <a name="create-a-cycle-counting-work-template"></a>Sukurkite ciklo skaičiavimo darbo šabloną
1. Pasirinkite Sandėlio valdymas > Nustatymas > Darbas > Darbo šablonai.
2. Lauke Darbo užsakymo tipas pasirinkite „Ciklo skaičiavimas“.
3. Spustelėkite Naujas.
4. Lauke Sekos numeris įveskite skaičių.
    * Rūšiavimo tvarka yra nuo mažiausio iki didžiausio skaičiaus. Reikšmė turi būti didesnė už 0 (nulį).  
5. Sąraše pažymėkite pasirinktą eilutę.
6. Lauke „Darbo šablonas“ įveskite reikšmę.
7. Lauke Darbo šablonas įveskite vertę.
8. Lauke Darbo telkinio ID įveskite arba pasirinkite reikšmę.
9. Lauke Darbo prioritetas įveskite skaičių.
10. Spustelėkite Įrašyti.
11. Spustelėkite Naujas.
12. Sąraše pažymėkite pasirinktą eilutę.
13. Lauke Darbo tipas pasirinkite „Skaičiavimas‟.
14. Lauke Darbo klasės ID įveskite arba pasirinkite reikšmę.
15. Spustelėkite Įrašyti.
16. Spustelėkite Darbo eilučių lūžiai.
17. Spustelėkite Naujas.
18. Lauke Sekos numeris įveskite skaičių.
    * Rūšiavimo tvarka yra nuo mažiausio iki didžiausio skaičiaus. Reikšmė turi būti didesnė už 0 (nulį).  
19. Spustelėkite Įrašyti.
20. Uždarykite puslapį.
21. Uždarykite puslapį.

## <a name="create-a-cycle-counting-plan"></a>Sukurkite ciklo skaičiavimo planą
1. Pasirinkite Sandėlio valdymas > Nustatymai > Ciklo skaičiavimas > Ciklų skaičiavimo planai.
2. Spustelėkite Naujas.
3. Lauke Ciklo skaičiavimo plano ID įveskite vertę.
4. Lauke Aprašas surinkite reikšmę.
5. Lauke Maksimalus ciklų skaičiavimo skaičius įveskite skaičių.
6. Lauke Darbo šablonas įveskite arba pasirinkite reikšmę.
7. Spustelėkite Naujas.
8. Lauke Sekos numeris įveskite skaičių.
    * Rūšiavimo tvarka yra nuo mažiausio iki didžiausio skaičiaus. Reikšmė turi būti didesnė už 0 (nulį).  
9. Lauke Aprašas įveskite reikšmę.
10. Spustelėkite Įrašyti.
11. Spustelėkite Apibrėžti produkto užklausą.
12. Sąraše pažymėkite pasirinktą eilutę.
13. Lauke Kriterijai įveskite arba pasirinkite reikšmę.
14. Spustelėkite GERAI.
15. Uždarykite puslapį.


