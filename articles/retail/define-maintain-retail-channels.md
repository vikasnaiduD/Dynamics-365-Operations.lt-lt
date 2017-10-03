---
title: "Apibrėžti ir prižiūrėti mažmeninės prekybos kanalus"
description: "Šiame straipsnyje pateikiama tradicinių parduotuvių, kurios „Microsoft Dynamics 365 for Retail“ nurodomos kaip mažmeninės prekybos parduotuvės, nustatymo proceso apžvalga. Jame pateikiama informacija apie užduotis, kurias turite atlikti prieš ir po mažmeninės prekybos parduotuvės nustatymo."
author: mugunthanm
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: 
ms.service: dynamics-365-retail
ms.technology: 
ms.search.form: RetailStoreTable, RetailStoreTableListPagePreviewPane
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, AX 7.0.0, Operations, UnifiedOperations, Retail
ms.custom: 16481
ms.assetid: 14496d96-1c72-43ce-a2e7-8467bab4ae46
ms.search.region: Global
ms.search.industry: Retail
ms.author: mumani
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.translationtype: Human Translation
ms.sourcegitcommit: 59b51840c05fe649cf322bfa64737a321728a5aa
ms.openlocfilehash: 3f0b566963574569cb40b72550e2337c9ba8a2ce
ms.contentlocale: lt-lt
ms.lasthandoff: 06/20/2017

---

# <a name="define-and-maintain-retail-channels"></a>Apibrėžti ir prižiūrėti mažmeninės prekybos kanalus

[!include[banner](includes/banner.md)]


Šiame straipsnyje pateikiama tradicinių parduotuvių, kurios „Microsoft Dynamics 365 for Retail“ nurodomos kaip mažmeninės prekybos parduotuvės, nustatymo proceso apžvalga. Jame pateikiama informacija apie užduotis, kurias turite atlikti prieš ir po mažmeninės prekybos parduotuvės nustatymo.

„Dynamics 365 for Retail‟ palaiko kelis mažmeninės prekybos kanalus, pvz., internetines parduotuves, skambučių centrus ir tradicines parduotuves. Tradicinė parduotuvė vadinama mažmeninės prekybos parduotuve. Kiekvienoje mažmeninės prekybos parduotuvėje gali būti naudojami savi mokėjimo būdai, kainų grupės, pardavimo vietos (POS) kasos aparatai, pajamų ir išlaidų sąskaitos bei darbuotojai. Prieš kurdami mažmeninės prekybos parduotuvę, turite nustatyti visus šiuos jos elementus. Kai sukuriate mažmeninės prekybos parduotuvę, galite priskirti produktus, kuriuos norite, kad ji platintų. Be to, parduotuvei priskiriami darbuotojai, kasos aparatai ir klientai. Galiausiai, įtraukite naują parduotuvę į organizacijos hierarchiją.

## <a name="setting-up-retail-stores"></a>Mažmeninės prekybos parduotuvių nustatymas
Prieš nustatydami mažmeninės prekybos parduotuvę programoje „Dynamics 365 for Retail‟, turite atlikti kai kurias būtinąsias užduotis. Tada galite sukurti mažmeninės prekybos parduotuvę ir pridėti informacijos.

### <a name="prerequisites"></a>Būtinieji komponentai

Prieš nustatydami mažmeninės prekybos parduotuvę, turite atlikti tolesnes užduotis.

1.  Sukonfigūruokite savo organizacijos struktūrą ir nustatykite mažmeninės prekybos asortimento, papildymo ir ataskaitų teikimo organizacijos hierarchijas.
2.  Nustatykite sandėlį, atitinkantį mažmeninės prekybos parduotuvę.
3.  Nustatykite mažmeninės prekybos parduotuvių, parduotuvių išrašų ir išrašų kvitų numeracijas.
4.  Sukonfigūruokite „Retail‟ parametrus.
5.  Nustatykite parduotuvėje naudojamus mokėjimo būdus.
6.  Norėdami kredito kortelių operacijas apdoroti mažmeninės prekybos POS kasos aparatuose, taip pat galite nustatyti mokėjimo paslaugas.
7.  Nustatykite PVM grupes.
8.  Nustatykite mažmeninės prekybos produktus. Vykdant šią užduotį, taip pat nustatomos mažmeninės prekybos produktų hierarchijos, produktų variantai ir produktų asortimentai.
9.  Nustatykite produktų kainų grupes.
10. Nustatykite mažmeninės prekybos produktų kainodarą. Vykdant šią užduotį, taip pat nustatomi kainos koregavimai, nuolaidos ir nuolaidų laikotarpiai.
11. Nustatykite darbuotojus. **Pastaba.** Taip pat darbuotojams turite priskirti reikiamas teises, kad jie galėtų prisijungti ir atlikti užduotis naudodami „Dynamics 365 for Retail“ sistemą, skirtą „Retail POS‟.
12. Sukonfigūruokite „Retail POS‟ profilius, priskirtinus parduotuvei. Ši užduotis apima daug kitų užduočių, pvz., kasos aparatų nustatymą, autonominių profilių nustatymą ir kvitų formatų bei profilių nustatymą.

Peržiūrėkite visas užduotis, įtrauktas į būtinąsias sąlygas, ir atlikite tik jums taikomas užduotis.

### <a name="set-up-a-retail-store"></a>Parduotuvės nustatymas

Atlikę būtinas užduotis, atlikite tolesnes užduotis, norėdami nustatyti informaciją apie mažmeninės prekybos parduotuvę.

1.  Sukurkite mažmeninės prekybos parduotuvę.
2.  Priskirkite parduotuvei PVM grupę.
3.  Parduotuvei priskirkite priimtus mokėjimo būdus.
4.  Įtraukite informaciją į mažmeninės prekybos parduotuvėse siūlomų produktų aprašus. Pavyzdžiui, galite įtraukti raiškiojo teksto ir vaizdų. Ši produktų informacija rodoma įvairiomis aplinkybėmis, pavyzdžiui, POS kasos aparate ar išspausdintose etiketėse.
5.  Mažmeninės prekybos parduotuvę pridėkite į numatytąją organizacijos hierarchiją, kuri priskirta **Mažmeninės prekybos asortimento**, **Mažmeninės prekybos papildymo** ar **Mažmeninės prekybos ataskaitų** tikslu.

### <a name="after-you-set-up-a-retail-store"></a>Nustačius mažmeninės prekybos parduotuvę

Įvedę mažmeninės prekybos parduotuvės informaciją, atlikite nurodytas užduotis, norėdami nusiųsti naujus mažmeninės prekybos parduotuvės duomenis į „Retail POS‟.

1.  Sukonfigūruokite parduotuvės POS kasos aparatus.
2.  Parduotuvei priskirkite produktų asortimentą.
3.  Apdorokite asortimentus norėdami sukurti produktų, kurie įtraukti į asortimentą, sąrašą ir padaryti produktus pasiekiamus mažmeninės prekybos parduotuvėje.
4.  Siųskite duomenis, pvz., numeracijas, aparatūros profilius ir POS ekrano maketus į „Retail POS‟ kasos aparatus.
5.  Publikuokite mažmeninės prekybos parduotuvę norėdami siųsti parduotuvės duomenis į „Retail POS‟.
6.  Vykdykite užduotis norėdami siųsti parduotuvės duomenis į „Retail POS‟.

## <a name="organization-hierarchies"></a>Organizacijų hierarchijos
„Retail‟ naudoja organizacijos hierarchijas mažmeninės prekybos kanalams struktūrizuoti. Organizacijos hierarchijos nurodo ryšius tarp organizacijų, kurios sudaro jūsų verslą. Kai nustatote parduotuves, galite įtraukti jas į organizacijos hierarchiją. Tada parduotuvės bendrina duomenis, kurie naudojami asortimentams, papildymui ir ataskaitoms.



