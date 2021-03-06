---
title: "Skambučių centro tęstinumo programos nustatymas"
description: "Šiame straipsnyje aprašyta, kaip nustatyti skambučių centro tęstinumo programą."
author: josaw1
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-365-retail
ms.technology: 
ms.search.form: MCROrderParameters
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 16081
ms.assetid: 426a9be7-a931-4780-b372-e06f6083dd60
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 0fa2c5aaf6953eed75729017cca8cf3c2220e80d
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="set-up-a-continuity-program-for-a-call-center"></a>Skambučių centro tęstinumo programos nustatymas

[!include[banner](includes/banner.md)]


Šiame straipsnyje aprašyta, kaip nustatyti skambučių centro tęstinumo programą.

Tęstinės programos, kuri taip pat vadinama pasikartojančio užsakymo programa, klientai reguliariai gauna produkto siuntas pagal iš anksto nustatytą grafiką. Kiekvienoje siuntoje gali būtų skirtingas produktas, pvz., knygų klubo mėnesio knyga, arba tas pats produktas gali būti siunčiamas pakartotinai. Norėdami nustatyti tęstinumo programą, turite atlikti toliau nurodytus veiksmus.

1.  Nustatykite tęstinumo parametrus puslapyje **Skambučių centro parametrai**.
2.  Sukurkite tęstinumo programą, kurioje būtų nurodyta išsami informacija, pvz., mokėjimo grafikas, siuntimo laikas ir tai, ar apmokama iš anksto. Taip pat turite įtraukti produktų, kurie įtraukti į tęstinę programą, sąrašą. Kiekvienas produktas gauna įvykio ID numerį, kuris priskiriamas iš eilės pradedant nuo 1. Įvykio ID nurodo tvarką, kuria siunčiami produktai.
    -   Jei klientai gauna skirtingą produktą kiekvienoje siuntoje, produktai siunčiami iš eilės pagal jų įvykio ID, pradedant nuo dabartinio įvykio.
    -   Jei klientai gauna tą patį produktą kiekvienoje siuntoje, sąraše yra tik vienas produktas, kuriam priskirtas vienas įvykio ID. Tas pats įvykis vyksta kelis kartus. Galite nurodyti, kiek kartų kartoti kiekvieną įvykį.

3.  Sukurkite pirminį produktą, kuris nurodo tęstinumo programą, kurią sukūrėte atlikdami 2 užduotį. Jei įtrauksite šį produktą į pardavimo užsakymą, bus atidarytas puslapis **Tęstinumas**. Tada galėsite naudoti tą puslapį, kad sukurtumėte faktinį tęstinumo užsakymą. Pirminis produktas nenurodo atskirų produktų, kuriuos klientas gauna kiekvienoje siuntoje.

Nustatę tęstinumo programą, kaip aprašyta aukščiau, klientui galite sukurti tęstinumo užsakymą. Be to, gali tekti atlikti toliau nurodytas papildomas priežiūros užduotis.

-   **Atnaujinti dabartinio tęstinumo įvykio laikotarpį** – nustatykite paketinę užduotį, sistemai nurodančią dabartinio įvykio laikotarpį.
-   **Sukurti antrinius tęstinumo užsakymus** – iš pirminio tęstinumo užsakymo sukurkite antrinius užsakymus.
-   **Apdoroti tęstinumo mokėjimus** – apdorokite su tęstinumo pardavimo užsakymais susietų mokėjimų sąskaitas ir pranešimus.
-   **Išplėsti tęstinumo eilutes** (jei reikia) – padidinkite tęstinumo įvykio kartojimo kartų skaičių. Tada siuntų kartojimą galima išplėsti už skambučių centro parametrų lauke **Tęstinumo kartojimo slenkstis** nustatytos ribos.
-   **Atlikti tęstinumo atnaujinimą** (jei reikia) – sinchronizuokite tęstinumo programos ir pirminių tęstinumo pardavimo užsakymų pakeitimus.
-   **Uždaryti pirmines tęstinumo eilutes ir užsakymus** – uždarykite tęstinumo užsakymus.





