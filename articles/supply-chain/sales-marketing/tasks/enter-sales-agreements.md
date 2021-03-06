--- 
title: "Įvesti pardavimo sutartis"
description: "Ši procedūra nurodo, kaip kurti pardavimo sutartį, kuri jūsų klientus įpareigoja pirkti nustatytą produktų kiekį per tam tikrą laikotarpį, suteikiant jiems specialias nuolaidas."
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
ms.search.industry: Service industries
ms.author: omulvad
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 8c11164f7edb8e05b93f3c58b9707c0bf2482228
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="enter-sales-agreements"></a>Įvesti pardavimo sutartis

[!include[task guide banner](../../includes/task-guide-banner.md)]

Ši procedūra rodo, kaip kurti pardavimo sutartį, kuria vienas iš jūsų klientų įsipareigoja pirkti produktą už

sutartą sumą per tam tikrą laiką už specialias nuolaidas. Šią procedūrą galite vykdyti demonstracinėje duomenų įmonėje USMF arba su savo duomenimis.


## <a name="set-up-sales-agreement-header"></a>Pardavimo sutarties eilutės nustatymas
1. Eikite į Pardavimas ir rinkodara > Pardavimo sutartys > Pardavimo sutartys.
2. Spustelėkite Naujas.
3. Lauke Kliento sąskaita spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
4. Sąraše raskite ir pasirinkite norimą įrašą.
5. Sąraše spustelėkite saitą pasirinktoje eilutėje.
6. Lauke Pardavimo sutarčių klasifikacija spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
7. Sąraše spustelėkite saitą pasirinktoje eilutėje.
8. Išplėskite skyrių Bendra.
9. Lauke Numatytasis įsipareigojimas pasirinkite „Produkto vertės įsipareigojimas“.
    * Įsipareigojimo tipas yra privalomas kriterijus, kurį turite priskirti sutarčiai, kad nustatytumėte, kaip sutartis bus įvykdyta. Naudojant keturis iš anksto nustatytus tipus galima nustatyti kliento įsipareigojimo tikslą, kuris išreiškiamas kaip kiekis arba vertė. Kiekio įsipareigojimo tipą galima taikyti tik konkrečiam produktui, bet verte grįstus tipus galima taikyti parduodant konkrečius ir nekonkrečius produktus.  
10. Lauke Galiojimo data nustatykite ateities datą, kurią sutartis nustos galioti.
11. Spustelėkite GERAI.

## <a name="set-up-product-value-commitment-lines"></a>Produkto vertės įsipareigojimo eilučių nustatymas
1. Spustelėkite Pridėti eilutę.
2. Lauke Prekės numeris spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.
3. Sąraše raskite ir pasirinkite norimą įrašą.
4. Sąraše spustelėkite saitą pasirinktoje eilutėje.
    * Pasirinktas sutarties įsipareigojimo tipas įtakoja, kokią informaciją galite įvesti sutarties eilutėse. Pvz., jei sutartis pagrįsta verte, turite nurodyti bendrą grynąją sumą (sutarta valiuta), už kurią klientas įsipareigoja nusipirkti iš jūsų prekių. Šiame pavyzdyje eilučių laukų Kiekis ir Vienetas naudoti negalima, nes kuriate sutartį, pagal kurią klientas pirks konkrečios vertės produktų kiekį.   
5. Lauke Grynoji suma įveskite piniginę sumą, už kurią klientas įsipareigojo pirkti.
6. Lauke Nuolaidos procentas įveskite procentinę reikšmę, kuri bus taikoma kliento pardavimo užsakymo eilutėms, susietoms su šia sutartimi.
7. Išplėskite skyrių Eilutės informacija.
8. Lauke Maksimaliai vykdoma pasirinktie Taip.
    * Jei pasirenkate Maksimaliai vykdoma, bendra visų pardavimo užsakymo eilučių, kurios naudoja konkrečias įsipareigojimo kainas, nuolaidas ir (arba) mokėjimo sąlygas, suma negali viršyti nurodytos įsipareigojimo sumos.  
    * Mažiausia ir didžiausia išleidimo sumos nurodo vertės, už kurią reikia parduoti prekių vykdant kiekvieną pasirinktos sutarties pardavimo užsakymą, intervalą.   
9. Išplėskite sekciją Pardavimo sutarties antraštė.
    * Jei sutarties būsena nėra nustatyta kaip Galiojanti, pardavimo užsakymų negalima susieti su sutartimi ir todėl jie neturi įtakos sutarties sąlygų vykdymui. Šio etapo metu būseną galite neautomatiškai pakeisti. Tačiau įprastai būsena keičiama tvirtinant kliento sutartį.  
10. Srityje Veiksmas spustelėkite Pardavimo sutartis.
11. Spustelėkite „Patvirtinimas“.
    * Įsitikinkite, kad parinktis Pažymėti sutartį kaip galiojančią, nustatyta kaip Taip.  
12. Lauke Spausdinti ataskaitą pasirinkite Taip.
13. Spustelėkite GERAI.
14. Uždarykite puslapį.
    * Dabar sutartis galioja ir jūs galite pradėti kliento užsakymus sieti su sutartimi ir dengti įsipareigoto tikslo sumą.  


