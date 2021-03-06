--- 
title: "Pardavimo sutarčių vykdymas"
description: "Ši procedūra nurodo, kaip įvykdyti pardavimo sutartį, su ja susiejus pardavimo užsakymus."
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
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: f0894bf962c139c2e9e4c9f8d1589fd933afcedb
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="fulfill-sales-agreements"></a>Pardavimo sutarčių vykdymas

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ši procedūra nurodo, kaip įvykdyti pardavimo sutartį, su ja susiejus pardavimo užsakymus. Šią procedūrą galite vykdyti demonstracinėje duomenų įmonėje USMF arba su savo duomenimis. Prieš paleisdami šį vadovą, įsitikinkite, kad turite galiojančią „Produkto vertės įsipareigojimas“ tipo pardavimo sutartį. Taip pat galite paleisti užduočių vadovą, pavadintą „Kurti pardavimo sutartis“.  




## <a name="release-a-sales-order-from-the-agreement"></a>Išleisti pardavimo užsakymą iš sutarties
1. Eikite į Pardavimas ir rinkodara > Pardavimo sutartys > Pardavimo sutartys.
2. Sąraše atidarykite sutartį, pagal kurią norite išleisti užsakymą.
3. Srityje Veiksmas spustelėkite Pardavimo sutartis.
4. Spustelėkite išleidimo užsakymas.
    * Kaip nurodo tekstas puslapio Kurti paleidimo viršuje, informacija, reikalinga pardavimo užsakymo eilutėse skirsis atsižvelgiant į tai, ar sutartis yra pagrįsta kiekiu ar verte.  
    * Šiame vadove pateikiamos sutarties tipas „Produkto vertės įsipareigojimas“. Todėl šio puslapio skyrius Eilutės yra tuščias. Jei įsipareigojimas pagrįstas kiekiu, eilutės informacija nukopijuojama iš sutarties.  
5. Spustelėkite Kurti.
    * Pranešimas informuoja, kad pardavimo užsakymas sukurtas. Kadangi užsakyme eilučių nėra, turite įtraukti užsakymo eilučių informaciją, norėdami užbaigti išleidimo procesą.   
6. Uždarykite puslapį.
7. Uždarykite puslapį.
8. Eikite į Pardavimas ir rinkodara > Pardavimo užsakymai > Visi pardavimo užsakymai.
9. Sąraše raskite ir atidarykite užsakymą, kuris ankstesnėje užduotyje buvo sukurtas kaip užsakymo išleidimo rezultatas.
10. Spustelėkite Pridėti eilutę.
11. Lauke Prekės numeris spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
12. Lauke Prekės numeris, įveskite arba pasirinkite prekę, kuri nurodyta susijusioje pardavimo sutartyje.
13. Lauke Kiekis įveskite skaičių.
    * Įsitikinkite, kad įvedate kiekį, su kuriuo grynoji suma bus mažesnė nei susijusios pardavimo sutarties vertė.  
    * Atkreipkite dėmesį, kad dėl to, jog pardavimo užsakymas yra susietas su sutartimi, sutartas nuolaidos procentas taikomas užsakymo eilutei.  
14. Spustelėkite eilutę „Atnaujinti“.
15. Spustelėkite „Pridėta“.
    * Puslapyje Pridėta sutartis rodomas ID ir sutarties, iš kurios eilutė išleista, sąlygos.  
16. Uždarykite puslapį.
17. Veiksmų srityje spustelėkite Bendra.
18. Spustelėkite Pridėta pardavimo sutartis.
19. Išplėskite skyrių Eilutės informacija.
20. Spustelėkite skirtuką Įvykdymas.
    * Skirtuke Įvykdymas rodoma suvestinė visų pardavimo užsakymo eilučių, kurios susietos su šiuo įsipareigojimo, jų įvykdymo būsena ir suma arba kiekis, kuris dar nepaleistas.   
21. Uždarykite puslapį.
22. Uždarykite puslapį.
23. Uždarykite puslapį.

## <a name="apply-sales-agreement-in-the-order-process"></a>Taikyti pardavimo sutartį užsakymo procese
1. Eikite į Pardavimas ir rinkodara > Pardavimo užsakymai > Visi pardavimo užsakymai.
2. Spustelėkite Naujas.
3. Lauke Kliento sąskaita spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
4. Sąraše raskite ir pasirinkite klientą, nurodyta pardavimo sutartyje.
5. Sąraše spustelėkite saitą pasirinktoje eilutėje.
6. Išplėskite skyrių Bendra.
7. Lauke Pardavimo sutarties ID spustelėję išplečiamąjį mygtuką atidarykite peržvalgą.
8. Sąraše spustelėkite saitą pasirinktoje eilutėje.
9. Spustelėkite Taip.
10. Spustelėkite GERAI.
11. Sąraše pažymėkite pasirinktą eilutę.
12. Lauke Prekės numeris spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
13. Lauke Prekės numeris, įveskite arba pasirinkite prekę, kuri nurodyta susijusioje pardavimo sutartyje.
14. Sąraše spustelėkite saitą pasirinktoje eilutėje.
15. Spustelėkite Įrašyti.
16. Veiksmų srityje spustelėkite Paimti ir pakuoti.
17. Spustelėkite Registruoti važtaraštį.
18. Išplėskite skyrių Parametrai.
19. Lauke Registravimas pasirinkite Taip.
20. Spustelėkite GERAI.
21. Spustelėkite GERAI.
22. Veiksmų srityje spustelėkite Bendra.
23. Spustelėkite Pridėta pardavimo sutartis.
24. Spustelėkite skirtuką Įvykdymas.


