---
title: "Banko derinimo gretinimo taisyklių nustatymas"
description: "Šioje temoje aiškinama, kaip nustatyti derinimo gretinimo taisykles ir derinimo gretinimo taisyklių rinkinius, kad būtų lengviau atlikti banko derinimo procesą. Derinimo gretinimo taisyklės – tai rinkinys kriterijų, naudojamų filtruojant banko išrašo eilutes ir banko dokumento eilutes, kai vykdomas derinimo procesas."
author: twheeloc
manager: AnnBe
ms.date: 10/27/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: BankReconciliationMatchRule, BankReconciliationMatchRuleSet
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.custom: 12971
ms.assetid: b5073f83-31dc-404f-af42-3fd84a02a7c6
ms.search.region: Global
ms.author: leguo
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 93438840123f02dd36927e044ff5ddbe60a76176
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="set-up-bank-reconciliation-matching-rules"></a>Banko derinimo gretinimo taisyklių nustatymas

[!include[banner](../includes/banner.md)]


Šioje temoje aiškinama, kaip nustatyti derinimo gretinimo taisykles ir derinimo gretinimo taisyklių rinkinius, kad būtų lengviau atlikti banko derinimo procesą. Derinimo gretinimo taisyklės – tai rinkinys kriterijų, naudojamų filtruojant banko išrašo eilutes ir banko dokumento eilutes, kai vykdomas derinimo procesas.

Galite nustatyti derinimo gretinimo taisykles ir derinimo gretinimo taisyklių rinkinius, kad būtų lengviau atlikti banko derinimo procesą. Derinimo gretinimo taisyklė – tai kriterijų rinkinys, naudojamas vykdant derinimo procesą, norint filtruoti banko išrašo eilutes ir „Microsoft Dynamics 365 for Finance and Operations, Enterprise edition“ banko operacijos eilutes. Norėdami nustatyti derinimo gretinimo taisykles, naudokite puslapį **Derinimo gretinimo taisyklės**. Galite nustatyti daugiau nei vieną gretinimo taisyklę ir pyslapyje **Derinimo gretinimo taisyklių rinkiniai** sukurti derinimo gretinimo taisyklių rinkinį. 

> [!NOTE] 
> Banko derinimo gretinimo taisyklės naudojamos, jei derinate elektroninį banko išrašą naudodamiesi išankstiniu banko derinimu. 

Puslapyje **Derinimo gretinimo taisyklės** galite pasirinkti, kokie veiksmai ir pasirinkimo kriterijai naudojami vykdant gretinimo taisyklę. Grupėje **Veiksmai** pasirinkite, koks veiksmas bus atliekamas vykdant gretinimo taisyklę derinimo proceso metu.  

> [!NOTE] 
> Rodomi laukai priklauso nuo to, kokią parinktį pasirinkote.

|                                    |                                                                                                                                                                                                                                                                                                               |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Veiksmas**                         |                                                                                                                                                                                                                                                                                                               | **Pasirinkus veiksmą galimi pasirinkimo kriterijai**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Sugretinti su banko dokumentu**       | Kurdami kriterijus nurodykite, kaip bus gretinami banko dokumentai ir banko išrašo eilutės, kai vykdoma puslapio **Banko suderinimo darbalapis** gretinimo taisyklė. Operacijų eilutės atrenkamos pagal papildomus „FastTab“ skirtukuose nustatytus kriterijus.                                | **1 veiksmas: apibrėžkite gretinimo taisyklę** – pasirinkite kriterijus, nurodančius, kurie banko išrašai turi būti gretinami su „Finance and Operations“ banko operacijomis. **2 veiksmas (pasirinktinai): pasirinkite išrašo eilutes, pagal kurias turi būti vykdomos gretinimo taisyklės:** pritaikykite filtrą, nurodantį, pagal kurią išrašo eilutę vykdyti taisykles.                                                                                                                                                                                                                                                                                                               |
| **Išvalyti atšaukimo išrašo eilutes** | Kurdami kriterijus nurodykite, kaip bus gretinami banko dokumentai ir banko išrašo eilutės, kai vykdoma puslapio **Banko suderinimo darbalapis** gretinimo taisyklė. Ši parinktis naudojama, kai dėl banko klaidos importuotame banko išraše yra dvi banko išrašo eilutės, kurias reikia derinti. | **1 veiksmas**:**rasti atšaukimo išrašo eilutes**– įtraukite pasirinkimo kriterijų, pagal kuriuos pasirenkamos atšaukimo banko išrašo eilutės. Pavyzdžiui, norėdami pasirinkti tik čekius, lauke Laukas pasirinkite **Banko operacijos kodas**, lauke **Operatorius** pasirinkite pliuso ženklą (+) ir lauke Reikšmė įveskite **Čekiai**. **2 veiksmas: rasti pirminio išrašo eilutes** – galite pridėti pasirinkimo kriterijų, pagal kuriuos banko dokumento eilutės bus gretinamos su banko išrašo eilutėmis. **3 veiksmas: rasti „Finance and Operations“ banko operacijas** – galite įtraukti pasirinkimo kriterijų, pagal kuriuos „Finance and Operations“ banko operacijos bus gretinamos su banko išrašų eilutėmis. |
| **Žymėti naujas operacijas**          | Kurdami kriterijus nurodykite, kaip puslapyje **Banko suderinimo darbalapis** turėtų būti pažymėtos naujos operacijos, kai vykdoma gretinimo taisyklė.                                                                                                                                                                 | **1 veiksmas: rasti išrašo eilutes**– įtraukite pasirinkimo laukų, kurie nurodytų, kurios puslapio **Banko suderinimo darbalapis** banko išrašo eilutės turėtų būti pasirinktos. **2 veiksmas: rasti „Finance and Operations‟** – galite įtraukti pasirinkimo kriterijų, pagal kuriuos būtų ieškoma banko dokumentų eilučių. Jei nerandamas joks banko dokumentas, išrašo eilutė bus pažymėta kaip nauja operacija.                                                                                                                                                                                                                                             |

 







