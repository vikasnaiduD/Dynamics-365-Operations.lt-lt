--- 
title: "Apdoroti mokėjimo grąžinimus"
description: "Ši procedūra nurodo, kaip konvertuoti patvirtintus ir apdorotus grąžinimus klientams į kredito pažymas."
author: omulvad
manager: AnnBe
ms.date: 11/10/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: omulvad
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 7e0a5d044133b917a3eb9386773205218e5c1b40
ms.openlocfilehash: 791ec304b9ea7c49fbea506d73c4daffd4478739
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="process-rebates-for-payment"></a>Apdoroti mokėjimo grąžinimus

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ši procedūra nurodo, kaip konvertuoti patvirtintus ir apdorotus grąžinimus klientams į kredito pažymas. Šį vadovą galite naudoti demonstracinėje įmonėje USMF. Išankstinė šio vadovo sąlyga – turėti vieną ar daugiau grąžinimo pretenzijų, kurių būsena yra „Žymėti“. Jei naudojate USMF, prieš šį vadovą rekomenduojama įvykdyti „Generuoti ir apdoroti kliento grąžinimus“.


## <a name="convert-rebate-claims-to-credit-note"></a>Konvertuoti grąžinimo pretenzijas į kredito pažymą
1. Eikite į „Visi klientai“.
2. Sąraše raskite ir pasirinkite norimą įrašą.
3. Sąraše spustelėkite saitą pasirinktoje eilutėje.
4. Veiksmų srityje spustelėkite Rinkti.
5. Spustelėkite „Sudengti operacijas“.
6. Spustelėkite Funkcijos.
7. Spustelėkite „Grąžinimo programa“.
    * Puslapyje „Grąžinimai“ surašytos grąžinimo pretenzijos, kurias apdorojote kliento grąžinimų darbo srityje ir kurių būsena yra „Žymėti“.    
8. Spustelėkite Redaguoti.
    * Lauke „Žymėti“ nustatykite žymes pretenzijose, kurias norite įtraukti į kredito pažymą.   
9. Spustelėkite Funkcijos.
10. Spustelėkite „Sukurti kredito pažymą“.
    * Rodomas pranešimas, kuris jus informuoja, kad žurnalas buvo užregistruotas (tai gautinų sumų suvartojimo žurnalas, kaip nurodyta puslapyje „Gautinų sumų parametrai“). Tai lemia, kad tikrosios atsakomybės (kredito) suma perkeliama į kliento balansą. Tai reiškia, kad kliento sąskaita kredituojama, o grąžinimo kaupimo sąskaita debetuojama.  
11. Uždarykite puslapį.
12. Spustelėkite Atšaukti.
    * Tai atnaujina puslapį, kad matytumėte atnaujinimus.  
13. Veiksmų srityje spustelėkite Rinkti.
14. Spustelėkite „Sudengti operacijas“.
    * Atkreipkite dėmesį, kad į kliento balansą įtraukta operacija su neigiama suma, kuri atitinka bendrą grąžinimo sumą, be sąskaitos faktūros nuorodos.   
15. Spustelėkite Atšaukti.


