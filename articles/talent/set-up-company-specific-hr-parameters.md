---
title: "Konkrečios įmonės personalo parametrų nustatymas"
description: "Kai kurie modulio Personalas (HR) parametrai naudojami keliose įmonėse, o kiti – konkrečioje įmonėje. Šiame straipsnyje paaiškinama, kaip nustatyti konkrečios įmonės HR parametrus."
author: rschloma
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-365-talent
ms.technology: 
ms.search.form: HRMParameters
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Core, Operations, Talent
ms.custom: 51941
ms.assetid: 2cfb061a-a616-4bf9-9d98-9cde00039eec
ms.search.region: Global
ms.author: shielas
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Talent July 2017 update
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: aca20b7a9a56ecef88b466324527650cf6fe34d2
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="set-up-company-specific-hr-parameters"></a>Konkrečios įmonės personalo parametrų nustatymas

[!include[banner](includes/banner.md)]


Kai kurie modulio Personalas (HR) parametrai naudojami keliose įmonėse, o kiti – konkrečioje įmonėje. Šiame straipsnyje paaiškinama, kaip nustatyti konkrečios įmonės HR parametrus.

Personalo parametrams nustatyti naudojami du puslapiai. Jei parametrai yra bendrai naudojami keliose įmonėse, galite naudoti puslapį **Bendrai naudojami žmogiškųjų išteklių parametrai**. Jei parametrai skirti konkrečiai įmonei (kitaip tariant, parametrai taikomi prie vienai įmonei), naudokite puslapį **Personalo parametrai**. Puslapyje **Personalo parametrai** parametrai suskirstyti į šešis toliau pateiktus skirtukus.

-   Bendra
-   Įdarbinimas – sprendime „Dynamics 365 for Talent‟ jo nėra
-   Kompensacija
-   Numeravimai
-   Nedarbingumo dėl ligos ar slaugymo aktas (FMLA)
-   Darbuotojų savitarna

Kiekviename skirtuke yra informacijos, susijusios su viena įmone. Skirtuko **Bendra** parametrai apibrėžia informacijos apie neatvykimą, sužalojimus ir ligas bei naujus darbuotojus, rodymą. Šio skirtuko parametrai taip pat nustato kai kuriuos numatytuosius įrašus, rodomus, kai dirbate. Tiksliau sakant, šiame skirtuke galite pasirinkti spalvą, kurią norite taikyti atviroms neatvykimų operacijoms, nurodyti stiliaus aprašą, naudojamą ataskaitoms, aktyvinti integravimą tarp mokymosi kursų ir neatvykimų registravimo bei pasirinkti neatvykimo kodą, naudojamą šiam integravimui valdyti. Taip pat galite nurodyti, kiek laiko sužeidimo ir ligos atvejų incidentai turėtų būti laikomi bei nurodyti numatytąjį identifikavimo numerį, rodomą, kai pasamdomas naujas darbuotojas. 

Skirtuko **Įdarbinimas** parametrai apibrėžia dokumentų tipus, kurie naudojami korespondencijoje, automatiškai siunčiamoje pretendentams, ir įdarbinimo projektą, kuris naudojamas neprašytiems prašymams (nesusijusiems su konkrečiu įdarbinimo projektu). Nurodytas skirstymo pagal terminus laikotarpis nustato įdarbinimo projektus, įtrauktus į išklotinę **Suskirstyti pagal terminus projektai**, esančią darbo srityje **Įdarbinimo valdymas**. Nurodytas prašymo pateikimo termino įspėjimo laikotarpis yra naudojamas įdarbinimo projektams, kurių prašymo pateikimo terminas artėja, rodyti išklotinėje **Prašymo pateikimo terminas artėja**, esančioje darbo srityje **Įdarbinimas**. 

Skirtuko **Kompensacija** nustatymai apibrėžia, ar vartotojai turi patvirtinti, kad nori išsaugoti informaciją fiksuotosios arba kintamosios atlyginimo dalies planą. Jei pažymėsite žymės langelį **Įgalinti tikrinimo įrašymą**, uždarydami su kompensacija susijusį puslapį vartotojai gaus pranešimą, kuriame klausiama, ar jie nori įrašyti įrašą. Kai kuriuose kompensacijos valdymo puslapiuose vartotojai informacijos naikinti negali. Todėl, reikalaudami, kad vartotojai patvirtintų, jog jie nori įrašyti informaciją, galėsite riboti informaciją, kuri įrašoma, bet kurios vėliau negalima panaikinti. Jei žymės langelis **Aktyvinti įrašymo tvirtinimą** nepažymėtas, įrašai visada įrašomi iš karto, galimai anksčiau nei tai padaro vartotojas. Jei naudojate našumo valdymą, skirtuke **Kompensacija** taip pat galite pasirinkti vertinimo modelį, kuris bus naudojamas vietoje modelio, našumo vertinimo metu priskirto kompensavimo planams. 

### <a name="previously-released-functionality"></a>Anksčiau išleistos funkcijos
Skirtuko **Numeracija** parametrai nurodo sekas, naudojamas ID automatiškai priskirti elementams personalo srityje, pvz., prašymams, neatvykimo registracijoms, kompensavimo proceso rezultatams, atvejų numeriams, kursams ir kursų darbotvarkei. Norėdami prižiūrėti numeracijų nuorodas ir kodus, naudokite **Numeracijos** sąrašo puslapį (spustelėkite **Organizacijos administravimas** &gt; **Numeracijos** &gt; **Numeracijos**).

### <a name="if-youre-using-dynamics-365-for-talent"></a>Jei naudojate „Dynamics 365 for Talent‟
Skirtuko **Numeracija** parametrai nurodo sekas, naudojamas ID automatiškai priskirti elementams personalo srityje, pvz., prašymams, neatvykimo registracijoms, kompensavimo proceso rezultatams, atvejų numeriams, kursams ir kursų darbotvarkei. Norėdami tvarkyti numeracijų nuorodas ir kodus, naudokite sąrašo puslapį **Numeracijos** (spustelėkite **Sistemos administravimas** &gt; **skirtuką Saitai** &gt; **Numeracijos** &gt; **Numeracijos**). 

Skirtuko **FMLA** parametrai nurodo, kiek valandų ir kokį laikotarpį darbuotojas turi išdirbęs tam, kad galėtų gauti FMLA išmokas, ir darbo pradžios datą, kuri naudojama siekiant nustatyti darbo trukmę. Parametrai taip pat apibrėžia darbuotojams skirtą FMLA valandų skaičių FMLA atostogų kalendorių, pagal kurį skaičiuojama, kiek FMLA valandų darbuotojai išnaudojo. Skirtuką **FMLA** gali naudoti tik įmonės, esančios Jungtinėse Amerikos Valstijose. 

**Pastaba:** išdirbtų valandų skaičius negali viršyti 1 250, o įdarbinimo trukmė negali viršyti 12 mėnesių. Šios didžiausios galimos reikšmės atitinka Jungtinių Amerikos Valstijų federalinę teisę. Galiausiai skirtuko **Darbuotojų savitarna** parametrai apibrėžia informaciją, kurią vadybininkas gali įvesti savo darbuotojų vardu.

<a name="see-also"></a>Taip pat žiūrėkite
--------

[Kelių juridinių subjektų personalo parametrų nustatymas](set-up-hr-parameters-across-legal-entities.md)




