---
title: Apskaitos paskirstymai
description: "Šiame straipsnyje pateikiama informacija apie apskaitos paskirstymus ir aprašomos pasirinktys, kurias galima apdoroti. Apskaitos paskirstymai naudojami šaltinio dokumento piniginėms sumoms paskirstyti į konkrečias DK sąskaitas."
author: twheeloc
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: AccountingDistribution
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.custom: 17231
ms.assetid: 9030355d-8e6e-408b-9e7d-7b346eaa652c
ms.search.region: Global
ms.author: peakerbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 52cb689723584c862d85fa51a643b42096372a29
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="accounting-distributions"></a>Apskaitos paskirstymai

[!include[banner](../includes/banner.md)]


Šiame straipsnyje pateikiama informacija apie apskaitos paskirstymus ir aprašomos pasirinktys, kurias galima apdoroti. Apskaitos paskirstymai naudojami šaltinio dokumento piniginėms sumoms paskirstyti į konkrečias DK sąskaitas. 

Apskaitos paskirstymai yra visą programą apimantis pajėgumas, kurį naudoja ir išplečia kiekvienas šaltinio dokumentas, pvz., pirkimo užsakymas, tiekėjo SF, išlaidų ataskaita ir laisvos formos SF. Pagal numatytuosius nustatymus, numatytasis apskaitos paskirstymas generuojamas kiekvienai šaltinio dokumento eilutei ir piniginei sumai, ir tam tikromis sąlygomis jį galima modifikuoti. 

> [!Note] 
> Tam tikri dokumentai taip pat palaiko antraštės dokumento pinigines sumas, pvz., užsakymų ir SF išlaidas. 

Bendrosios apskaitos paskirstymo galimybės suteikia tokias apskaitos paskirstymų apdorojimo parinktis:

-   **Paskirstyti sumas** – peržiūrėkite ir modifikuokite apskaitos paskirstymus konkrečioje dokumento antraštėje arba eilutėje ir visose antrinėse eilutėse, pvz., mokesčių ar rinkliavų.
    -   Svarbiausių piniginės sumos paskirstymų (pirminių paskirstymų) pagrindinės sąskaitos ir finansinės dimensijos gali būti redaguojamos tiesiogiai tinklelyje esančiame segmentuotų įrašų valdiklyje. Išplėstinė kaina yra tipinis tokio pirminio paskirstymo pavyzdys.
    -   Paskirstymo sumos priklauso nuo dokumento valiutos termino. Paprastai ši valiuta yra operacijos valiuta. Apskaitos ir ataskaitų valiutos sumos generuojamos kaip papildomos knygos apskaitos dalis.
    -   Paskirstymai rodo apskaitos datą ir apskaitos įvykį. Paprastai apskaitos įvykiui būna nustatyta reikšmė **Nėra**, kol dokumentas dar neužregistruotas / neįtrauktas į žurnalą. Tuo metu apskaitos įvykis tampa **Pradinis**. Užregistravę paskirstymus, jų modifikuoti negalėsite.
    -   Pirminiams paskirstymams gali būti įgalintas mygtukas **Skaidyti**. **Skaidyti** sugeneruoja naujus apskaitos paskirstymus, o skaidymas gali būti atliekamas pagal procentinę išraišką, sumą arba kiekį.
    -   Mygtuką**Paskirstyti tolygiai** galima naudoti kartu su **Skaidyti**, kad suma būtų automatiškai tolygiai paskirstyta tarp visų paskirstymų.
    -   Gali būti įgalintas pirminių paskirstymų mygtukas **Nustayti iš naujo**, kai yra daugiau nei vienas paskirstymas. **Nustatyti iš naujo** atšaukia rankiniu būdu padarytas paskirstymo modifikacijas panaikindamas visus esamus paskirstymus ir iš naujo sugeneruodamas numatytuosius paskirstymus.
    -   Bet koks antrinis paskirstymas, pvz., nuolaida, mokestis ir PVM, visada atliekamas po pirminio paskirstymo. Pirminį ir antrinį ryšį galite peržiūrėti pasirinkę **Nuoroda** &gt; **Pirminė informacija**.
    -   Gali būti redaguojama ir antrinių paskirstymų pagrindinė sąskaita ir finansinė dimensija.
    -   Apskaitos paskirstymų finansinės dimensijos atitinka numatytąjį modelį, kad dokumentą galima išplėsti. Jei norite sužinoti daugiau, žr. susijusius straipsnius.
    -   Nuokrypių paskirstymai gali būti generuojami gretinimo scenarijuose, pvz., tiekėjo SF gretinimas su pirkimo užsakymu. Gretinimo ryšius tarp apskaitos paskirstymo galite peržiūrėti pasirinkę **Nuoroda** &gt; **Dokumento informacija**.
    -   Pasirodo mygtukas **Taisyti** ir jis yra įgalintas dokumentams, palaikantiems taisymus. **Taisyti** sukuria naujus paskirstymus. Pirma, sukuriami paskirstymai, kurie atšaukia pradinius paskirstymus. Šių paskirstymų modifikuoti negalima. Tada sukuriami nauji teisingo apskaitos paskirstymai. Šiuos paskirstymus galima modifikuoti, jei modifikuoti galima pradinius paskirstymus.
    -   Mygtukas**Projekto informacija** įgalinamas kaip plėtinys, kai eilutė yra susijusi su projektu. Projekto apskaitos paskirstymai leidžia modifikuoti tokią informaciją, kaip lėšų skyrimo šaltinis ir eilutės ypatybė.
    -   Galite peržiūrėti dabartinio dokumento apskaitos būseną – **Nuoroda**. Būsena yra viso dokumento ir nurodo, ar dokumentas yra nebaigtas ar baigtas.
-   **Peržiūrėti paskirstymus** – peržiūrėkite visų dokumento eilučių ir piniginių sumų apskaitos paskirstymus. Negalite modifikuoti apskaitos paskirstymų iš šio rodinio.


Daugiau informacijos žr. dalyje [Apskaitos paskirstymai ir papildomos knygos žurnalo įrašai, skirti laisvos formos SF](accounting-distributions-subledger-journal-entries-vendor-invoices.md)



