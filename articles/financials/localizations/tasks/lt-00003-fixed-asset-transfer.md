--- 
title: "Generuoti ilgalaikio turto perkėlimo iš vieno sandėlio į kitą dokumentą (Lietuva)"
description: "Jei jūsų organizacijai reikia perkelti ilgalaikį turtą iš vieno padalinio į kitą ir du padaliniai nėra toje pačioje vietoje, perkėlimas turi būti patvirtintas važtaraščiu."
author: KimANelson
manager: AnnBe
ms.date: 02/17/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Lithuania
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 551227f0cce597c1a1f254fc71091173758dfc7c
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="generate-a-fixed-asset-transfer-between-warehouses-document-lithuania"></a>Generuoti ilgalaikio turto perkėlimo iš vieno sandėlio į kitą dokumentą (Lietuva)

[!include[task guide banner](../../includes/task-guide-banner.md)]

Jei jūsų organizacijai reikia perkelti ilgalaikį turtą iš vieno padalinio į kitą ir du padaliniai nėra toje pačioje vietoje, perkėlimas turi būti patvirtintas važtaraščiu. Taip pat reikia generuoti perkėlimo važtaraštį pakeitus darbuotoją, atsakingą už ilgalaikio turto perdavimą. Priklausomai nuo įgalintų parametrų, važtaraštis gali būti numeruojamas automatiškai arba neautomatiniu būdu.

Ši procedūra taikoma tik Lietuvai skirtoms funkcijoms. 

Procedūra buvo sukurta naudojant demonstracinių duomenų įmonę USMF, todėl prieš pradedant reikia rankiniu būdu pakeisti USMF juridinio subjekto pirminį adresą į LTU. 

Ši procedūra skirta už ilgalaikį turtą atsakingiems buhalteriams.


## <a name="preset-vehicle-models"></a>Iš naujo nustatyti transporto priemonių modelius
1. Eikite į Organizacijos administravimas > Nustatymas > Transporto priemonė > Transporto priemonių modeliai.
2. Spustelėkite Naujas.
3. Lauke Modelis įveskite reikšmę.
    * Ši vertė bus spausdinama važtaraštyje.  
4. Lauke Aprašas įveskite reikšmę.
5. Spustelėkite Įrašyti.

## <a name="set-up-packing-slip-auto-numbering"></a>Nustatyti automatinį važtaraščio numeravimą
1. Eikite į Organizacijos administravimas > Numeracijos > Skaitiklių valdymas.
2. Spustelėkite Redaguoti.
3. Lauke Modulis pasirinkite parinktį.
4. Lauke Sąskaitos kodas pasirinkite parinktį.
5. Pažymėkite žymės langelį Automatinis numeravimas.
6. Spustelėkite Įrašyti.
7. Eikite į Organizacijos administravimas > Numeracijos > SF numeravimo nustatymas.
8. Spustelėkite Redaguoti.
9. Lauke Numeravimas įveskite reikšmę.
10. Lauke Modulis pasirinkite parinktį.
11. Lauke Numeracijos kodas įveskite arba pasirinkite vertę.
    * Čia pasirinkta numeracija turi būti naudojama automatiniam važtaraščio numeravimui.  
12. Lauke Sąskaitos kodas pasirinkite parinktį.
13. Pažymėkite žymės langelį Tęsti.
14. Spustelėkite Įrašyti.

## <a name="generate-packing-slip"></a>Generuoti važtaraštį

## <a name="specify-transportation-details"></a>Nurodyti transportavimo informaciją
1. Eikite į Ilgalaikis turtas > Užklausos ir ataskaitos > Važtaraščiai.
2. Veiksmų srityje spustelėkite Bendra.
3. Spustelėkite Transportavimo informacija.
4. Spustelėkite Redaguoti.
5. Lauke Spausdinti transportavimo informaciją pasirinkite Taip.
    * Jei pasirinkta, transportavimo informacija, kurią galite nurodyti šioje formoje, bus spausdinama važtaraštyje.  
6. Lauke Išduotos prekės įveskite arba pasirinkite vertę.
7. Lauke Paketas įveskite reikšmę.
8. Lauke Vežėjo tipas pasirinkite parinktį.
9. Lauke Vežėjas įveskite arba pasirinkite reikšmę.
10. Lauke Modelis įveskite arba pasirinkite reikšmę.
11. Lauke Registracijos numeris įveskite reikšmę.
12. Lauke Priekabos registracijos numeris įveskite vertę.
13. Lauke Vairuotojas įveskite arba pasirinkite reikšmę.
14. Lauke Vairuotojo vardas ir pavardė įveskite reikšmę.
15. Lauke Pakrovimo data ir laikas įveskite datą ir laiką.
16. Lauke Pakrovimo adresas įveskite arba pasirinkite reikšmę.
17. Spustelėkite Įrašyti.
    * Baigę turto iškrovimo procesą taip pat galite užpildyti važtaraščio iškrovimo informaciją.  
18. Lauke Iškrovimo data ir laikas įveskite datą ir laiką.
19. Lauke Iškrovimo adresas įveskite arba pasirinkite reikšmę.
20. Spustelėkite Įrašyti.
21. Uždarykite puslapį.

## <a name="verify-the-packing-slip-report"></a>Patikrinti važtaraščio ataskaitą
1. Veiksmų srityje spustelėkite Bendra.
2. Spustelėkite Ilgalaikio turto važtaraštis.
3. Spustelėkite GERAI.
    * Sugeneravus ataskaitą bus spausdinama visa transportavimo informacija.  


