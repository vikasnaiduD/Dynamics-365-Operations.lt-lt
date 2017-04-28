---
title: Asortimento nustatymas
description: "Šiame straipsnyje aprašyta, kas yra asortimentas ir paaiškinta, kaip asortimentus nustatyti „Microsoft Dynamics 365 for Operations“ versijoje „Retail“."
author: josaw1
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core, Retail
ms.custom: 15811
ms.assetid: d2580048-e798-4b33-85f9-d1bad7d262fc
ms.search.region: global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: 0c6a7bdc4ba82dd57ab3e395e6dfb0ae4de31fc4
ms.openlocfilehash: 906fc6eb42eb54cb3a3d5621377f250f59de20d7
ms.lasthandoff: 03/31/2017


---

# <a name="set-up-assortments"></a>Asortimento nustatymas

[!include[banner](includes/banner.md)]


Šiame straipsnyje aprašyta, kas yra asortimentas ir paaiškinta, kaip asortimentus nustatyti „Microsoft Dynamics 365 for Operations“ versijoje „Retail“.

Asortimentas yra susijusių produktų, kuriuos priskiriate mažmeninės prekybos kanalui, pvz., plytos ir skiedinys sandėlyje arba internetinėje parduotuvėje, rinkinys. Asortimentą galite naudoti identifikuoti produktams, kurie yra kiekvienoje parduotuvėje. Galite naudoti asortimentą identifikuoti produktus, kurie yra kiekvienoje parduotuvėje. Asortimente gali būti produktų kategorijos. Todėl visi konkrečiai kategorijai priskirti produktai yra įtraukti į asortimentą. Asortimentas taip pat gali apimti konkrečius produktus ir konkrečius produktų variantus. Kurdami asortimentą, tuo pačiu metu galite priskirti tūkstančius produktų savo mažmeninės prekybos kanalams, bet kartu ir visus derinius, kurių reikia jūsų parduotuvėms. Galite nustatyti tiek produktų asortimente, kiek jums reikia. Kiekvieną produktą galima įtraukti į vieną ar daugiau asortimentų, o kiekvieną asortimentą galima priskirti vienam ar keliems mažmeninės prekybos kanalsms. Pavyzdžiui, nustatykite vieną asortimentą, kuris apima bazinį produktų rinkinį. Šį asortimentą gauna visos parduotuvės. Tada nustatykite kitą asortimentą, kuris apima tik didelę sporto įrangą. Šį asortimentą gauna tik didesnės parduotuvės. Toliau pateikiamoje diagramoje parodyta, kaip priskirti produktus asortimentui ir kaip asortimentus priskirti mažmeninės prekybos kanalams. ![Prekių asortimento ryšiai](./media/assortments_relationship.gif)

## <a name="prerequisites"></a>Būtinieji komponentai
Prieš sukurdami asortimentą ir priskirdami jį prie mažmeninės prekybos kanalui, turite atlikti šias užduotis.

| Užduotis                              | Prekės/Paslaugos pavadinimas                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|-----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Sukurkite mažmeninės prekybos kanalą.          | Mažmeninės prekybos kanalas skirtas plytų ir skiedinio parduotuvei, internetinei parduotuvei arba ar internetinei prekyvietei. Turite sukurti bent vieną mažmeninės prekybos kanalą ir sukonfigūruoti parduotuvės parinktis. Asortimentai priskiriami parduotuvėms, kad būtų galima identifikuoti parduotuvės produktus.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Sukurkite organizacijos hierarchiją. | Sukūrę savo organizacijos mažmeninės prekybos kanalą, turite sukonfigūruoti mažmeninės organizacijos hierarchiją, kuri atitinka jūsų mažmeninės prekybos kanalo organizacinę struktūrą. Organizacijos hierarchiją galima naudoti asortimentams, prekių papildymui ir ataskaitoms. Pridėdami savo mažmeninės prekybos kanalus į organizacijos hierarchiją, galite priskirti asortimentus parduotuvių grupėms. Užuot priskyrus asortimentą atskirai kiekvienai parduotuvei, galite priskirti asortimentą aukšto lygio organizacijos mazgui. Tada, kaskart pridedant naują mažmeninį kanalą į aukšto lygio organizacijos mazgą, mažmeninės prekybos kanalas automatiškai gauna visus asortimentus, kurie buvo priskirti aukštesnio lygio organizacijos mazgui. Asortimentus galite priskirti tik mažmeninės prekybos kanalams, kurie yra įtraukti į organizacijos hierarchiją, kuri yra priskirta **Mažmeninio asortimento** tikslu. |
| Nustatykite produktus.                  | Prieš pridėdami produktus į asortimentą, turite įtraukti juos į „Microsoft Dynamics AX“. Produktus galite pridėti rankiniu būdu arba importuoti iš tiekėjo. Pridėję produktus, turite išleisti juos juridiniam asmeniui. Jūsų mažmeninės prekybos kanaluose gali būti tik juridiniam asmeniui išleisti produktai. Produktus, kurie dar neišleisti juridiniam asmeniui, galima pridėti prie asortimento ir asortimentą galima patvirtinti. Tačiau kol produktai bus išleisti juridiniam asmeniui, jų negalima pateikti į mažmeninės prekybos kanalus.                                                                                                                                                                                                                                                                                     |
| Nustatykite kategorijos hierarchiją.      | Kurdami savo mažmeninės prekybos produktus, galite grupuoti ir suskirstyti juos naudodami kategorijų hierarchijos funkciją „Microsoft Dynamics 365 for Operations“. Galite sukurti vieną pagrindinę hierarchiją visų produktų, kuriuos platinate savo mažmeninės prekybos kanalais, grupavimui ir skirstymui. Taip pat galite kurti atskiras, papildomas kategorijų hierarchijas grupuoti arba skirstyti savo produktus specialiais tikslais, pavyzdžiui, akcijoms arba asortimentams. Naudodami kategorijų hierarchijas, galite priskirti visus produktus, tam tikrai kategorijai į asortimentą. Bet kurie produktai, kurie pridedami į asortimente esančią kategoriją, yra automatiškai įtraukiami į asortimentą. Tada kitą kartą paleidžiant mažmeninės prekybos asortimentą, šie produktai bus prieinami mažmeninės prekybos kanaluose, kuriems yra priskirtas asortimentas.                                            |

## <a name="setting-up-an-assortment"></a>Asortimento nustatymas
Baigę skirstyti, galite sukurti asortimentą ir priskirti jį savo mažmeninės prekybos kanalams. Norėdami sudaryti asortimentą, turite atlikti toliau nurodytas užduotis.

1.  Sukurkite naują asortimentą arba nukopijuokite esamą asortimentą.
2.  Pasirinkite mažmeninės kanalus arba aukšto lygio mažmeninės prekybos kanalų grupes, kurioms taikomas asortimentas.
3.  Pridėti produktų kategorijas, atskirus produktus ar produktų variantus į asortimentą. Galite įtraukti visus produktus į tam tikrą kategoriją arba pašalinti pasirinktus produktus iš kategorijos, kuri yra įtraukta į asortimentą.
4.  Paskelbkite asortimentą. Paskelbus asortimentą, paleidžiama automatiškai mažmeninės prekybos asortimento planuoklė. Šis procesas generuoja produktų sąrašą. Baigus procesą, gaminiai tampa prieinami mažmeninės prekybos kanaluose, kuriems yra priskirtas asortimentas. Jei daromi paskelbto asortimento pakeitimai, arba keičiami asortimentui priskirti mažmeninės prekybos kanalai, asortimentas turi būti atnaujintas. Norėdami atnaujinti asortimentą po pakeitimų, galite paleisti parduotuvių planuoklę kaip paketinę užduotį.




