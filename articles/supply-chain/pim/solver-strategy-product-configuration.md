---
title: "Sprendimo priemonės strategija produktams konfigūruoti"
description: "Šioje temoje aprašoma, kaip, naudodami sprendimo priemonės strategiją, galite pagerinti produktų konfigūravimo našumą."
author: cvocph
manager: AnnBe
ms.date: 01/02/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
ms.search.form: PCCreateProductConfigurationModel, PCProductConfigurationModelListPage
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Core, Operations
ms.custom: 
ms.assetid: 
ms.search.region: Global
ms.search.industry: 
ms.author: conradv
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 8075abccdcdde21df967dcc9948a738895f35cef
ms.openlocfilehash: 035103b183c637dcce454686d44535a6fa07c745
ms.contentlocale: lt-lt
ms.lasthandoff: 01/25/2018

---

# <a name="solver-strategy-for-product-configuration"></a>Sprendimo priemonės strategija produktams konfigūruoti

[!include[banner](../includes/banner.md)]

Šioje temoje aprašoma, kaip, naudodami sprendimo priemonės strategiją, galite pagerinti produktų konfigūravimo našumą.

Sprendimo priemonės strategijų koncepcija pirmą kartą buvo pristatyta „Microsoft Dynamics AX 2012 R2“ 7 kaupiamajame naujinime (CU7). Ji buvo išplėsta „Microsoft Dynamics AX 2012 R3“ 8 kaupiamajame naujinime (CU8) ir sprendime „Microsoft Dynamics 365 for Finance and Operations, Enterprise edition 7.3“.

Sprendimo priemonės strategijos koncepciją dabar sudaro tolesnės strategijos.

- Numatyta
- Pirmiausia mažiausi domenai
- Iš viršaus į apačią
- Z3

## <a name="solver-strategy"></a>Sprendimo priemonės strategija 

Produkto konfigūracijos modelį galima suformuluota kaip [apribojimų patenkinimo problemą (CSP)](http://aima.cs.berkeley.edu/2nd-ed/newchap05.pdf). Spręsti CSP problemoms „Microsoft Solver Foundation“ (MSF) teikia dviejų tipų sprendimo priemonės strategijas, kurias galima naudoti produktų konfigūracijos modeliuose. Šios sprendimo priemonės strategijos remiasi [euristika](https://techterms.com/definition/heuristic), kurią naudojant, nustatoma, kokia tvarka svarstomi CSP kintamieji sprendžiant problemą. Euristika gali pastebimai paveikti našumą, kai sprendžiama problema ar problemų klasė.

Sprendime „Finance and Operations“ produktų konfigūracijos modelių sprendimo priemonės strategija nustato, kuri sprendimo priemonė naudojama su euristika. Strategijos **Numatytoji**, **Pirmiausia mažiausi domenai** ir **Iš viršaus į apačią** naudoja dvi MSF sprendimo priemones, o strategija **Z3** naudoja sprendimo priemonę Z3. 

Realaus klientų įgyvendinimo tyrimai parodė, kad, pakeitus produkto konfigūracijos modelio sprendimo priemonės strategiją, atsakymo laiką galima sumažinti nuo minučių iki milisekundžių. Todėl verta išbandyti skirtingas sprendimo priemonės strategijas, kad rastumėte našiausią strategiją jūsų produkto konfigūracijos modeliui.

## <a name="change-the-settings-for-the-solver-strategy"></a>Sprendimo priemonės strategijos parametrų keitimas

Norėdami keisti sprendimo priemonės strategiją, puslapio **Produktų konfigūracijos modeliai** veiksmų srityje pasirinkite **Modelių ypatybės**. Tada dialogo lange **Redaguoti modelių informaciją** pasirinkite sprendimo priemonės strategiją.

[![Sprendimo priemonės strategijos keitimas](./media/solver-strategy.png)](./media/solver-strategy.png)

Šiuo metu nėra jokios logikos, kuri automatiškai aptiktų, kuri sprendimo priemonės strategija bus efektyviausia produktų konfigūracijai pagal apribojimus. Todėl sprendimo priemonės strategijas turite išbandyti po vieną.

Tolesnėje lentelėje pateikiama rekomendacijų apie tai, kurią sprendimo priemonės strategiją naudoti įvairiose situacijose.

| Sprendimo priemonės strategija      | Naudoti strategiją šioje situacijoje |
|----------------------|-----------------------------------|
| Numatyta              | **Numatytoji** strategija optimizuota spręsti modelius, pagrįstus lentelių apribojimais. Klientų įgyvendinimo tyrimai parodė, kad situacijose, kai plačiai naudojami lentelių apribojimai, ši strategija yra našiausia. |
| Pirmiausia mažiausi domenai | Strategijos **Pirmiausia mažiausi domenai** ir **Iš viršaus į apačią** yra glaudžiai susijusios. Klientų įgyvendinimo tyrimai parodė, kad strategijos **Iš viršaus į apačią**, pristatytos CU8 naujinime, rezultatai geresni už strategijos **Pirmiausia mažiausi domenai**. Tačiau strategija **Pirmiausia mažesni domenai** produkte laikoma dėl suderinamumo su ankstesnėmis versijomis. Pastebėta, kad abi šios sprendimo priemonės strategijos našiau sprendžia modelius su keliais aritmetiniais reiškiniais, kai nenaudojami lentelių apribojimai. Tačiau kai kuriais atvejais **numatytosios** strategijos rezultatai už šių dviejų strategijų rezultatus yra geresni. Todėl nepamirškite išbandyti kiekvienos strategijos. |
| Iš viršaus į apačią             | Strategijos **Pirmiausia mažiausi domenai** ir **Iš viršaus į apačią** yra glaudžiai susijusios. Klientų įgyvendinimo tyrimai parodė, kad strategijos **Iš viršaus į apačią**, pristatytos CU8 naujinime, rezultatai geresni už strategijos **Pirmiausia mažiausi domenai**. Tačiau strategija **Pirmiausia mažesni domenai** produkte laikoma dėl suderinamumo su ankstesnėmis versijomis. Pastebėta, kad abi šios sprendimo priemonės strategijos našiau sprendžia modelius su keliais aritmetiniais reiškiniais, kai nenaudojami lentelių apribojimai. Tačiau kai kuriais atvejais **numatytosios** strategijos rezultatai už šių dviejų strategijų rezultatus yra geresni. Todėl nepamirškite išbandyti kiekvienos strategijos. |
| Z3                   | Rekomenduojame kaip numatytąją sprendimo priemonės strategiją naudoti strategiją **Z3**. Jei esate susirūpinę dėl našumo ir išplečiamumo, galite įvertinti kitas strategijas. |

## <a name="additional-resources"></a>Papildomi ištekliai

[Produkto konfigūracijos modelio kūrimas](build-product-configuration-model.md)

[Euristika](https://techterms.com/definition/heuristic)

[Apribojimų patenkinimo problema](http://aima.cs.berkeley.edu/2nd-ed/newchap05.pdf)

