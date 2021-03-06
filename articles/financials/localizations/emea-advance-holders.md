---
title: "Avanso turėtojai"
description: "Sužinokite apie avanso turėtojo funkciją programoje „Microsoft Dynamics 365 for Finance and Operations“ (leidimas „Enterprise‟)."
author: LizaGolub
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: HcmWorkerAdvHolderTableListPage_RU
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 262574
ms.search.region: Czech Republic, Estonia, Hungary, Latvia, Lithuania, Poland, Russia
ms.author: v-elgolu
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 36b6d74d29ed4606c1b501b68e0f2253e66c8eb6
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="advance-holders"></a>Avanso turėtojai

[!include[banner](../includes/banner.md)]


Sužinokite apie avanso turėtojo funkciją programoje „Microsoft Dynamics 365 for Finance and Operations“ (leidimas „Enterprise‟).

*Avanso turėtojas* yra įmonės darbuotojas, kuris yra atsakingas už organizacijos pateiktą išlaidų sumą. Tik įmonės darbuotojas gali būti avanso turėtojas. Vykdant įsigijimą, avanso turėtojas įmonei praneša apie patirtas išlaidas. Įmonė darbuotojui kompensuoja išlaidų sumą. Įmonė valdo kiekvieno avanso turėtojo balansą. Juridinių subjektų Estijoje, Latvijoje, Lietuvoje, Lenkijoje, Čekijos Respublikoje, Vengrijoje ir Rusijoje vartotojai gali nurodyti konkrečias operacijas ir operacijas su įmonės darbuotojais, kurie yra atsakingi už organizacijos pateiktą išlaidų sumą.

## <a name="set-up-an-advance-holder"></a>Avanso turėtojo nustatymas
Norint nustatyti avanso turėtoją, reikia nurodyta tvarka atlikti toliau pateiktas užduotis.
1.  Sukurkite avanso turėtojų grupes.
2.  Nustatykite darbuotojų registravimo šabloną.
3.  Nustatykite mokėtinų sumų parametrus.
4.  Sukurkite konkrečias kiekvieno avanso turėtojo mokėjimo sąlygas.
5.  Sukurkite avanso turėtoją.

### <a name="advance-holder-groups"></a>Avanso turėtojų grupės

Naudokite puslapį **Avanso turėtojų grupės**, kad sukurtumėte avanso turėtojų grupę. Galite nurodyti avanso turėtojų grupės pavadinimą, aprašą ir korespondentinę sąskaitą.
### <a name="employee-posting-profile"></a>Darbuotojų registravimo šablonas

Naudokite puslapį **Darbuotojų registravimo šablonai**, kad sukurtumėte avanso turėtojų operacijų šabloną. Galite nurodyti toliau pateiktą darbuotojų registravimo šablono informaciją.
|Laukas |aprašymas|
|------|-----------|
|Registravimo šablonas|Įveskite avanso turėtojo registravimo šablono identifikavimo kodą.|
|aprašymas|Įveskite trumpą registravimo šablono aprašą.|
|Galioja|Pasirinkite vieną iš tolesnių registravimo šablono nustatymo grupavimo lygio parinkčių. 
**Lentelė** – ši parinktis naudojama nustatant vieno avanso turėtojo registravimo šabloną. Turite nurodyti avanso turėtojo kodą lauke Nuoroda.
**Grupė** – ši parinktis naudojama nustatant avanso turėtojų grupės registravimo šabloną. Turite nurodyti grupės kodą lauke Nuoroda.
**Visi** – ši parinktis naudojama nustatant visų avanso turėtojų registravimo šabloną.| |Nuoroda|Pasirinkite avanso turėtojo kodą, jei lauke Galioja pasirinkta parinktis Lentelė, arba pasirinkite avanso turėtojo grupę, jei lauke Galioja pasirinkta parinktis Grupė.| |Suminė sąskaita|Pasirinkite operacijų registravimo suminę sąskaitą.|



### <a name="account-payable-parameters"></a>Mokėtinų sumų parametrai

Norėdami nurodyti avanso turėtojo operacijas, puslapio **Mokėtinų sumų parametrai** dalyje **Avanso turėtojai** turite nustatyti toliau pateiktą informaciją.
|                                                |                   |
|------------------------------------------------|-------------------|
|  **Laukas**                                     | **Aprašas**                                                                                                                                                                  |
| **Registravimo šablonas**                            | Pasirinkite numatytąjį avanso turėtojų operacijų baigimo šabloną.                                                                                                         |
| **Avanso turėtojų rūšiavimas**                     | Jei pažymėta, avanso turėtojai bus rodomi puslapio **Avanso turėtojai** sąrašo pradžioje.                                                                     |
| **Išduoti, kai balansas atidarytas**                 | Jei pažymėta, bus leidžiamas avanso grynaisiais pinigais išdavimas avanso turėtojui, kurio atidarytas balansas teigiamas.                                                                      |
| **Laukų grupė Balanso uždarymas per grynuosius: pavadinimas** | Pasirinkite grynųjų pinigų kvitų žurnalo kodą. Žurnalo kodas naudojamas grynųjų pinigų išmokėjimo kvitams ir kompensavimo kvitams generuoti, kai avanso turėtojo balansas uždaromas per grynuosius pinigus. |
| **Grynieji pinigai**                                       | Pasirinkite grynųjų pinigų sąskaitą, kad nurodytumėte kvitus, naudojamus uždarant avanso turėtojo balansus.                                                                 |
| **Laukų grupė Balanso uždarymas per banką: pavadinimas** | Pasirinkite operacijų žurnalo kodą, kad uždarytumėte balansus per banką.                                                                                                   |
| **Sąskaitos tipas**                               | Pasirinkite banką, kad uždarytumėte avanso turėtojo balansus per banką.                                                                                                        |
| **Pagrindinė sąskaita**                               | Pasirinkite banko sąskaitos kodą, kad uždarytumėte avanso turėtojo balansus per banką.                                                                                           |

### <a name="terms-of-payment-for-advance-holder"></a>Avanso turėtojo mokėjimo sąlygos

Norėdami tinkamai užregistruoti pirkimo užsakymą per avanso turėtoją, turite naudoti mokėjimo sąlygas, kurių parinktis **Iš avanso turėtojo** nustatyta į **Taip**.
### <a name="create-an-advance-holder-creation"></a>Avanso turėtojo kūrimas

Prieš kurdami avanso turėtoją, turite būti jau nustatę darbuotojus. Daugiau informacijos žr. [Darbuotojo informacijos įvedimas (užduočių vedlys)](../../fin-and-ops/hr/tasks/enter-worker-information.md) Naudokite puslapį **Avanso turėtojai**, kad darbuotoją nustatytumėte kaip avanso turėtoją. Pasirinkite darbuotoją, kurį nustatysite kaip avanso turėtoją, spustelėkite **Redaguoti** ir tada nustatykite parinktį **Avanso turėtojas** į **True**. Taip pat turite užpildyti tolesnius laukus.
|                |                                                                                             |
|----------------|---------------------------------------------------------------------------------------------|
| **Laukas**      | **Aprašas**                                                                             |
| **Grupė**      | Pasirinkite avanso turėtojų grupę.                                                             |
| **Serija**     | Įveskite dokumento, kuris naudojamas avanso turėtojo tapatybei patvirtinti, seriją. |
| **Numeris**     | Įveskite dokumento, kuris naudojamas avanso turėtojo tapatybei patvirtinti, numerį. |
| **Išdavimo data** | Pasirinkite arba įveskite dokumento išdavimo datą.                                                    |
| **Išdavė**  | Įveskite institucijos arba asmens, kuris išdavė dokumentą, informaciją.                       |

## <a name="advance-holder-inquiries-and-reports"></a>Avanso turėtojo užklausos ir ataskaitos
### <a name="advance-holder-transactions-inquiry"></a>Avanso turėtojo operacijų užklausa

Norėdami peržiūrėti avanso turėtojo operacijų sąrašą, puslapyje **Avanso turėtojai** spustelėkite mygtuką **Operacijos**. Norėdami peržiūrėti visų avanso turėtojų operacijas arba kurti konkrečią užklausą pagal avanso turėtojų operacijas, spustelėkite **Mokėtinos sumos** &gt; **Užklausos ir ataskaitos** &gt; **Avanso turėtojų užklausos ir ataskaitos** &gt; Operacijos. Spustelėkite **Kvitas**, kad atidarytumėte puslapį **Kvitų operacijos**.
### <a name="advance-holder-balance-inquiry"></a>Avanso turėtojo balanso užklausa

Norėdami peržiūrėti avanso turėtojo balansą, naudokite puslapį **Avanso turėtojai**. Norėdami peržiūrėti visų avanso turėtojų balansą arba kurti konkrečią užklausą pagal avanso turėtojų sąskaitas, spustelėkite **Mokėtinos sumos** &gt; **Užklausos ir ataskaitos** &gt; **Avanso turėtojų užklausos ir ataskaitos** &gt; **Balansas**.
### <a name="advance-holder-balance-report"></a>Avanso turėtojo balanso ataskaita

Norėdami peržiūrėti ir spausdinti ataskaitą, pagrįstą avanso turėtojų balanso informacija, spustelėkite **Mokėtinos sumos** &gt; **Užklausos ir ataskaitos** &gt; **Avanso turėtojų užklausos ir ataskaitos** &gt; **Avanso turėtojo balanso ataskaita**.
### <a name="advance-holder-transactions-report"></a>Avanso turėtojo operacijų ataskaita

Norėdami peržiūrėti ir spausdinti ataskaitą, pagrįstą avanso turėtojų operacijomis, spustelėkite **Mokėtinos sumos** &gt; **Užklausos ir ataskaitos** &gt; **Avanso turėtojų užklausos ir ataskaitos** &gt; **Avanso turėtojo operacijų ataskaita**.

## <a name="advance-holder-transactions"></a>Išankstinio savininko operacijos

Sužinokite, kaip programoje „Microsoft Dynamics 365 for Finance and Operations‟ (leidimas „Enterprise‟) dirbti su išankstinio savininko operacijomis.

Šių darbuotojų, kurie yra avanso turėtojai, operacijas galima registruoti naudojant avanso turėtojo sąskaitas. Darbuotojo ID, kuris priskirtas kiekvienam išankstiniams savininkui, galima naudoti norint sekti visas avanso turėtojo operacijas. Šis numeris nuskaitomas kaip avanso turėtojo operacijų sąskaitos numeris puslapiuose **Bendrieji žurnalai** ir **Avanso turėtojo operacijos**.

### <a name="create-and-post-a-purchase-order-with-advance-holder-details"></a>Pirkimo užsakymo su avanso turėtojo informacija kūrimas ir registravimas
Daugiau bendros informacijos apie pirkimo užsakymus žr. temoje [Pirkimo užsakymo apžvalga](../../supply-chain/procurement/purchase-order-overview.md). Jei tiekėjo SF sukuriama ir užregistruojama su avanso turėtojo informacija, avanso turėtojo balansas bus užregistruotas darbuotojo balanso sąskaitoje, o ne tiekėjo balanso sąskaitoje. Norėdami avanso turėtojo informaciją įtraukti į pirkimo užsakymą, atlikite tolesnius veiksmus.

-   Dalies **Kaina ir nuolaida** lauke **Mokėjimo sąlygos** pasirinkite mokėjimo sąlygą. <!---For more information about **Terms of payment**, see [Define vendor payment terms](accounts-payable/tasks/define-vendor-payment-terms).--> Pasirinkite mokėjimo sąlygą, kurios parinktis **Iš avanso turėtojo**, esanti puslapyje **Mokėjimo sąlygos**, pažymėta. Daugiau informacijos apie avanso turėtojų mokėjimo sąlygų nustatymą žr. temoje [Avanso turėtojai](emea-advance-holders.md).
-   „FastTab“ **Kaina ir nuolaida** lauke **Avanso turėtojas** pasirinkite pirkimo užsakymo avanso turėtoją.

Pirkimo užsakymo registravimo proceso metu sukuriamos dvi tiekėjo operacijos su priešingomis sumomis ir viena avanso turėtojo operacija. Sukuriama tik viena tiekėjo operacija be avanso turėtojo informacijos.

### <a name="settle-advance-holder-balances-via-a-bank"></a>Avanso turėtojo balanso sudengimas per banką
Kai avanso turėtojų balansus sudengiate per banką, žurnalo įrašai apie avanso turėtojo balansų uždarymą sukuriami pagrindiniame žurnale. Žurnalo ir banko kodus galite nustatyti puslapio **Mokėtinų sumų parametrai** dalyje **Avanso turėtojai**. Daugiau informacijos žr. temoje [Avanso turėtojai](emea-advance-holders.md). Norėdami uždaryti avanso turėtojo balansą per banką, atidarykite **Mokėtinos sumos** &gt; **Avanso turėtojai** &gt; **Avanso turėtojai**. Veiksmų srityje spustelėkite mygtuką **Balansas** ir tada spustelėkite **Uždaryti per banką**. Puslapyje **Uždaryti per banką** įveskite toliau nurodytą informaciją.

| Laukas                    | aprašymas |
|------------------------------|-------------------|
| **Mokėjimo data**          | Įvesti mokėjimo registravimo datą.|
| **Suma, skirta perkelti** | Įveskite balanso sumą uždarymo metu. Suma, kuri yra nurodyta formos **Balansas** lauke **Suma**, rodoma pagal numatytuosius parametrus. |
| **Automatiškai**                | Norėdami kurti ir registruoti žurnalą, kuris yra iš anksto nustatytas puslapyje **Gautinų sumų parametrai**, pažymėkite žymės laukelį **Automatiškai**.|

### <a name="settle-advance-holder-balances-via-cash"></a>Avanso turėtojo balanso sudengimas per kasą
Kai avanso turėtojų balansus sudengiate per kasą, žurnalo įrašai apie avanso turėtojo balansų uždarymą sukuriami važtaraščių žurnale. Žurnalo ir kasos kodus galite nustatyti puslapio **Mokėtinų sumų parametrai** skirtuke **Avanso turėtojai**. Daugiau informacijos žr. temoje [Avanso turėtojai](emea-advance-holders.md). Norėdami uždaryti avanso turėtojo balansą per kasą, atidarykite **Mokėtinos sumos** &gt; **Avanso turėtojai** &gt; **Avanso turėtojai**. Veiksmų srityje spustelėkite mygtuką **Balansas** ir tada spustelėkite **Uždaryti per kasą**. Puslapyje **Uždaryti per kasą** įveskite toliau nurodytą informaciją.

| Laukas                    | aprašymas
|------------------------------|-----------------|
| **Mokėjimo data**          | Įvesti mokėjimo registravimo datą.|
| **Suma, skirta perkelti** | Įveskite balanso sumą uždarymo metu. Suma, kuri yra nurodyta formos **Balansas** lauke **Suma**, rodoma pagal numatytuosius parametrus. |
| **Automatiškai**                | Norėdami automatiškai kurti ir registruoti žurnalą, kuris yra iš anksto nustatytas puslapyje **Gautinų sumų parametrai**, pažymėkite žymės laukelį **Automatiškai**.     |

Apdorojus važtaraščių žurnalą, jei suma, esanti lauke **Suma, skirta perkelti** yra neigiama, uždarius balansą generuojamas avanso turėtojo išmokėjimo kvitas. Jei suma lauke **Suma, skirta perkelti** yra teigiama, generuojamas kompensacijos kvitas.

## <a name="additional-resources"></a>Papildomi ištekliai

- [Išankstinis mokėjimas darbuotojui (Rytų Europa)](tasks/advance-payment-employee.md)




