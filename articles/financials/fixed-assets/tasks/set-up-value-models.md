--- 
title: Nustatyti knygas
description: "Šioje procedūroje parodoma, kaip kurti naują ilgalaikio turto knygą ir susieti ją su ilgalaikio turto grupe."
author: saraschi2
manager: AnnBe
ms.date: 10/11/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: a29cae6cdcd03903359a3a468243c6ad03c7adc6
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="set-up-books"></a>Nustatyti knygas

[!include[task guide banner](../../includes/task-guide-banner.md)]

Šioje procedūroje parodoma, kaip kurti naują ilgalaikio turto knygą ir susieti ją su ilgalaikio turto grupe. Joje naudojamas vaidmuo Buhalteris ir USMF juridinio subjekto demonstraciniai duomenys.


## <a name="create-a-book"></a>Knygos kūrimas
1. Pasirinkite Ilgalaikis turtas > Sąranka > Knygos.
2. Spustelėkite Naujas.
3. Lauke Knyga įveskite reikšmę.
4. Lauke Aprašas įveskite reikšmę.
    * Pasirinkus Skaičiuoti nusidėvėjimą, susijusi knyga bus įtraukta į nusidėvėjimo pasiūlymus. Jei parinktis nepasirinkta, turto knyga nebus automatiškai nudėvima.  
5. Lauke Skaičiuoti nusidėvėjimą pasirinkite Taip.
6. Lauke Nusidėvėjimo šablonas įveskite arba pasirinkite reikšmę.
    * Alternatyvus nusidėvėjimo šablonas taip pat vadinamas nusidėvėjimo perjungimo metodu. Į šį šabloną nusidėvėjimo pasiūlymas persijungs, kai alternatyvus šablonas apskaičiuos nusidėvėjimo sumą, kuri yra lygi numatytajam nusidėvėjimo šablonui arba už jį didesnė.  
    * Visiško nusidėvėjimo šablonas naudojamas neįprastas atvejais papildomai skaičiuojant turto nusidėvėjimą. Pavyzdžiui, galite tai naudoti norėdami įrašyti nusidėvėjimą įvykus gamtos katastrofai.  
    * Pasirinkus Kurti nusidėvėjimo koregavimus su pagrindo koregavimais, nusidėvėjimo koregavimai bus automatiškai sukurti atnaujinus turto vertę. Jei parinktis nepasirinkta, atnaujinta turto vertė turės įtakos tik tolimesniems nusidėvėjimo skaičiavimams.  
7. Lauke Kurti nusidėvėjimo koregavimus su pagrindo koregavimais pasirinkite Taip.
    * Pagal numatytuosius parametrus ilgalaikio turto knygos operacijos bus registruojamos DK. Galite išjungti knygos registravimo DK funkciją, nustatydami lauką Registruoti DK į parinktį Ne. Knygos, kurios neregistruojamos DK, paprastai naudojamos mokesčių registravimo tikslais. Taip suteikiama daugiau lankstumo naikinant ankstesnes turto knygos operacijas, nes jos nebuvo perkeltos į DK.  
    * Pagal numatytuosius parametrus registravimo sluoksnis nustatomas į parinktį Dabartinis sluoksnis, jei knyga registruojama DK, arba į parinktį Nė vienas, jei knyga neregistruojama DK. Jei reikia, kad šios knygos operacijos būtų registruojamos į kitą sluoksnį, atnaujinkite registravimo sluoksnį.  
8. Lauke Kalendorius įveskite arba pasirinkite reikšmę.
    * Išvestinių knygų operacijos bus registruojamos kitose knygose tuo pačiu metu. Galite kurti operacijas naudodami pagrindinę knygą – tada registravimo metu tikslios operacijų kopijos užregistruojamos išvestinėse knygose. Išvestinės knygos operacijos nėra perskaičiuojamos, todėl jos neturėtų būti naudojamos atliekant nusidėvėjimo operacijas.  

## <a name="associate-the-book-with-a-fixed-asset-group"></a>Knygos susiejimas su ilgalaikio turto grupe
1. Spustelėkite Ilgalaikio turto grupės.
2. Lauke Ilgalaikio turto grupė įveskite arba pasirinkite reikšmę.
3. Lauke Dėvėjimo laikas įveskite skaičių.
    * Atkreipkite dėmesį, kad lauko Nusidėvėjimo laikotarpiai reikšmė apskaičiuojama nustačius dėvėjimo laiką.  
    * Mokesčių tvarkymo tikslais galite pagal poreikį nustatyti nusidėvėjimo konvenciją.  


