--- 
title: "Elektroninių parašų nustatymas"
description: "Naudokite šią procedūrą norėdami nustatyti elektroninius parašus."
author: maertenm
manager: AnnBe
ms.date: 11/10/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: sericks
ms.search.scope: Operations
ms.search.region: Global
ms.author: maertenm
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 11fee0b2358e6a2b84c221f8eb06e32c888e5f44
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="set-up-electronic-signatures"></a>Elektroninių parašų nustatymas

[!include[task guide banner](../../includes/task-guide-banner.md)]

Naudokite šią procedūrą norėdami nustatyti elektroninius parašus. Elektroninis parašas patvirtina asmens, kuris ketina pradėti ar patvirtinti skaičiavimo procesą, tapatybę. Juriant šią procedūrą naudojama demonstracinių duomenų įmonė yra DAT.


## <a name="enable-the-electronic-signature-configuration-key"></a>Elektroninio parašo konfigūracijos rakto įgalinimas
1. Pasirinkite Sistemos administravimas > Nustatymai > Licencijos konfigūracija.
2. Medyje išplėskite „Administravimas“.
    * Patikrinkite, ar pažymėtas žymės langelis Elektroninis parašas.  
    * Jei žymės langelis Elektroninis parašas nepažymėtas, turite įjungti techninės priežiūros režimą. Priežiūros režimą galima įjungti šioje aplinkoje paleidžiant priežiūros užduotį iš „Lifecycle Services“ arba vietinėje sistemoje naudojant įrankį Deployment.Setup.  
3. Uždarykite puslapį.

## <a name="set-up-electronic-signature-parameters"></a>Elektroninio parašo parametrų nustatymas
1. Pasirinkite Organizacijos administravimas > Nustatymai > Elektroninis parašas > Elektroninio parašo parametrai.
2. Spustelėkite Redaguoti.
3. Lauke Pastaba įveskite reikšmę.
    * Įveskite pranešimą, kurį pasirašantieji gaus, kai bus reikalaujama parašo. Galite įvesti bet kokį tekstą. Paprastai šis tekstas nurodo vartotojui, ką reiškia elektroninis dokumento pasirašymas.  
    * Jei norite įvesti pranešimo tekstą kitomis kalbomis, spustelėkite mygtuką Vertimai.  
4. Spustelėkite Įrašyti.
5. Uždarykite puslapį.

## <a name="set-up-reason-codes-for-electronic-signatures"></a>Elektroninių parašų priežasčių kodų nustatymas
1. Pasirinkite Organizacijos administravimas > Nustatymai > Elektroninis parašas > Elektroninio parašo priežasčių kodai.
2. Spustelėkite Naujas.
    * Prieš naudodami elektroninius parašus turite nustatyti priežasčių kodus. Galiojantis priežasties kodas būtinas pasirašant dokumentą.     Pasirašantysis pasirenka priežasties kodą, siekdamas nurodyti elektroninio parašo paskirtį. Pavyzdžiui, priežasties kodas gali būti naudojamas nurodyti teisėtą patvirtinimą.  
3. Lauke Priežasties kodas įveskite reikšmę.
4. Lauke Aprašas įveskite reikšmę.
    * Jei reikia, įveskite papildomus priežasties kodus.  
5. Spustelėkite Įrašyti.
6. Uždarykite puslapį.

## <a name="require-electronic-signatures-for-existing-processes"></a>Elektroninių parašų prašymas esamiems procesams
1. Pasirinkite Organizacijos administravimas > Nustatymai > Elektroninis parašas > Elektroniniam parašui taikomi reikalavimai.
2. Sąraše raskite ir pasirinkite norimą įrašą.
    * Pasirinkti procesą, kuriam būtini elektroniniai parašai.  
3. Pažymėkite arba išvalykite žymės langelį Būtinas parašas.
    * Pakartokite šiuos veiksmus su kiekvienu elektroninių parašų reikalaujančiu procesu.  
4. Spustelėkite Įrašyti.

## <a name="create-a-custom-requirement-for-electronic-signatures"></a>Pasirinktinio elektroninių parašų reikalavimo kūrimas
1. Spustelėkite Naujas.
2. Pažymėkite arba išvalykite žymės langelį Būtinas parašas.
3. Lauke Pavadinimas įveskite proceso, kuriam būtinas elektroninis parašas, pavadinimą.
4. Lauke Lentelės pavadinimas spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
5. Sąraše suraskite ir pasirinkite lentelę, kurioje saugomi pasirašytini duomenys.
6. Sąraše spustelėkite saitą pasirinktoje eilutėje.
7. Lauke Lauko pavadinimas spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
8. Sąraše suraskite ir pasirinkite norimą stebėti lentelės lauką.
9. Sąraše spustelėkite saitą pasirinktoje eilutėje.
    * Nustatykite, kada reikalingas parašas.     Pasirinkite Visada, jei parašo reikalaujama, kada lauke pakeičiami duomenys.     Pasirinkite Tik, jei parašo reikalaujama tik esant tam tikroms sąlygoms. Jei pasirinksite Tik, taip pat turite pasirinkti vieną iš šių pasirinkčių: Kai įterpiamas įrašas, Kai atnaujinamas įrašas arba Kai panaikinamas įrašas.  
10. Spustelėkite Įrašyti.
11. Uždarykite puslapį.


