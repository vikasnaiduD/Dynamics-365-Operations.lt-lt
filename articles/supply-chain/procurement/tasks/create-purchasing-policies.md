--- 
title: Kurti pirkimo strategijas
description: "Šioje procedūroje parodoma, kaip kurti pirkimo strategijas ir suderinti jas su pirkimo verslo procesais."
author: mkirknel
manager: AnnBe
ms.date: 08/23/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: c2b3a66443394f5bfbe51b6685513281025d68fd
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="create-purchasing-policies"></a>Kurti pirkimo strategijas

[!include[task guide banner](../../includes/task-guide-banner.md)]

Šioje procedūroje parodoma, kaip kurti pirkimo strategijas ir suderinti jas su pirkimo verslo procesais. Prieš kurdami pirkimo strategijas turite nustatyti pirkimo strategijos parametrus. Galima kurti, modifikuoti ir nurašyti pirkimo strategiją, bet pirkimo strategijos negalima naikinti. Šią procedūrą paprastai atlieka pirkimo vadovas. Šią procedūrą galite atlikti demonstracinių duomenų įmonėje USMF arba su savo duomenimis.


## <a name="set-up-policy-parameters"></a>Strategijos parametrų nustatymas
1. Pasirinkite Pirkimo strategijos.
2. Spustelėkite Parametrai.
    * Strategijos pirmumo taisyklės taikomos skirtingiems jūsų organizacijos lygiams. Rodomi organizacijos vienetai priklauso nuo jūsų organizacijos hierarchijos ir nuo to, kuriems hierarchijos lygiams priskirta paskirtis Įsigijimo vidinė kontrolė. Pvz., organizacijoje gali būti juridiniai subjektai, išlaidų centrai, regionai ir padaliniai, bet galbūt tik kai kuriems iš jų priskirta hierarchijos paskirtis Įsigijimo vidinė kontrolė. Pagal numatytuosius parametrus galimas organizacijos tipas Įmonė.  
3. Spustelėkite skirtuką Strategijos taisyklės tipo parametrai.
4. Medyje pasirinkite Pirkimo strategija\Pirkimo paraiškos kontrolės taisyklė.
    * Strategijos taikymo pirmumo tvarką galite nurodyti strategijos lygiu. Tačiau naudodami kai kurių tipų strategijas galite nepaisyti atskirų tipų strategijos taisyklių pirmumo tvarkos. Pvz., galite nustatyto tokią pirkimo strategijų pirmumo tvarką: išlaidų centras, padalinys, įmonė. Taikydami katalogo strategijos taisyklę galite nustatyti tokią pirmumo tvarką: padalinys, išlaidų centras, įmonė. Galite pakeisti katalogo strategijos taisyklės pirmumo tvarką. Kai darbuotojas sukuria paraišką, rodomas katalogas priklauso nuo strategijų, susijusių su darbuotojo padaliniu, tada – su jo išlaidų centru ir su įmone.  
    * Jei nurodytas daugiau nei vienas organizacinis lygis, galite naudoti rodyklę Aukštyn / Žemyn, kad nustatytumėte taisyklės Pirkimo paraiškos kontrolė pirmumo tvarką.  
5. Uždarykite puslapį.

## <a name="create-a-new-policy"></a>Kurti naują strategiją
1. Spustelėkite Naujas.
2. Lauke Pavadinimas surinkite reikšmę.
3. Lauke Aprašas įveskite reikšmę.
    * Viena pirkimo strategija gali būti taikoma tik vienai organizacijos hierarchijai. Pvz., viena hierarchija vadinasi „Geografinė“, o kita – „Padalinys“, o joms priskirtos pirkimo strategijos skiriasi.  
    * Pasirinkite organizaciją, kuriai turėtų būti taikoma strategija.  
4. Norėdami įtraukti pasirinktą organizaciją, spustelėkite rodyklę.
    * Galite pakartoti šį procesą, norėdami įtraukti daugiau organizacijų.  

## <a name="add-a-policy-rule"></a>Įtraukti strategijos taisyklę
1. Sąraše Strategijos taisyklės tipas pasirinkite paraiškos paskirties taisyklę.
    * Sukursite taisyklę, kuri numatytąją paraiškos paskirtį nustato į tipą Suvartojimas, bet suteikia galimybę jį pakeisti į tipą Papildymas.  
2. Spustelėkite Kurti strategijos taisyklę.
3. Lauke Leisti neautomatiškai perrašyti pasirinkite Taip.
4. Spustelėkite Uždaryti.
    * Dabar galite nustatyti kitas pirkimo strategijos taisykles.   Atkreipkite dėmesį, tipe Strategijos taisyklė negali būti persidengiančių taisyklių, kurios vienu metu yra aktyvios vienoje įsigijimo strategijoje.  
5. Uždarykite puslapį.
6. Uždarykite puslapį.


