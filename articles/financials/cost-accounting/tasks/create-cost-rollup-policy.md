--- 
title: Kurti savikainos sumavimo strategija
description: "Ši procedūra parodo, kaip sukurti savikainos sumavimo strategiją ir sukurti taisykles strategijai."
author: YuyuScheller
manager: AnnBe
ms.date: 06/27/2017
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
ms.openlocfilehash: 42656cbf445fd3f79844884d7d35243c5b051a4a
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="create-a-cost-rollup-policy"></a>Kurti savikainos sumavimo strategija

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ši procedūra parodo, kaip sukurti savikainos sumavimo strategiją ir sukurti taisykles strategijai. Kuriant šią procedūrą buvo naudojami USP2 demonstraciniai duomenys.


## <a name="create-a-policy"></a>Sukurkite strategiją
1. Eikite į Išlaidų apskaita > Strategijos > Savikainos sumavimo strategijos.
2. Spustelėkite Naujas.
3. Lauke Strategijos pavadinimas įrašykite reikšmę.
4. Lauke Aprašas įveskite reikšmę.
5. Lauke Savikainos objekto dimensijų hierarchija įveskite arba pasirinkite reikšmę.
    * Pasirinkite Savikainos sumavimo CC.  
6. Lauke Savikainos elementų dimensijų hierarchija įveskite arba pasirinkite reikšmę.
    * Pasirinkite Savikainos sumavimo CC.  
7. Spustelėkite Įrašyti.

## <a name="create-rules-for-the-cost-rollup-policy"></a>Sukurkite savikainos sumavimo strategijos taisykles
1. Spustelėkite Naujas.
2. Sąraše pažymėkite pasirinktą eilutę.
3. Lauke Savikainos objekto dimensijų hierarchijos mazgas įveskite arba pasirinkite reikšmę.
    * Pasirinkite 007.  
4. Lauke Savikainos elementų dimensijų hierarchijos mazgas įveskite arba pasirinkite reikšmę.
    * Pasirinkite Savikainos sumavimo CE.  
5. Lauke Antrinis savikainos elementas įveskite arba pasirinkite reikšmę.
    * Šiam pavyzdžiui priskirkite antrinį savikainos elementą CC-007 išlaidų centrui.  
6. Spustelėkite Naujas.
7. Sąraše pažymėkite pasirinktą eilutę.
8. Lauke Savikainos objekto dimensijų hierarchijos mazgas įveskite arba pasirinkite reikšmę.
    * Pasirinkite 008.  
9. Lauke Savikainos elementų dimensijų hierarchijos mazgas įveskite arba pasirinkite reikšmę.
    * Pasirinkite Savikainos sumavimo CE.  
10. Lauke Antrinis savikainos elementas įveskite arba pasirinkite reikšmę.
    * Šiam pavyzdžiui priskirkite antrinį savikainos elementą CC-008 išlaidų centrui.  
11. Spustelėkite Naujas.
12. Sąraše pažymėkite pasirinktą eilutę.
13. Lauke Savikainos objekto dimensijų hierarchijos mazgas įveskite arba pasirinkite reikšmę.
    * Pasirinkite 009.  
14. Lauke Savikainos elementų dimensijų hierarchijos mazgas įveskite arba pasirinkite reikšmę.
    * Pasirinkite Savikainos sumavimo CE.  
15. Lauke Antrinis savikainos elementas įveskite arba pasirinkite reikšmę.
    * Šiam pavyzdžiui priskirkite antrinį savikainos elementą CC-009 išlaidų centrui.  
    * Tęskite, kol visi išlaidų centrai bus susieti su jų atitinkamais antrinės savikainos elementais.  
16. Spustelėkite Įrašyti.


