---
title: Savikainos elemento dimensijos
description: "Kaip vienas iš pagrindinių ramsčių savikainos apskaitoje norint kategorizuoti ir sekti išlaidų srautą naudojamos savikainos elemento dimensijos."
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: CAMDimension
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, Operations, UnifiedOperations
ms.custom: 223204
ms.assetid: 1eda0e62-760b-4737-9dfd-3c3c38d80c1a
ms.search.region: global
ms.author: yuyus
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: c06f4f636a58ac8068415b1291bd8668e7a977d5
ms.contentlocale: lt-lt
ms.lasthandoff: 05/25/2017

---

# <a name="cost-element-dimensions"></a>Savikainos elemento dimensijos

[!include[banner](../includes/banner.md)]


Kaip vienas iš pagrindinių ramsčių savikainos apskaitoje norint kategorizuoti ir sekti išlaidų srautą naudojamos savikainos elemento dimensijos. 

Savikainos elementas sąskaitų plane atitinka su savikaina susijusį elementą. Iš esmės jis gali būti bet kokio tipo žemiausio verslo lygio elementas, į kurį gali būti nukreiptas išlaidų srautas. Savikainos elementai kaip sąvokos intervalas nuo DK sąskaitų iki visų su savikaina susijusių išteklių. Šiuo metu išlaidų apskaita palaiko DK sąskaitas.

## <a name="two-types-of-cost-elements"></a>Dviejų tipų savikainos elementai
Yra dviejų tipų savikainos elementai: pirminiai savikainos elementai ir antriniai savikainos elementai. Toliau pateikiamoje lentelėje aprašomi šių dviejų tipų skirtumai.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Pirminiai savikainos elementai</strong></td>
<td><strong>Antriniai savikainos elementai</strong></td>
</tr>
<tr class="even">
<td>Pirminiai savikainos elementai atitinka išlaidų srautą iš finansinės apskaitos į išlaidų apskaitą. Savikainos elemento struktūra atitinka pelno ir nuostolio sąskaitos struktūrą didžiojoje knygoje, kai savikainos elementas gali atitikti pagrindinę sąskaitą. Ne visos pagrindinės sąskaitos būtinai turi būti pateikiamos kaip savikainos elementai priklausomai nuo verslo poreikių. Pirminių savikainos elementų pavyzdžiai:
<ul>
<li>Parduotų prekių savikaina (COG)</li>
<li>Netiesioginės medžiagų išlaidos</li>
<li>Personalo išlaidos</li>
<li>Energijos išlaidos</li>
</ul></td>
<td>Antriniai savikainos elementai atitinka vidinių išlaidų srautą, nes šios išlaidos sukurtos ir naudojamos tik savikainos apskaitoje. Jie naudojami norint užtikrinti, kad būtų galima atsekti išlaidų šaltinį. Šie savikainos elementai naudojami savikainos paskirstymuose ir skaičiuojant papildomas išlaidas. Antrinių savikainos elementų pavyzdžiai:
<ul>
<li>Gamybos išlaidos</li>
<li>Pridėtinės išlaidos už gamybą, medžiagas ir rinkodarą</li>
</ul></td>
</tr>
</tbody>
</table>

## <a name="cost-element-dimensions-and-cost-element-dimension-members"></a>Savikainos elemento dimensijos ir savikainos elemento dimensijos nariai
Savikainos elementai vadinami *savikainos elemento dimensijos*. Atskiros dimensijos vertės vadinamos *savikainos elemento dimensijos nariai*. Pavyzdžiui, jūs turite JAV sąskaitų plano struktūrą (COA), kuri yra jūsų privalomųjų ataskaitų pagrindas. Ši COA naudojama kaip savikainos elemento dimensija. Sąskaitas, kurios yra pirminiai savikainos elementai, savikainos apskaitoje atitinka savikainos elemento dimensijos nariai. Toliau pateikiamoje ekrano nuotraukoje pavaizduotas pagrindinių sąskaitų pavyzdys, kai pagrindinės sąskaitos yra savikainos elemento dimensija su savo faktinėmis pagrindinėmis sąskaitomis, kurios yra savikainos elemento dimensijos nariai. 

[![savikainos elemento dimensijos](./media/cost-element-dimensions.png)](./media/cost-element-dimensions.png)

## <a name="import-cost-element-dimension-members-through-data-connectors"></a>Savikainos elemento dimensijos narių importavimas naudojant duomenų jungtis
Norėdami supaprastinti savikainos apskaitos savikainos elemento dimensijos narius, kad galėtumėte gauti pirminės savikainos elementus iš vienos ar kelių šaltinio sistemų, galite naudoti iš anksto parengtas duomenų jungtis arba savo pasirinktas jungtis.

## <a name="implementation-considerations"></a>Diegimo aplinkybės
Kadangi savikainos elementai atitinka žemiausią savikainos informacijos lygį, diegdami savikainos elementų struktūrą turėtumėte įsitikinti, kad pateikti visi savikainos elementai, kurių reikia norint paruošti vadovybės ataskaitą. Gali būti sunku rasti išlaidų kontrolei tinkantį išlaidų elementų skaičių. Turint tūkstančius išlaidų elementų gali būti sunku valdyti kiekvieną išlaidų elementą atskirai. Arba galite grupuoti išlaidų elementus ir valdyti išlaidų kontrolę sudėtiniu lygmeniu.



