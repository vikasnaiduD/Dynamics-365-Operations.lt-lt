---
title: "Elektroninių ataskaitų konfigūravimas duomenims į „Power BI“ perkelti"
description: "Šioje temoje paaiškinama, kaip galima naudoti elektroninio ataskaitų (ER) konfigūraciją, norint išdėstyti duomenų perkėlimą iš „Finance and Operations“ egzemplioriaus į „Power BI“ tarnybas. Šioje temoje pateikiamame pavyzdyje „Intrastat“ operacijos naudojamos kaip verslo duomenys, kuriuos reikia perkelti. „Power BI“ schemos vizualizacijoje naudojami šie „Intrastat“ operacijų duomenys, kad „Power BI“ ataskaitoje būtų pateiktas įmonės importavimo / eksportavimo veiklų analizės rodinys."
author: NickSelin
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application User, Developer, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 220314
ms.assetid: 2685df16-5ec8-4fd7-9495-c0f653e82567
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 90749012c3eb4f3d1c275f0661f8cff43ec285a2
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="configure-electronic-reporting-to-pull-data-into-power-bi"></a>Elektroninių ataskaitų konfigūravimas duomenims į „Power BI“ perkelti

[!include[banner](../includes/banner.md)]


Šioje temoje paaiškinama, kaip galima naudoti elektroninio ataskaitų (ER) konfigūraciją, norint išdėstyti duomenų perkėlimą iš „Finance and Operations“ egzemplioriaus į „Power BI“ tarnybas. Šioje temoje pateikiamame pavyzdyje „Intrastat“ operacijos naudojamos kaip verslo duomenys, kuriuos reikia perkelti. „Power BI“ schemos vizualizacijoje naudojami šie „Intrastat“ operacijų duomenys, kad „Power BI“ ataskaitoje būtų pateiktas įmonės importavimo / eksportavimo veiklų analizės rodinys.

<a name="overview"></a>Apžvalga
--------

„Microsoft Power BI“ yra programinės įrangos paslaugų, programų ir jungčių, kurios kartu naudojamos norint išorinius duomenų šaltinius paversti nuosekliomis, vizualiai įtraukiančiomis ir interaktyvių įžvalgomis, rinkinys. Elektroninės ataskaitos (ER) „Microsoft Dynamics 365 for Finance and Operations“ vartotojams suteikia galimybę lengvai konfigūruoti duomenų šaltinius ir išdėstyti duomenų perkėlimą iš „Finance and Operations“ į „Power BI“. Duomenys perkeliami kaip failai „OpenXML“ darbalapio („Microsoft Excel“ darbaknygės failų) formatu. Perkelti failai saugomi „Microsoft SharePoint Server“, kuris šiuo tikslu sukonfigūruotas. Saugomi failai naudojami „Power BI“ norint kurti ataskaitas su vizualizacijomis (lentelėmis, diagramomis, schemomis ir t.t.). „Power BI“ ataskaitas bendrai naudoja „Power BI“ vartotojai, ir jas galima pasiekti „Power BI“ ataskaitų srityse bei „Finance and Operations“ puslapiuose. Šioje temoje paaiškinamos toliau nurodytos užduotys.

-   „Finance and Operations” konfigūravimas.
-   ER formato konfigūracijos parengimas, norint gauti duomenis „Finance and Operations“.
-   ER aplinkos konfigūravimas duomenims į „Power BI“ perkelti.
-   Perkeltų duomenų naudojimas „Power BI“ ataskaitai kurti.
-   „Power BI“ ataskaitos prieigos programoje „Finance and Operations“ kūrimas.

## <a name="prerequisites"></a>Būtinieji komponentai
Norint įvykdyti šios temos pavyzdžio užduotis, reikia toliau nurodytų prieigų.

-   Prieiga prie „Finance and Operations“ naudojant vieną iš tolesnių vaidmenų.
    -   Elektroninės ataskaitos kūrėjas
    -   Elektroninės ataskaitos funkcijų konsultantas
    -   Sistemos administratorius
-   Prieiga prie „SharePoint Server“, kuris sukonfigūruotas naudoti su „Finance and Operations“
-   Prieiga prie „Power BI“ sistemos

## <a name="configure-document-management-parameters"></a>Dokumentų valdymo parametrų konfigūravimas
1.  Puslapyje **Dokumentų valdymo parametrai** sukonfigūruokite prieigą prie „SharePoint Server“, kuris bus naudojamas įmonėje, prie kurios esate prisijungę (šiame pavyzdyje – įmonėje DEMF).
2.  Patikrinkite ryšį su „SharePoint Server“ ir įsitikinkite, kad prieiga jums suteikta. [![Puslapis Dokumentų valdymo parametrai](./media/ger-power-bi-sharepoint-server-setting-1024x369.png)](./media/ger-power-bi-sharepoint-server-setting.png)
3.  Atidarykite sukonfigūruotą „SharePoint“ svetainę. Sukurkite naują aplanką, kuriame ER išsaugos „Excel“ failus su verslo duomenimis, kurie „Power BI“ ataskaitose reikalingi kaip „Power BI“ duomenų rinkinių šaltinis.
4.  „Finance and Operations“ puslapyje **Dokumentų tipai** sukurkite naują dokumento tipą, kuris bus naudojamas norint pasiekti ką tik sukurtą „SharePoint“ aplanką. Lauke **Grupė** įveskite **Failas**, lauke **Vieta** įveskite **SharePoint** ir tada įveskite „SharePoint“ aplanko adresą. [![Puslapis Dokumentų tipai](./media/ger-power-bi-sharepoint-document-type-1024x485.png)](./media/ger-power-bi-sharepoint-document-type.png)

## <a name="configure-er-parameters"></a>ER parametrų konfigūravimas
1.  Darbo srityje **Elektroninės ataskaitos** spustelėkite saitą **Elektroninių ataskaitų parametrai**.
2.  Visuose skirtuko **Priedai** laukuose pasirinkite dokumentų tipą **Failas**.
3.  Darbo srityje **Elektroninės ataskaitos** nustatykite reikiamą teikėją kaip aktyvų, spustelėdami **Nustatyti kaip aktyvų**. Norėdami gauti daugiau informacijos, paleiskite užduočių vedlį **ER: paslaugų teikėjo pasirinkimas**.

## <a name="use-an-er-data-model-as-the-source-of-data"></a>ER duomenų modelio kaip duomenų šaltinio naudojimas
ER duomenų modelis turi būti nustatytas kaip verslo duomenų, kurie bus naudojami „Power BI“ ataskaitose, šaltinis. Šis duomenų modelis įkeliamas iš ER konfigūracijų saugyklos. Daugiau informacijos žr. puslapyje [Elektroninių ataskaitų konfigūracijų atsisiuntimas iš „Lifecycle Services“](download-electronic-reporting-configuration-lcs.md) arba paleiskite užduočių vedlį **ER: konfigūracijos importavimas iš „Lifecycle Services‟**. Pasirinkite **Intrastat** kaip duomenų modelį, kuris bus įkeltas iš pasirinktos ER konfigūracijų saugyklos. (Šiame pavyzdyje naudojama 1 modelio versija.) **Intrastat** ER modelio konfigūraciją galite pasiekti puslapyje **Konfigūracijos**. [![Puslapis Konfigūracijos](./media/ger-power-bi-data-model-1024x371.png)](./media/ger-power-bi-data-model.png)

## <a name="design-an-er-format-configuration"></a>ER formato konfigūracijos kūrimas
Turite sukurti naują ER formato konfigūraciją, kuri **Intrastat** duomenų modelį naudoja kaip verslo duomenų šaltinį. Šio formato konfigūracija turi išvesties rezultatus generuoti kaip „OpenXML“ („Excel“ failo) formato elektroninius dokumentus. Norėdami gauti daugiau informacijos, paleiskite užduočių vedlį **ER: konfigūracijos, skirtos generuoti ataskaitas OPENXML formatu, kūrimas**. Naują konfigūraciją pavadinkite **Importavimo / eksportavimo veiklos**, kaip pavaizduota tolesnėje iliustracijoje. Kurdami ER formatą, naudokite „Excel“ failą [ER duomenys – importavimo ir eksportavimo informacija](https://go.microsoft.com/fwlink/?linkid=845208) kaip šabloną. (Norėdami daugiau informacijos apie tai, kaip importuoti formato šabloną, paleiskite užduočių vedlį). [![Importavimo / eksportavimo veiklų konfigūracija](media/ger-power-bi-format-configuration.png)](media/ger-power-bi-format-configuration.png) Norėdami keisti formato **Importavimo / eksportavimo veiklos** konfigūraciją, atlikite tolesnius veiksmus.

1.  Spustelėkite **Konstruktorius**.
2.  Skirtuke **Formatas** šio formato failo elementą pavadinkite **„Excel“ išvesties failas**. [![„Excel“ išvesties failo elementas](./media/ger-power-bi-format-configuration-file-element-name-1024x395.png)](./media/ger-power-bi-format-configuration-file-element-name.png)
3.  Skirtuke **Susiejimas** nurodykite „Excel“ failo, kuris bus visada generuojamas naudojant šį formatą, pavadinimą. Konfigūruokite susijusią išraišką, kad būtų pateikta reikšmė **Importavimo ir eksportavimo informacija** (failo vardo plėtinys .xlsx bus pridėtas automatiškai). [![Formato kūrimo įrankis](./media/ger-power-bi-format-configuration-output-file-name-1024x396.png)](./media/ger-power-bi-format-configuration-output-file-name.png)
4.  Įtraukite naują šio formato duomenų šaltinio elementą. (Šis išvardijimas bus reikalingas atliekant tolesnį duomenų susiejimą.)
    1.  Duomenų šaltinį pavadinkite **direction\_enum**.
    2.  Pasirinkite duomenų šaltinio tipą **Duomenų modelių išvardijimas**.
    3.  Nurodykite duomenų modelio išvardijimą **Kryptis**.

    [![direction\_enum](./media/ger-power-bi-format-configuration-mapping-added-enum-1024x454.png)](./media/ger-power-bi-format-configuration-mapping-added-enum.png)
5.  Atlikite **Intrastat** duomenų modelio elementų ir sukurto formato elementų susiejimą, kaip pavaizduota tolesnėje iliustracijoje. [![Susiejimas](./media/ger-power-bi-format-configuration-mapping-details-1024x454.png)](./media/ger-power-bi-format-configuration-mapping-details.png)

Paleidus ER formatą sugeneruojamas išvesties rezultatas „Excel“ formatu. „Intrastat“ operacijų informacija nusiunčiama į išeigos rezultatą ir atskiriama kaip operacijos, nurodančios importavimo veiklas arba eksportavimo veiklas. Spustelėkite **Paleisti**, norėdami išbandyti naują „Intrastat“ operacijų sąrašo ER formatą puslapyje **Intrastat** (**Mokestis** &gt; **Deklaracijos** &gt; **Užsienio prekyba** &gt; **Intrastat**). [![Puslapis Intrastat](./media/ger-power-bi-format-test-run-transactions-1024x322.png)](./media/ger-power-bi-format-test-run-transactions.png) Sugeneruojamas tolesnis išeigos rezultatas. Failas pavadintas **Importavimo ir eksportavimo informacija.xlsx**, kaip nurodėte formato parametruose. [![Importavimo ir eksportavimo informacija.xlsx](./media/ger-power-bi-format-test-run-output-1024x472.png)](./media/ger-power-bi-format-test-run-output.png)

## <a name="configure-the-er-destination"></a>ER paskirties vietos konfigūravimas
Turite sukonfigūruoti ER sistemą siųsti naujos ER formato konfigūracijos išeigos rezultatą ypatingu būdu.

-   Išeigos rezultatas turi būti siunčiamas pasirinkto „SharePoint Server“ aplanką.
-   Kiekvieną kartą paleidus formato konfigūraciją, turi būti nauja to paties „Excel“ failo versija.

Puslapyje **Elektroninės ataskaitos** (**Organizacijos administravimas** &gt; **Elektroninės ataskaitos**) spustelėkite elementą **Elektroninių ataskaitų paskirtis** ir įtraukite naują paskirties vietą. Lauke **Nuoroda** pasirinkite anksčiau sukurtą formato konfigūraciją **Importavimo / eksportavimo veiklos**. Atlikite šiuos veiksmus, norėdami įtraukti naują nuorodos failo paskirties vietos įrašą.

1.  Lauke **Pavadinimas** įveskite failo paskirties vietos pavadinimą.
2.  Lauke **Failo vardas** pasirinkite „Excel“ failo formato komponento vardą **„Excel“ išvesties failas**.

Spustelėkite naujo paskirties vietos įrašo mygtuką **Parametrai**. Tada dialogo lange **Paskirties vietos parametrai** atlikite tolesnius veiksmus.

1.  Skirtuke **Power BI** nustatykite parinktį **Įjungta** į **Taip**.
2.  Lauke **SharePoint** pasirinkite anksčiau sukurtą dokumentų tipą **Bendrai naudojama**.

## <a name="schedule-execution-of-the-configured-er-format"></a>Sukonfigūruoto ER formato vykdymo planavimas
Puslapio **Konfigūracijos** (**Organizacijos administravimas** &gt; **Elektroninės ataskaitos** &gt; **Konfigūracijos**) konfigūracijų medyje pasirinkite anksčiau sukurtą konfigūraciją **Importavimo / eksportavimo veiklos**. Keisti 1.1 versijos būseną iš **Juodraštis** į **Baigta**, kad šį formatą būtų galima naudoti. [![Puslapis Konfigūracijos](./media/ger-power-bi-format-configuration-complete-1024x401.png)](./media/ger-power-bi-format-configuration-complete.png) Pasirinkite baigtą konfigūracijos **Importavimo / eksportavimo veiklos** versiją ir spustelėkite **Paleisti**. Atkreipkite dėmesį, kad sukonfigūruota paskirties vieta taikoma išeigos rezultatui, sugeneruotam „Excel“ formatu. Nustatykite parinktį **Paketinis vykdymas** į **Taip**, norėdami šią ataskaitą paleisti režimu be priežiūros. Spustelėkite **Pasikartojimas**, norėdami suplanuoti reikiamą šio paketinio vykdymo pasikartojimą. Pasikartojimas nurodo, kaip dažnai atnaujinti duomenys bus perduoti iš „Finance and Operations“ į „Power BI“. [![Dialogo langas Elektroninių ataskaitų parametrai](./media/ger-power-bi-format-configuration-run-to-schedule-1024x413.png)](./media/ger-power-bi-format-configuration-run-to-schedule.png) Sukonfigūruotą ER ataskaitos vykdymo užduotį galite rasti puslapyje **Paketinės užduotys** (**Sistemos administravimas &gt; Užklausos &gt; Paketinės užduotys**). [![Puslapis Paketinės užduotys](./media/ger-power-bi-format-configuration-running-job-1024x410.png)](./media/ger-power-bi-format-configuration-running-job.png)Kai ši užduotis vykdoma pirmą kartą, pasirinktame „SharePoint“ aplanke paskirties vieta sukuria naują „Excel“ failą sukonfigūruotu pavadinimu. Kaskart vėliau paleidus užduotį, paskirties vieta sukuria naują šio „Excel“ failo versiją. [![Nauja „Excel“ failo versija](./media/ger-power-bi-output-file-in-sharepoint-server-folder-2-1024x412.png)](./media/ger-power-bi-output-file-in-sharepoint-server-folder-2.png)

## <a name="create-a-power-bi-dataset-by-using-the-output-result-of-the-er-format"></a>„Power BI“ duomenų rinkinio kūrimas naudojant ER formato išeigos rezultatą
Prisijunkite prie „Power BI“ ir atidarykite esamą „Power BI“ grupę (darbo sritis) arba sukurkite naują grupę. Skyriaus **Duomenų importavimas arba prijungimas** dalyje **Failai** spustelėkite **Įtraukti** arba kairiosios srities dalyje **Duomenų rinkiniai** spustelėkite pliuso ženklą (**+**). [![Duomenų rinkinio kūrimas](./media/ger-power-bi-add-dataset-1024x524.png)](./media/ger-power-bi-add-dataset.png) Pasirinkite parinktį **„SharePoint“ – komandos svetainės** ir tada įveskite naudojamo „SharePoint Server“ kelią (pateiktame pavyzdyje – **https://ax7partner.litware.com**). Tada naršykite ir atidarykite aplanką **/Shared Documents/GER data/PowerBI** bei pasirinkite „Excel“ failą, kurį sukūrėte kaip naujo „Power BI“ duomenų rinkinio duomenų šaltinį. [![„Excel“ failo pasirinkimas](./media/ger-power-bi-add-dataset-select-excel-file-1024x522.png)](./media/ger-power-bi-add-dataset-select-excel-file.png) Spustelėkite **Prijungti**, tada – **Importuoti**. Sukuriamas naujas duomenų rinkinys, pagrįstas pasirinktu „Excel“ failu. Duomenų rinkinį taip pat galima automatiškai įtraukti į naujai sukurtą ataskaitų sritį. [![Duomenų rinkinys ataskaitų srityje](./media/ger-power-bi-added-dataset-1024x489.png)](./media/ger-power-bi-added-dataset.png) Konfigūruokite šio duomenų rinkinio naujinimo grafiką norėdami vykdyti periodinį naujinimą. Periodiniai naujinimai suteikia galimybę naudoti naujus „Finance and Operations“ verslo duomenis, periodiškai paleidžiant ER ataskaitą per naujas „Excel“ failo versijas, sukurtas „SharePoint Server“.

## <a name="create-a-power-bi-report-by-using-the-new-dataset"></a>„Power BI“ ataskaitos kūrimas naudojant naują duomenų rinkinį
Norėdami kurti naują „Power BI“ ataskaitą, spustelėkite sukurtą „Power BI“ duomenų rinkinį **Importavimo ir eksportavimo informacija**. Tada konfigūruokite vizualizaciją. Pvz., pasirinkite vizualizaciją **Užpildyta schema** ir sukonfigūruokite ją, kaip nurodyta toliau.

-   Duomenų rinkinio lauką **CountryOrigin** priskirkite schemos vizualizacijos laukui **Vieta**.
-   Duomenų rinkinio lauką **Amount** priskirkite schemos vizualizacijos laukui **Spalvų sotis**.
-   Duomenų rinkinio laukus **Veikla** ir **Metai** įtraukite schemos vizualizacijos laukų rinkinį **Filtrai**.

Įrašyti „Power BI“ ataskaitą **Importavimo ir eksportavimo informacijos ataskaita**. [![Importavimo ir eksportavimo informacijos ataskaita](./media/ger-power-bi-added-report-1024x498.png)](./media/ger-power-bi-added-report.png) Atkreipkite dėmesį, kad schemoje rodomos šalys / regionai, nurodyti „Excel“ faile (šiame pavyzdyje – Austrija ir Šveicarija). Šios šalys / regionai pateikiami naudojant skirtingas spalvas, kad būtų parodyta proporcinga kiekvienoje šalyje / regione išrašytų SF sumų dalis. Atnaujinkite „Intrastat“ operacijų sąrašą. Įtraukiama eksportavimo operacija, kuri buvo sugeneruota Italijoje. [![„Intrastat“ operacijų sąrašas](./media/ger-power-bi-new-run-new-transaction-1024x321.png)](./media/ger-power-bi-new-run-new-transaction.png) Palaukite kito suplanuoto ER ataskaitos vykdymo ir kito suplanuoto „Power BI“ duomenų rinkinio naujinimo. Tada peržiūrėkite „Power BI“ ataskaitą (pasirinkite, kad būtų rodomos tik importuotos operacijos). Atnaujintoje schemoje dabar rodoma Italija. [![Atnaujinta schema](./media/ger-power-bi-new-run-new-map-1024x511.png)](./media/ger-power-bi-new-run-new-map.png)

## <a name="access-power-bi-report-in-finance-and-operations"></a>Pasiekite„Power BI“ ataskaitą programoje „Finance and Operations“.
Nustatykite „Finance and Operations“ ir „Power BI“ integravimą. Daugiau informacijos rasite puslapyje [„Power BI‟ integravimo konfigūravimas darbo sritims](configure-power-bi-integration.md). Darbo sričių puslapyje **Elektroninės ataskaitos**, kuriame palaikomas „Power BI“ integravimas (**Organizacijos administravimas** &gt; **Darbo sritys** &gt; **Elektroninių ataskaitų darbo sritis**), spustelėkite **Parinktys** &gt; **Atidaryti ataskaitų katalogą**. Pasirinkite sukurtą „Power BI“ ataskaitą **Importavimo ir eksportavimo informaciją**, kad ta ataskaita pasirinktame puslapyje būtų rodoma kaip veiksmo elementas. Spustelėkite veiksmo elementą, norėdami atidaryti „Finance and Operations“ puslapį, kuriame rodoma ataskaita, sukurta naudojant „Power BI“. [![Importavimo ir eksportavimo informacijos ataskaita](./media/ger-power-bi-review-bi-report-in-ax-form-1024x586.png)](./media/ger-power-bi-review-bi-report-in-ax-form.png)

<a name="see-also"></a>Taip pat žiūrėkite
--------

[Elektroninių ataskaitų paskirties vietos](electronic-reporting-destinations.md)

[Elektroninių ataskaitų apžvalga](general-electronic-reporting.md)




