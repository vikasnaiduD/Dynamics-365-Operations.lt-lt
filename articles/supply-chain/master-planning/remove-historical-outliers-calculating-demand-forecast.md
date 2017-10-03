---
title: "Skaičiuodami poreikio prognozę iš praeities operacijų duomenų pašalinkite pašalines reikšmes"
description: "Šiame straipsnyje aprašoma, kaip iš praeities duomenų, kurie naudojami poreikio prognozei apskaičiuoti, pašalinti pašalines reikšmes. Pašalinę pašalines reikšmes, galite padidinti prognozės tikslumą."
author: roxanadiaconu
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: ReqDemPlanForecastParameters, ReqDemPlanOutlierQuerySetup
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations
ms.custom: 72621
ms.assetid: 88a964af-14eb-4c5c-945b-388e5908362c
ms.search.region: global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: Human Translation
ms.sourcegitcommit: d421b161216d700f7819f1da8c0ca8ad089b5670
ms.openlocfilehash: 72735c9e3fb4291076f0b577f45384dec319b2a7
ms.contentlocale: lt-lt
ms.lasthandoff: 05/25/2017

---

# <a name="remove-outliers-from-historical-transaction-data-when-calculating-a-demand-forecast"></a>Skaičiuodami poreikio prognozę iš praeities operacijų duomenų pašalinkite pašalines reikšmes

[!include[banner](../includes/banner.md)]


Šiame straipsnyje aprašoma, kaip iš praeities duomenų, kurie naudojami poreikio prognozei apskaičiuoti, pašalinti pašalines reikšmes. Pašalinę pašalines reikšmes, galite padidinti prognozės tikslumą.

Pašalinę pašalines reikšmes galite padidinti prognozės tikslumą. Ši užduotis nėra privaloma. Toliau pateikta proceso apžvalga.

1.  Norėdami atidaryti puslapį **Pašalinių reikšmių šalinimas**, kuriame, naudodami užklausą, galėtumėte pasirinkti šalintinas operacijas, spustelėkite **Bendrasis planavimas** &gt; **Sąranka** &gt; **Poreikio prognozė** &gt; **Pašalinių reikšmių šalinimas**.
2.  Pasirinkite įmonę, kuriai užklausa taikoma, tada įveskite pavadinimą ir aprašą. **Užklausos datos** laukas automatiškai nustatomas į dabartinę datą.
3.  Pažymėkite žymės langelį **Aktyv.**, kad iš praeities duomenų pašalintumėte operacijas, rastas naudojant užklausą. Šis parametras pradės veikti, kai kursite pagrindinę prognozę.
4.  Puslapyje **Pašalinių reikšmių šalinimo užklausa** galite pridėti, šalinti ir pasirinkti kriterijus, apibrėžiančius, kurios operacijos bus pašalintos skaičiuojant pagrindinę prognozę. Pvz., pasirinkite konkrečią prekę arba užsakymo operaciją, kurią norite pašalinti.
5.  Spustelėkite **Rodyti operacijas**. Puslapyje **Pašalinių reikšmių operacijos** išvardijamos operacijos, kurios atitinka jūsų užklausoje nurodytus kriterijus ir kurios apskaičiuojant poreikio prognozę bus pašalintos iš praeities duomenų.

**Pastaba:** taip pat galite sukurti užklausą, paremtą esama užklausa. Pasirinkite užklausą, kurią norite kopijuoti, tada spustelėkite **Dubliuoti**. Lauke **Užklausos data** identifikuojama versija. Užklausą galite naudoti tokią, kokia ji yra, arba galite spustelėti **Redaguoti užklausą** ir modifikuoti kriterijus. Neprivaloma: galite modifikuoti naujosios užklausos pavadinimą ir aprašą.

<a name="see-also"></a>Taip pat žiūrėkite
--------

[Įvadas į poreikio prognozes](introduction-demand-forecasting.md)

[Prognozės tikslumo stebėjimas](monitor-forecast-accuracy.md)



