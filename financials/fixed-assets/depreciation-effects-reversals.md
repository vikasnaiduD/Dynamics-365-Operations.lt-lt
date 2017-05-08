---
title: "Nusidėvėjimo poveikis su atšaukimais"
description: "Šiame straipsnyje aptartos galimos ilgalaikio turto operacijos atšaukimo pasekmės."
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AssetTrans
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 2961
ms.assetid: 63a3ac92-c321-4379-a86a-b1b14915f340
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b41901d573e977a89fcd1a7c1ebf7185e162c654
ms.openlocfilehash: 292186b17406851e40917225cf0c1b8c8e98c654
ms.lasthandoff: 03/31/2017


---

# <a name="depreciation-effects-with-reversals"></a>Nusidėvėjimo poveikis su atšaukimais

[!include[banner](../includes/banner.md)]


Šiame straipsnyje aptartos galimos ilgalaikio turto operacijos atšaukimo pasekmės. 

Galite atšaukti ilgalaikio turto operacijas ir su ilgalaikiu turtu susietas operacijas. Atšauktą operaciją taip pat galite anuliuoti. 

Atšaukite arba anuliuokite galite operaciją, kuri nebuvo paskutinė operacija, registruota turto knygoje. Pirmiausia turėtumėte nustatyti, ar po operacijos, kurią atšaukiate, buvo užregistruota kokių nusidėvėjimo operacijų. Taip yra todėl, nes, atšaukiant operaciją, nusidėvėjimas neperskaičiuojamas. Todėl po atšaukimo nusidėvėjimas dažnai pervertinamas ar nuvertinamas, kaip parodyta pavyzdžiuose. 

Kad užtikrintumėte, kad, atšaukiant operaciją, nusidėvėjimas teisingas, netęskite atšaukimo, jeigu gaunate pranešimą, kad nusidėvėjimas nebus skaičiuojamas iš naujo. Geriau pirmiausia atšaukite nusidėvėjimo operaciją, kuri užregistruota po operacijos, kurią bandote atšaukti, tada tęskite atšaukimą. Nebūsite įspėti apie nusidėvėjimo perskaičiavimus ir galėsite tęsti atšaukimą. 

Toliau pateiktuose pavyzdžiuose rodomi skaičiavimai, kurie atliekami, jei tęsiate nepaisydami pranešimo ir pirmiausia neatšaukę nusidėvėjimo operacijų.

## <a name="example-1-depreciation-is-overstated"></a> 1 pavyzdys: nusidėvėjimas pervertintas
Turtas nustatytas su 5 metų naudojimu ir tiesiogiai proporcingu nusidėvėjimu (60 nusidėvėjimo laikotarpių). Šiame pavyzdyje nusidėvėjimas pervertintas.
#### <a name="asset-transaction-history"></a>Turto operacijų retrospektyva

| Data       | Operacijos tipas                                                          | Suma                                    |
|------------|---------------------------------------------------------------------------|-------------------------------------------|
| Sausio 1  | Įsigijimas                                                               | 59 000,00                                 |
| Sausio 1  | Įsigijimo koregavimas                                                    | 1000,00                                  |
| Sausio 31 | Nusidėvėjimas (sukurtas naudojant pasiūlymą vienam nusidėvėjimo laikotarpiui) | 1 000,00Skaičiavimas: balansinė vertė (59 000 + 1 000) / likusių nusidėvėjimo laikotarpių skaičius (60) |

#### <a name="reversal-action"></a>Atšaukimo veiksmai

| Data      | Operacijos tipas                | Suma    |
|-----------|---------------------------------|-----------|
| Sausio 1 | Įsigijimo derinimo atšaukimas | -1000,00 |

#### <a name="depreciation-effect"></a>Nusidėvėjimo efektas

| Data        | Operacijos tipas        | Suma                                                                                |
|-------------|-------------------------|---------------------------------------------------------------------------------------|
| Vasario 28 | Nusidėvėjimas (pasiūlymas) | 983,05Skaičiavimas: balansinė vertė (59 000 – 1 000 nusidėvėjimas) / likusių nusidėvėjimo laikotarpių skaičius (59) |

Nusidėvėjimas parvertintas 16,95 (1000–983,05).

## <a name="example-2-depreciation-is-understated"></a> 2 pavyzdys: Nusidėvėjimas nuvertintas
Turtas nustatytas su 5 metų naudojimu ir tiesiogiai proporcingu nusidėvėjimu (60 nusidėvėjimo laikotarpių). Šiame pavyzdyje nusidėvėjimas nuvertintas.
#### <a name="asset-transaction-history"></a>Turto operacijų retrospektyva

| Data       | Operacijos tipas                                                          | Suma                                      |
|------------|---------------------------------------------------------------------------|---------------------------------------------|
| Sausio 1  | Įsigijimas                                                               | 59 000,00                                   |
| Sausio 1  | Vertės mažinimas                                                     | 1000,00                                    |
| Sausio 31 | Nusidėvėjimas (sukurtas naudojant pasiūlymą vienam nusidėvėjimo laikotarpiui) | 966,67Skaičiavimas: balansinė vertė (59 000 – 1 000) / likusių nusidėvėjimo laikotarpių skaičius (60) |

#### <a name="reversal-action"></a>Atšaukimo veiksmai

| Data      | Operacijos tipas               | Suma    |
|-----------|--------------------------------|-----------|
| Sausio 1 | Vertės mažinimo atšaukimas | -1000,00 |

#### <a name="depreciation-effect"></a>Nusidėvėjimo efektas

| Data        | Operacijos tipas        | Suma                                                                                       |
|-------------|-------------------------|----------------------------------------------------------------------------------------------|
| Vasario 28 | Nusidėvėjimas (pasiūlymas) | 983,62Skaičiavimas: balansinė vertė (59 000 – 966,67 nusidėvėjimas) / likusių nusidėvėjimo laikotarpių skaičius (59) |

Nusidėvėjimas nuvertintas 16,95 (983,62–966,67).



<a name="see-also"></a>Taip pat žiūrėkite
--------

[Ilgalaikio turto nusidėvėjimas](fixed-asset-depreciation.md)



