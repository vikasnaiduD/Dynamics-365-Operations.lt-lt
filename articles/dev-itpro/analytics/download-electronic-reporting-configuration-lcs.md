---
title: "Elektroninių ataskaitų konfigūracijų atsisiuntimas iš „Lifecycle Services“"
description: "Šioje temoje paaiškinama, kaip atsisiųsti elektroninių ataskaitų (ER) konfigūracijas iš „Microsoft Dynamics Lifecycle Services“ (LCS)."
author: NickSelin
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
ms.search.form: ERSolutionImport, ERWorkspace
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.custom: 105843
ms.assetid: dc44dea2-22ce-401e-98b9-d289e0e2825b
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-05-31
ms.dyn365.ops.version: AX 7.0.1
ms.translationtype: HT
ms.sourcegitcommit: 2771a31b5a4d418a27de0ebe1945d1fed2d8d6d6
ms.openlocfilehash: 8fae33fbe2d1433e4263ed4087dad2bc894e0b84
ms.contentlocale: lt-lt
ms.lasthandoff: 11/03/2017

---

# <a name="download-electronic-reporting-configurations-from-lifecycle-services"></a>Elektroninių ataskaitų konfigūracijų atsisiuntimas iš „Lifecycle Services“

[!include[banner](../includes/banner.md)]


Šioje temoje paaiškinama, kaip atsisiųsti elektroninių ataskaitų (ER) konfigūracijas iš „Microsoft Dynamics Lifecycle Services“ (LCS).

Ši mokymo programa padės jums atsisiųsti naujausias elektroninio ataskaitų (ER) konfigūracijas iš „Microsoft Dynamics Lifecycle Services“ (LCS).

1.  Prisijunkite prie „Finance and Operations“ naudodami vieną iš tolesnių vaidmenų.
    -   Elektroninės ataskaitos kūrėjas
    -   Elektroninės ataskaitos funkcijų konsultantas
    -   Sistemos administratorius

2.  Pasirinkite **Organizacijos administravimas** &gt; **Elektroninės ataskaitos**.
3.  Dalyje **Konfigūracijų teikėjai** pasirinkite plytelę **Microsoft**.
4.  Plytelėje **Microsoft** spustelėkite **Saugyklos**. [![update-er-from-lcs-for-ms-open-ms-repositories-list](./media/update-er-from-lcs-for-ms-open-ms-repositories-list.png)](./media/update-er-from-lcs-for-ms-open-ms-repositories-list.png)
5.  Puslapio **Konfigūracijų saugyklos** tinklelyje pasirinkite esamą tipo **LCS** saugyklą. Jei ši saugykla tinklelyje nerodoma, atlikite tolesnius veiksmus.
    1.  Spustelėdami **Įtraukti** įtraukite naują saugyklą.
    2.  Pasirinkite **LCS** kaip saugyklos tipą.
    3.  Spustelėkite **Kurti saugyklą**.
    4. Paraginti vykdykite autorizavimo instrukcijas.
    5.  Įveskite saugyklos pavadinimą ir aprašymą.
    6.  Spustelėkite **Gerai**, kad patvirtintumėte naują saugyklos įrašą.
    7.  Tinklelyje pasirinkite naują tipo **LCS** saugyklą.

6.  Spustelėkite **Atidaryti**, norėdami peržiūrėti pasirinktos saugyklos ER konfigūracijų sąrašą. [![update-er-from-lcs-for-ms-make-lcs-repository](./media/update-er-from-lcs-for-ms-make-lcs-repository.png)](./media/update-er-from-lcs-for-ms-make-lcs-repository.png)
7.  Kairiojoje srityje esančiame konfigūracijų medyje pasirinkite reikiamą ER konfigūraciją.
8.  „FastTab“ **Versijos** pasirinkite reikiamą pasirinktos ER konfigūracijos versiją.
9.  Spustelėkite **Importuoti**, kad pasirinktą versiją atsisiųstumėte iš LCS į dabartinį „Finance and Operations“ egzempliorių. **Pastaba.** Mygtuko **Importuoti** negalima naudoti ER konfigūracijų versijose, kurios jau yra dabartiniame „Finance and Operations“ egzemplioriuje. [![update-er-from-lcs-for-ms-download-configuration](./media/update-er-from-lcs-for-ms-download-configuration.png)](./media/update-er-from-lcs-for-ms-download-configuration.png)

**Pastaba.** Atsižvelgiant į ER parametrus, konfigūracijos patikrinamos po importavimo. Galite būti informuoti apie rastas nenuoseklumo problemas. Prieš naudodami importuotą konfigūracijos versiją, turite išspręsti šias problemas. Daugiau informacijos ieškokite šios temos susijusių straipsnių sąraše.

<a name="see-also"></a>Taip pat žiūrėkite
--------

[Elektroninių ataskaitų apžvalga](general-electronic-reporting.md)




