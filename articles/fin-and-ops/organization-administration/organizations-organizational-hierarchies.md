---
title: "Organizacijos ir organizacijų hierarchijos"
description: "Organizacija yra grupė žmonių, kurie dirba kartu vykdydami verslo procesą arba siekdami tikslo. Organizacijos hierarchijos nurodo ryšius tarp organizacijų, kurios sudaro jūsų verslą."
author: sericks007
manager: AnnBe
ms.date: 08/18/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: OMHierarchyManager
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.custom: 17291
ms.assetid: 76b7ca45-93d4-45cc-b191-66ee63afa1fd
ms.search.region: Global
ms.author: sericks
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 4f8afc37e8d69b06622176d4f6cfb3ff06a0ab54
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="organizations-and-organizational-hierarchies"></a>Organizacijos ir organizacijų hierarchijos

[!include[banner](../includes/banner.md)]


Organizacija yra grupė žmonių, kurie dirba kartu vykdydami verslo procesą arba siekdami tikslo. Organizacijos hierarchijos nurodo ryšius tarp organizacijų, kurios sudaro jūsų verslą.

<a name="organizations"></a>Organizacijos
-------------

Programoje „Microsoft Dynamics 365 for Finance and Operations“ galima nurodyti šių tipų vidines organizacijas: juridinius subjektus, valdymo vienetus ir komandas.

Visos vidinės organizacijos yra objekto **Šalis** tipai. Todėl šios organizacijos naudoja adresų knygelę, kurioje saugomi adresai ir kontaktinė informacija. Šalis, kuri gali būti asmuo arba organizacija, gali priklausyti vienai ar daugiau adresų knygelių.
### <a name="legal-entities"></a>Juridiniai subjektai

Juridinis subjektas yra organizacija, turinti registruotą ar įteisintą teisinę struktūrą. Juridiniai subjektai gali sudaryti teisines sutartis ir privalo paruošti išrašus apie savo veiklą. 

Įmonė yra juridinio subjekto tipas. Šiame „Microsoft Dynamics 365 for Finance and Operations“ leidime įmonės yra vienintelė juridinių subjektų rūšis, kurią galima kurti, o kiekvienas juridinis subjektas susiejamas su įmonės ID. Šis susiejimas taikomas todėl, kad kai kuriose duomenų modelių funkcinėse programos srityse naudojamas įmonės ID arba DataAreaId. Dėl duomenų saugumo, šiose funkcinėse srityse naudojimas ribojamas įmonės viduje. Vartotojai gali gauti prieigą tik prie tos įmonės duomenų, prie kurios yra prisiregistravę.

### <a name="operating-units"></a>Valdymo vienetai

Valdymo vienetas yra organizacija, kuri yra naudojama ekonominiams ištekliams valdyti ir verslo veiklos procesams skirstyti. Valdymo vienete žmonės turi maksimaliai išnaudoti negausius išteklius, pagerinti procesus ir atsiskaityti už savo našumą. 

Programoje „Microsoft Dynamics 365 for Finance and Operations“ valdymo vienetų tipai apima išlaidų centrus, verslo struktūros vienetus, vertės srautus, padalinius ir mažmeninės prekybos kanalus. Tolesnėje lentelėje pateikta daugiau informacijos apie kiekvieną valdymo vieneto tipą.

| Valdymo vienetų tipai | Aprašymas         | Paskirtis      |
|---------------------|---------------------|--------------|
| Išlaidų centras         | Valdymo vienetas, kurio vadovai yra atsakingi už į biudžetą įtrauktas ir faktines išlaidas.                                                      | Naudojama verslo procesų, apimančių juridinius subjektus, valdymo ir veikimo kontrolei.                                         |
| Verslo struktūros vienetas       | Pusiau savarankiškas valdymo vienetas, sukurtas strateginiams verslo tikslams pasiekti.                                                        | Naudojama finansinėms ataskaitoms, pagrįstoms pramonės šakomis ar produkto eilutėmis, kurias organizacija prižiūri nepriklausomai nuo juridinių subjektų. |
| Vertės srautas        | Valdymo vienetas, kontroliuojantis vieną ar daugiau gamybos srautų.                                                                                  | Dažniausiai naudojama „lean manufacturing“ siekiant valdyti veiklas ir srautus, būtinus tiekiant klientams produktą ar paslaugą.  |
| Padalinys          | Valdymo vienetas, nurodantis organizacijos, kuri atlieka konkrečią užduotį, pvz., pardavimą ar apskaitą, kategoriją ar funkcinę sritį. | Naudojama informuoti apie funkcines sritis. Padaliniui gali būti priskirta pelno ir nuostolio atsakomybė, be to, jį gali sudaryti išlaidų centrų grupė.   |
| Mažmeninės prekybos kanalas      | Valdymo vienetas, nurodantis plytų ir skiedinio parduotuvę, internetinę parduotuvę ar internetinę prekyvietę.                                          | Naudojama vieno ar kelių juridinių subjektų vienos ar daugiau parduotuvių valdymo ir veikimo kontrolei.                                  |

### <a name="teams"></a>Komandos

Komanda yra organizacija, kurios nariai bendrai prisiima atsakomybę, dalijasi palūkanomis ir turi bendrą tikslą. Komandų negalima naudoti organizacijos hierarchijose.

<a name="organizational-hierarchies"></a>Organizacijų hierarchijos
--------------------------

Norėdami peržiūrėti įvairius verslo aspektus, nustatykite organizacijos hierarchijas. Pavyzdžiui, galima nustatyti juridinių subjektų hierarchiją, skirtą mokesčių, juridinėms ar privalomosioms ataskaitoms kurti. Nustatykite hierarchiją, pagrįstą valdymo vienetais, kad būtų kuriamos finansinės informacijos, kurios nebūtina pateikti, bet kuri naudojama vidaus kontrolei, ataskaitos. Pavyzdžiui, galima kurti pirkimo hierarchiją, skirtą valdyti pirkimo strategijas, taisykles ir verslo procesus. 

Programoje „Microsoft Dynamics 365 for Finance and Operations“ kiekvienai hierarchijai priskiriama paskirtis. Hierarchijos paskirtis apibrėžia organizacijų, kurias galima įtraukti į hierarchiją, tipus. Paskirtis taip pat apibrėžia taikymo scenarijus, kuriuose hierarchija gali būti naudojama. 

Organizacijos hierarchijoje galite bendrai naudoti parametrus, strategijas ir operacijas. Organizacija gali perimti arba nepaisyti jos pirminės organizacijos parametrų. Tačiau bendrai naudojami bendrieji duomenys, pvz., produktai ir adresų knygelės, taikomi visai organizacijai ir jų negalima nepaisyti atskiroms organizacijoms. Organizacijos ir hierarchijos kuriamos tik kruopščiai planuojant. Daugiau informacijos apie hierarchijos konstruktorių žr. [Organizacijos hierarchijos planavimas](plan-organizational-hierarchy.md).






