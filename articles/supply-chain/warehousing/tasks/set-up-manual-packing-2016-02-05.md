--- 
title: "Neautomatinio pakavimo nustatymas (2016 m. vasario ir gegužės mėn.)"
description: "Atliekant pakavimo procesą, produktus galima tikrinti ir pakuoti į konteinerius."
author: BibiSp
manager: AnnBe
ms.date: 11/04/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: bis
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 7f992a6a1655cd868d79228c490d59b46bfae715
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="set-up-manual-packing-february--may-2016-only"></a>Neautomatinio pakavimo nustatymas (2016 m. vasario ir gegužės mėn.)

[!include[task guide banner](../../includes/task-guide-banner.md)]

Atliekant pakavimo procesą, produktus galima tikrinti ir pakuoti į konteinerius. Atlikdami ši procesą sandėlio darbininkai produktus paima iš saugojimo vietų ir perkelia į pakavimo stotį, kurioje jie patikrina prekių kiekį ir tipus bei jas priskiria į atitinkamus konteinerius. Kai konteineris yra visiškai supakuotas, jie jį gali uždaryti ir perkelti į pakrovimo rampas, ir produktus galima siųsti. Šioje procedūroje naudojama demonstracinė įmonė USMF.


## <a name="set-up-location-profiles"></a>Nustatyti vietų šablonus
1. Pasirinkite Sandėlio valdymas > Nustatymas > Sandėlis > Vietos profiliai.
2. Spustelėkite Naujas.
    * Vietos profilis naudojamas su pakavimo stotimis ir jame pateikiama vietos informacija ir taisyklės.  
3. Lauke Vietos šablono ID įveskite vertę.
4. Lauke Pavadinimas surinkite reikšmę.
5. Lauke Vietos formatas įveskite arba pasirinkite reikšmę.
6. Lauke Vietos tipas įveskite arba pasirinkite reikšmę.
7. Lauke Leisti skirtingas prekes pasirinkite Taip.
8. Lauke Leisti įvairias atsargų būsenas pasirinkite Taip.
9. Lauke Nepaisyti paketo dienų taisyklių pasirinkite Taip.
10. Uždarykite puslapį.

## <a name="set-up-warehouse-management-parameters"></a>Sandėlio valdymo parametrų valdymas 
1. Pasirinkite Sandėlio valdymas > Nustatymas > Sandėlio valdymo parametrai.
2. Spustelėkite skirtuką Pakavimas.
3. Lauke Pakavimo vietos profilio ID įveskite arba pasirinkite reikšmę.
    * Pasirinkite vietos profilį, kurį norite naudoti pakuodami.  
4. Uždarykite puslapį.

## <a name="set-up-container-types"></a>Konteinerių tipų nustatymas
1. Pasirinkite Sandėlio valdymas > Nustatymas > Konteineriai > Konteinerių tipai.
2. Spustelėkite Naujas.
    * Galite apibrėžti naudotinų konteinerių tipus. Galite nurodyti faktines konteinerio dimensijas – taros svorį, didžiausią svorį, didžiausią tūrį, ilgį, plotį ir svorį.  Atributai yra pritaikyti laukai, kuriuose galite įtraukti papildomų konteinerio tipo dimensijų.     
3. Lauke Konteinerio tipo kodas įveskite reikšmę.
4. Lauke Aprašas įveskite reikšmę.
5. Lauke „Taros svoris“ įveskite skaičių.
6. Lauke Didžiausias svoris įveskite skaičių.
7. Lauke „Tūris“ įveskite skaičių.
8. Lauke Ilgis įveskite skaičių.
9. Lauke Plotis įveskite skaičių.
10. Lauke Aukštis įveskite skaičių.
11. Spustelėkite Įrašyti.
12. Uždarykite puslapį.

## <a name="set-up-packing-profiles"></a>Pakavimo profilių nustatymas
1. Pasirinkite Sandėlio valdymas > Nustatymas > Pakavimas > Pakavimo profiliai.
2. Spustelėkite Naujas.
3. Lauke Pakavimo profilio ID įveskite reikšmę.
4. Lauke Aprašas įveskite reikšmę.
5. Lauke Konteinerio uždarymo profilio ID įveskite arba pasirinkite reikšmę.
    * Konteinerio uždarymo profilio ID yra neprivalomas ir jis yra numatytasis šio pakavimo profilio konteinerio uždarymo profilis.  
6. Lauke Konteinerio ID režimas pasirinkite parinktį.
    * Šia parinktimi nustatoma, ar konteinerio ID bus automatiškai sugeneruotas konteinerį sukūrus, ar konteinerio ID bus sukurtas rankiniu būdu.  
7. Lauke Konteinerio tipas įveskite arba pasirinkite reikšmę.
    * Konteinerio tipas pagal numatytuosius parametrus bus naudojamas kuriant naują konteinerį.  
8. Pasirinkite žymės langelį Automatiškai kurti konteinerį uždarant konteinerį.
9. Spustelėkite Įrašyti.
10. Uždarykite puslapį.

## <a name="set-up-container-closing-profiles"></a>Konteinerių uždarymo profilių nustatymas
1. Pasirinkite Sandėlio valdymas > Nustatymas > Konteineriai > Konteinerių uždarymo profiliai.
    * Konteinerių uždarymo profiliais apibrėžiama, kas vyksta konteinerį uždarius. Galite nustatyti kelis konteinerių uždarymo profilius.       
2. Spustelėkite Naujas.
3. Lauke Konteinerio uždarymo profilio ID įveskite reikšmę.
4. Lauke Aprašas įveskite reikšmę.
5. Lauke Deklaracija pasirinkite parinktį.
    * Nurodykite, ar deklaruojama bus uždarant konteinerius, ar patvirtinant siuntą. Atkreipkite dėmesį, kad, norint deklaruoti, reikalingas modulis Transportavimo valdymas. Kad deklaravimas veiktų, jį reikia įdiegti transportavimo mechanizmuose.  
6. Lauke Sandėlis įveskite arba pasirinkite reikšmę.
7. Lauke Galutinės siuntos numatytoji vieta įveskite arba pasirinkite reikšmę.
    * Tai bus vieta, į kurią produktai bus perkelti uždarius konteinerius. Sandėlio parametruose turi būti apibrėžtas šios vietos profilis.  
8. Lauke Svorio vienetas įveskite arba pasirinkite reikšmę.
9. Spustelėkite Įrašyti.


