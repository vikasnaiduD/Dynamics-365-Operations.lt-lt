--- 
title: Nustatyti gamybos eigos modelius
description: "Gamybos eigos modeliai apibūdina, kaip apskaičiuojamas ir tvarkomas pažangiosios gamybos darbo elementų pajėgumas."
author: cvocph
manager: AnnBe
ms.date: 11/11/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: conradv
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 9b947a02be981155053e33a4ef20e19bf2a194a5
ms.openlocfilehash: 3da0b5c4fc50136a98017e37b65afea9f8ec7b38
ms.contentlocale: lt-lt
ms.lasthandoff: 07/27/2017

---
# <a name="define-production-flow-models"></a>Nustatyti gamybos eigos modelius

[!include[task guide banner](../../includes/task-guide-banner.md)]

Gamybos eigos modeliai apibūdina, kaip apskaičiuojamas ir tvarkomas pažangiosios gamybos darbo elementų pajėgumas. Todėl gamybos eigos modelio apibrėžimas yra būtinas darbo elementų apibrėžimo komponentas. Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.


## <a name="define-a-production-flow-model"></a>Apibrėžkite gamybos eigos modelį. 
1. Eikite į Gamybos kontrolė > Sąranka > „Lean“ gamybos eiga > Gamybos eigos modeliai.
2. Spustelėkite Naujas.
3. Lauke Gamybos eigos modelis įveskite gamybos eigos modelio ID.
4. Lauke Modelio tipas pasirinkite pasirinktį.
    * Yra dviejų tipų modeliai: Našumo tipas ir Valandų tipas. Našumo tipo darbo elementų, kuriems naudojamas šis gamybos eigos modelis, pajėgumas išreiškiamas ir apskaičiuojamas produktų kiekiu. Našumo tipo darbo elementų, kuriems naudojamas šis gamybos eigos modelis, pajėgumas išreiškiamas ir apskaičiuojamas valandomis. Atkreipkite dėmesį, kad šios ypatybės negalima pakeisti į esamą gamybos eigos modelį. Kai darbo elementas turi pajėgumo rezervavimų, gamybos eigos modelio tipo keisti negalima.  
5. Įveskite EPE ciklo dienų skaičių.
    * Intervalu aprašomas laikotarpis, kai kiekviena gamybos eigos ar darbo elemento parengta dalis bus gaminama bent kartą. Kuo trumpesnis EPE ciklas, tuo lankstesnis gamybos procesas. Jei EPE ciklas = 0, visą poreikį galima patenkinti per tą pačią dieną. EPE ciklas naudojamas planuoti pažangiosios gamybos proceso užduotis. Planuojant užduotį su darbo elementu, kurio EPE ciklas = 5, planavimo procesas ieškos darbo langelio pajėgumo, kurio Termino data – EPE ciklas (5 dienos iki termino) siekiant užtikrinti, kad produktą galima pagaminti per šį ciklą. Produkto atsargų gamybos laikas paprastai yra lygus arba didesnis negu susijusio gamybos proceso EPE ciklas.  
6. Lauke Planavimo laikotarpio tipas pasirinkite pasirinktį.
    * Kai darbo elementas turi pajėgumo rezervavimų, planavimo laikotarpio tipo keisti negalima. Šiam konkrečiam darbo elementui galima pasirinkti tik laikotarpio tipo gamybos eigos modelius.  
7. Lauke Planavimo laiko riba įveskite skaičių.
    * Planavimo laiko riba apibūdina skaičių dienų, kai pajėgumo rezervavimus susijusiems darbo elementams galima atlikti. Planavimo laiko riboje įveskite dienų skaičių.   „Kanban“ proceso užduotys, nepatenkančios į šį laikotarpį, nebuvo suplanuotos automatinio planavimo būdu. Planavimo laiko ribos paprastai yra du kartus didesnės už vidutinį atsargų gavimo laiką produktams, pagamintiems per produktų eigą arba darbo elementą. EPE ciklas negali trukti daugiau nei pusę planavimo laiko ribos.     
8. Lauke Pajėgumo trūkumo reakcija pasirinkite pasirinktį.
    * Galimos parinktys: atidėti – atidedama visa planavimo įvykio paklausa kitą pasiekiamą gamybos datą su galimu našumu. Atšaukti – baigti automatinį planavimo įvykio planavimą ir palikti susijusias užduotis.   Įtraukti į pageidaujamą datą – planuoti pageidaujamas užduotis užklausų laikotarpiui. Tokiu būdu perkraunamas šios datos langelis ir iš planuotojo reikalaujama peržiūrėti ir rankiniu būdu atlikti veiksmus.   Paskirstyti turimiems laikotarpiams – skirtingos planavimo įvykio užduotys paskirstomos visoms pasiekiamoms gamybos datoms pradedant nuo pirmos pasiekiamos datos. Minimalus paskirstymo kiekis yra „kanban“ užduoties kiekis. Paskirstymas priskiria minimalų planavimo kiekį („kanban“ kiekį) kiekvienai datai su pakankamu našumu.  

