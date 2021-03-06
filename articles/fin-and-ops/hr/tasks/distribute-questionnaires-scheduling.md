--- 
title: "Platinti klausimynus naudojant planavimą"
description: "Klausimyno planavimo funkcija suteikia galimybę planuoti ir platinti klausimynus keliems respondentams."
author: kherr75
manager: AnnBe
ms.date: 11/01/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-365-talent
ms.technology: 
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Operations, Talent
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 63a02a64ff28531bae950f1b61d9167eaa0b0373
ms.openlocfilehash: 8dd7365a18f371694f21a19efca76bd3e29ed641
ms.contentlocale: lt-lt
ms.lasthandoff: 11/01/2017

---
# <a name="distribute-questionnaires-using-scheduling"></a>Platinti klausimynus naudojant planavimą

[!include[task guide banner](../../includes/task-guide-banner.md)]

Klausimyno planavimo funkcija suteikia galimybę planuoti ir platinti klausimynus keliems respondentams. Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.


## <a name="create-a-questionnaire-schedule"></a>Klausimyno grafiko kūrimas
1. Pasirinkite Klausimynas > Platinti > Klausimynų grafikai.
2. Spustelėkite Naujas.
3. Lauke Planavimas įveskite reikšmę.
4. Lauke Aprašas įveskite reikšmę.
    * Nustatykite grafiką į Anoniminis, jei atsakymai turėtų būti registruojami be su jais susietų vardų.  
    * Parinktį Leisti anoniminius rezultatus pirmiausia reikia nustatyti personalo parametruose.  
5. Lauke Tipas pasirinkite planavimo tipą.  Šiame pavyzdyje naudojame pasitenkinimo tipą.
6. Sąraše raskite ir pasirinkite norimą įrašą.
7. Sąraše spustelėkite saitą pasirinktoje eilutėje.
8. Lauke Data įveskite datą.
9. Išplėskite skyrių Darbuotojų savitarnos el. paštas.
10. Lauke „Tema“ įveskite reikšmę.
    * Pavyzdys: galimas klausimynas  
11. Lauke Tekstas įveskite el. laiško tekstą. Atkreipkite dėmesį, kad kintamasis gali būti naudojamas sistemos reikšmėms pakeisti.
    * Pavyzdys: Gerb. %P%, prisijunkite prie darbuotojų savitarnos, kad užpildytumėte klausimyną apie darbuotojų sveikatą.  Contoso  
12. Spustelėkite Įrašyti.

## <a name="use-the-setup-details-to-select-the-questionnaires-to-be-answered-as-well-as-any-queries-to-use-to-select-respondents"></a>Naudokite sąrankos informaciją klausimynui (-ams) parinkti ir teikti užklausas respondentams pasirinkti.
1. Spustelėkite Sąrankos informacija.
2. Sąraše pasirinkite užklausą klausimyno respondentams sistemoje ieškoti.
    * Pavyzdys: darbuotojai  
3. Spustelėkite Peržiūrėti arba modifikuoti užklausą, norėdami pasirinkti konkrečius žmones arba koreguokite užklausą, kad rastumėte konkrečius kriterijus atitinkančių žmonių.
    * Atkreipkite dėmesį, kad visi respondentai turi būti sistemos vartotojai.  
4. Sąraše pažymėkite asmens eilutę.
5. Lauke Kriterijai įveskite arba pasirinkite reikšmę.
    * Pasirinkite Julia Funderburk  
6. Sąraše pasirinkite Julia Funderburk
7. Spustelėkite GERAI.
8. Spustelėkite skirtuką Klausimynai.
9. Medyje išplėskite dalį pasitenkinimo apklausos tipo klausimyno mazgas.
10. Medyje pažymėkite Darbuotojų sveikatos įvertinimas.
11. Spustelėkite GERAI.
12. Spustelėkite Planuojamas atsakymų seansas.
    * Atkreipkite dėmesį, kad funkcija Planuojamas atsakymų seansas sukuriama kiekvienam pažymėtam / užklaustam vartotojui.  
13. Uždarykite puslapį.

## <a name="start-the-questionnaire-schedule-in-order-to-make-the-questionnaire-available-for-respondents-to-complete"></a>Pradėkite klausimyno grafiką, kad respondentai galėtų klausimyną užpildyti.
1. Spustelėkite Funkcijos.
2. Spustelėkite Pradėti.
3. Spustelėkite GERAI.

## <a name="send-the-email-to-inform-respondents-of-the-available-questionnaire"></a>Siųskite respondentams el. laišką, informuojantį apie galimą klausimyną.
1. Spustelėkite Funkcijos.
2. Spustelėkite Siųsti el. laišką.
3. Spustelėkite Atšaukti.

## <a name="use-planned-answer-sessions-to-monitor-who-needs-to-complete-the-questionnaire"></a>Naudokite funkciją Suplanuotas atsakymų seansas, norėdami stebėti, kas turi užpildyti klausimyną.
1. Spustelėkite Planuojamas atsakymų seansas.
    * Panaikinkite visus likusius suplanuotus atsakymų seansus, kai esate pasirengę baigti suplanuotą seansą.  
2. Spustelėkite Naikinti.
3. Spustelėkite Taip.
4. Uždarykite puslapį.

## <a name="end-the-schedule-when-all-respondents-have-completed-the-questionnaire-andor-all-remaining-planned-answer-sessions-have-been-deleted"></a>Baikite grafiką, kai visi respondentai užpildė klausimyną ir (arba) panaikinti visi likę suplanuoti atsakymų seansai.
1. Spustelėkite Funkcijos.
2. Spustelėkite Baigti.
3. Spustelėkite GERAI.


