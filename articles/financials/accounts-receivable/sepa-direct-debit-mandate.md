---
title: "SEPA tiesioginio debeto įgaliojimo nustatymas"
description: "Bendros mokėjimų eurais erdvės (SEPA) tiesioginis debetas leidžia kreditoriui surinkti lėšas iš kliento banko sąskaitos, jei klientas kreditoriui suteikė pasirašytą įgaliojimą."
author: ShivamPandey-msft
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: CustParameters
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.custom: 59491
ms.assetid: 653a135f-c515-4ae3-9da2-82b5e1f103b5
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 5b9afeb24692010ca5de33156f372d86f167161e
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="set-up-sepa-direct-debit-mandate"></a>SEPA tiesioginio debeto įgaliojimo nustatymas

[!include[banner](../includes/banner.md)]


Bendros mokėjimų eurais erdvės (SEPA) tiesioginis debetas leidžia kreditoriui surinkti lėšas iš kliento banko sąskaitos, jei klientas kreditoriui suteikė pasirašytą įgaliojimą. Įgaliojimas, kurį pasirašo klientas, įgalioja kreditorių surinkti mokėjimą ir nurodo kliento bankui jį išmokėti. Ši tema išdėstyta taip, kad parodytų SEPA tiesioginio debeto įgaliojimų nustatymo procesą.

## <a name="prerequisites"></a>Būtinieji komponentai
Pateiktoje lentelėje parodytos būtinosios sąlygos, kurias reikia įvykdyti prieš pradedant.

| Kategorija       | Būtinoji sąlyga                                                                                                                                              |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| Šalis/regionas | Pagrindinis juridinio subjekto adresas turi būti šioje šalyje / regione: Austrija, Belgija, Nyderlandai, Ispanija, Italija, Prancūzija arba Vokietija. |

1. Nustatykite tiesioginio debeto įgaliojimų numeraciją. Kiekvienas tiesioginio debeto įgaliojimas turi turėti unikalų numerį. Naudodami puslapį **Numeracijos** sukurkite tiesioginio debeto įgaliojimų numeraciją. Naudosite šį identifikatorių, kad priskirtumėte numeraciją tiesioginio debeto įgaliojimų sistemai puslapyje **Gautinų sumų parametrai**.

2. Nustatykite tiesioginio debeto įgaliojimų Gautinų sumų parametrus. Puslapį **Gautinų sumų parametrai** naudokite tiesioginio debeto įgaliojimų parametrams nustatyti. Norėdami nustatyti parametrus, skirtuke **Tiesioginis debetas** pagal poreikį pakeiskite numatytuosius parametrus. Tada skirtuke **Numeracijos** atnaujinkite lauką **Tiesioginio debeto įgaliojimo ID** pagal anksčiau nustatytą numeraciją.

3. Nustatykite tiesioginio debeto įgaliojimų mokėjimo būdą. Turite nustatyti tiesioginio debeto įgaliojimų mokėjimo būdą. Naudojate šį mokėjimo būdą pateikdami SF užklausas, kad būtų generuojami tiesioginio debeto mokėjimai. Naudokite **Mokėjimo būdų** puslapį, kad nustatytumėte mokėjimo būdą. Norėdami nustatyti tiesioginio debeto įgaliojimų mokėjimo būdą, turite atlikti toliau nurodytus papildomus mokėjimo būdo veiksmus.

-   Lauke **Mokėjimo tipas** pasirinkite **Elektroninis mokėjimas**.
-   Pasirinktinai: jei tikitės, kad kiekvienas jūsų klientas turės kelis įgaliojimus, lauke **Laikotarpis** pasirinkite **Sąskaita faktūra**. Kiekvienai sąskaitai faktūrai bus sukurtas atskiras mokėjimas ir kiekvienas mokėjimas naudos tai sąskaitai faktūrai nurodytą įgaliojimą.
-   Pasirinkite parinktį **Reikalauti įgaliojimo**, kad sukurtumėte mokėjimus naudojant tiesioginio debeto įgaliojimus. Parinktis **Reikalauti įgaliojimo** prieinama tik tada, jei **Mokėjimo tipo** lauke pasirenkate **Elektroninis mokėjimas**.

Taip pat žr.

[Tiesioginio debeto apžvalga](sepa-direct-debit-overview.md) 

[Kurti kliento tiesioginio debeto įgaliojimą](tasks/create-direct-debit-mandate-customer.md) 


