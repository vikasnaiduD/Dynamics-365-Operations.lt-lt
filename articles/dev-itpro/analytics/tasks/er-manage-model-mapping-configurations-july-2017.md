--- 
title: "Modelių susiejimo konfigūracijų valdymas elektroninėse ataskaitose (ER)"
description: "Šie veiksmai paaiškina, kaip sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmenį turintis vartotojas gali valdyti elektroninių ataskaitų (ER) modelio susiejimus atskirose ER konfigūracijose."
author: NickSelin
manager: AnnBe
ms.date: 06/19/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 35fdc1e98897d449ce18fe38cc6b7896ca5c5278
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="manage-model-mapping-configurations-for-electronic-reporting-er"></a>Modelių susiejimo konfigūracijų valdymas elektroninėse ataskaitose (ER)

[!include[task guide banner](../../includes/task-guide-banner.md)]

Šie veiksmai paaiškina, kaip sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmenį turintis vartotojas gali valdyti elektroninių ataskaitų (ER) modelio susiejimus atskirose ER konfigūracijose. Šiame užduočių vedlyje kursite reikiamas pavyzdinės įmonės „Litware, Inc.“ ER konfigūracijas. Norėdami atlikti užduočių vedlio veiksmus, pirmiausia turite užbaigti užduočių vedlio „ER: konfigūracijos teikėjo kūrimas ir pažymėjimas aktyviu“ veiksmus. 

Kadangi įmonės dalijasi ER konfigūracijomis, galite baigti šį užduočių vedlį, naudodami jūsų pasirinktą įmonės duomenų rinkinį. Šio užduočių vedlio funkcijas galima naudoti, jei įdiegėte vieną iš tolesnių karštųjų pataisų: https://fix.lcs.dynamics.com/Issue/Resolved?kb=4012872, skirtą „Dynamics AX“ 7.0 versijai arba https://fix.lcs.dynamics.com/Issue/Resolved?kb=4012871, skirtą „Dynamics 365 for Operations“ versijai.

1. Pasirinkite Organizacijos administravimas > Darbo sritys > Elektroninės ataskaitos.
    * Patikrinkite, ar pavyzdinės įmonės „Litware, Inc.” konfigūracijos teikėjas yra galimas ir pažymėtas kaip aktyvus. Jei nematote šio konfigūracijos teikėjo, pirmiausia turite atlikti užduočių vedlio „Konfigūracijos teikėjo kūrimas ir pažymėjimas aktyviu” veiksmus.   

## <a name="add-a-new-er-model-configuration"></a>Įtraukti naują ER modelio konfigūraciją
1. Spustelėkite Ataskaitų konfigūracijos.
    * Pridėkite naują modelio konfigūraciją. Pavadinimas turi būti unikalus konfigūracijos medyje.  
2. Spustelėdami Kurti konfigūraciją, atidarykite išplečiamąjį dialogo langą.
3. Lauke Pavadinimas įrašykite „Duomenų modelio pavyzdys“.
    * Duomenų modelio pavyzdys  
4. Spustelėkite Sukurti konfigūraciją.
5. Spustelėkite Konstruktorius.
6. Spustelėdami Naujas atidarykite išplečiamąjį dialogo langą.
7. Lauke Pavadinimas įveskite Šaknis.
    * Šaknis  
8. Spustelėkite Pridėti.
9. Spustelėdami Naujas atidarykite išplečiamąjį dialogo langą.
10. Lauke „Pavadinimas“ įveskite „Įmonė“.
    * Įmonė  
11. Spustelėkite Pridėti.
12. Lauke Aprašymas įveskite tekstą, juridinio subjekto arba įmonės, kurioje vartotojas prisijungęs vykdymo metu, aprašymą. 
    * Juridinio subjekto arba įmonės, kurioje vartotojas prisijungęs vykdymo metu, aprašymas.  
13. Spustelėkite Šakninė nuoroda.
14. Spustelėkite GERAI.
15. Spustelėkite Įrašyti.
16. Uždarykite puslapį.
17. Spustelėkite keisti būseną.
18. Spustelėkite Baigti.
19. Spustelėkite GERAI.

## <a name="add-a-new-er-model-mapping-configuration"></a>Pridėkite naują ER modelio susiejimo konfigūraciją
1. Spustelėdami Kurti konfigūraciją, atidarykite išplečiamąjį dialogo langą.
2. Lauke Naujas įveskite „Modelio susiejimas, pagrįstas duomenų modeliu „Duomenų modelio pavyzdys“.
3. Lauke Pavadinimas įrašykite „Susiejimo pavyzdys‟.
    * Susiejimo pavyzdys  
4. Spustelėkite Sukurti konfigūraciją.
5. Išplėskite sekciją Išankstiniai reikalavimai.
    * Žinokite, kad išankstinių reikalavimų grupė „Įgyvendinimas“ pridėta automatiškai. Grupėje yra išankstinio reikalavimo komponentas, kuris nurodo pirminių duomenų modelio konfigūraciją ir yra pažymėtas kaip Įgyvendinimas. Tai reiškia, kad ši susiejimo modelio pavyzdžio konfigūracija skirta duomenų modelio „Duomenų modelio pavyzdys“ įgyvendinimui. Todėl šis komponentas privers ER atsisiųsti modelio susiejimo konfigūraciją „Susiejimo pavyzdys“ iš ER saugyklos kai bus atsisiunčiama modelio konfigūracija „Duomenų modelio pavyzdys“.   
6. Spustelėkite Konstruktorius.
    * Atkreipkite dėmesį, kad sukurto modelio susiejimo konfigūracijoje yra naujas tuščias susiejimas tokiu pačiu pavadinimu, kaip sukurta konfigūracija. Žinokite, kad kai pasirinktoje pirminio modelio konfigūracijoje yra modelio susiejimų, jie bus nukopijuoti į naują modelio susiejimo konfigūraciją.   
7. Spustelėkite Konstruktorius.
8. Medyje pasirinkite „Dynamics 365 for Operations\Table“.
9. Spustelėkite „Įtraukti šaknį“.
10. Lauke „Pavadinimas“ įveskite „Įmonė“.
    * Įmonė  
11. Lauke „Lentelė“, įveskite „CompanyInfo“.
    * CompanyInfo  
12. Spustelėkite GERAI.
13. Medyje išplėskite „Company“.
14. Medyje išplėskite „Company\find()“.
15. Medyje pasirinkite „Company\find()\Name“.
16. Spustelėkite Susieti.
17. Spustelėkite Įrašyti.
18. Uždarykite puslapį.
19. Uždarykite puslapį.
20. Veiksmų srityje spustelėkite Konfigūracijos.
21. Spustelėkite Vartotojo parametrai.
22. Lauke Paleisti parametrus pasirinkite Taip.
23. Spustelėkite GERAI.
24. Spustelėkite Redaguoti.
25. Lauke Paleisti juodraštį pasirinkite Taip.

## <a name="add-a-new-er-format-configuration"></a>Įtraukite naują ER formato konfigūraciją
1. Medyje pasirinkite „Sample data model“.
2. Spustelėdami Kurti konfigūraciją, atidarykite išplečiamąjį dialogo langą.
3. Lauke Naujas įveskite „Formatas, pagrįstas duomenų modeliu „Duomenų modelio pavyzdys“.
4. Lauke Pavadinimas įrašykite „Formato pavyzdys‟.
    * Formato pavyzdys  
5. Spustelėkite Sukurti konfigūraciją.
6. Spustelėkite Konstruktorius.
7. Spustelėdami Įtraukti šakninį elementą atidarykite išplečiamąjį dialogo langą.
8. Medyje pasirinkite „Tekstas \ Eilutė‟.
9. Spustelėkite GERAI.
10. Spustelėkite skirtuką „Susiejimas“.
11. Medyje išplėskite „modelis‟.
12. Medyje pasirinkite „model\Company“.
13. Spustelėkite Susieti.
14. Spustelėkite Įrašyti.
15. Uždarykite puslapį.
    * Vykdykite sukurto formato projekto versiją bandymams.  
16. Spustelėkite Vykdyti.
    * Versijos FastTab spustelėkite Vykdyti.  
17. Spustelėkite GERAI.
    * Peržiūrėkite išvestį, kurioje yra įmonės pavadinimas, kurioje vartotojas, kuris vykdo šią formato konfigūraciją, prisijungęs. Žinokite, kad sukurtą modelio susiejimo konfigūraciją naudoja ši formato konfigūracija, nes yra tik viena konfigūracija, kurioje yra reikalingi modelio susiejimai.   

## <a name="add-alternative-er-model-mapping-configuration"></a>Pridėkite alternatyvią ER modelio susiejimo konfigūraciją
1. Medyje pasirinkite „Sample data model“.
2. Spustelėdami Kurti konfigūraciją, atidarykite išplečiamąjį dialogo langą.
3. Lauke Naujas įveskite „Modelio susiejimas, pagrįstas duomenų modeliu „Duomenų modelio pavyzdys“.
4. Lauke Pavadinimas įrašykite „Susiejimo pavyzdys (alternatyva)“.
    * Susiejimo pavyzdys (alternatyva)  
5. Spustelėkite Sukurti konfigūraciją.
6. Spustelėkite Konstruktorius.
7. Spustelėkite Konstruktorius.
8. Medyje pasirinkite „Dynamics 365 for Operations\Table“.
9. Spustelėkite „Įtraukti šaknį“.
10. Lauke „Pavadinimas“ įveskite „Įmonė“.
    * Įmonė  
11. Lauke „Lentelė“, įveskite „CompanyInfo“.
    * CompanyInfo  
12. Spustelėkite GERAI.
13. Spustelėkite Redaguoti.
14. Medyje pasirinkite „Eilutė \ SUJUNGTI“.
15. Spustelėkite „Įtraukti funkciją“.
16. Medyje išplėskite „Company“.
17. Medyje išplėskite „Company\find()“.
18. Medyje pasirinkite „Company\find()\Name“.
19. Spustelėkite „Įtraukti duomenų šaltinį“.
20. Lauke „Formulė“ įveskite reikšmę.
    * CONCATENATE(Company.'find()'.Name, ";",  
21. Medyje pasirinkite „Company\find()\Company(DataArea)“.
22. Spustelėkite „Įtraukti duomenų šaltinį“.
23. Lauke „Formulė“ įveskite reikšmę.
    * CONCATENATE(Company.'find()'.Name, ";", Company.'find()'.DataArea)  
24. Spustelėkite Įrašyti.
25. Uždarykite puslapį.
26. Spustelėkite Įrašyti.
27. Uždarykite puslapį.
28. Uždarykite puslapį.
29. Lauke Paleisti juodraštį pasirinkite Taip.

## <a name="use-an-existing-er-model-mapping-configuration"></a>Naudokite esamą ER modelio susiejimo konfigūraciją
1. Medyje pasirinkite „Sample data model\Sample format“.
2. Spustelėkite Vykdyti.
    * Atkreipkite dėmesį, kad pasirinktos ER formato konfigūracijos projekto versijos vykdyti negalima, nes yra daugiau kaip viena modelio susiejimo konfigūracija, prieinama neapibrėžtam duomenų modeliui, kuris buvo pasirinktas kaip veikiančio ER formato duomenų šaltinis.   
    * toliau jūs apibrėšite alternatyvią modelio susiejimo konfigūraciją, kaip tą, iš kurios bus naudojami modelio susiejimai kaip duomenų šaltiniai veikiančiam ER formatui.   
3. Medyje pasirinkite „Sample data model\Sample mapping (alternative)“.
4. Lauke Numatytoji modelio susiejimo reikšmė pasirinkite Taip.
5. Medyje pasirinkite „Sample data model\Sample format“.
6. Spustelėkite Vykdyti.
7. Spustelėkite GERAI.
    * Atkreipkite dėmesį, kad numatytąją modelio susiejimo konfigūraciją naudoja ši formato konfigūracija elektroniniam dokumentui generuoti (sukurtoje išvestyje yra įmonės kodas).  


