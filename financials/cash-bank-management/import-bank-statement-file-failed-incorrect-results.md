---
title: "Banko išrašo failo importavimo trikčių šalinimas"
description: "Svarbu, kad banko išrašo failas iš banko atitiktų maketą, kurį palaiko „Microsoft Dynamics 365 for Operations“. Dėl griežtų banko išrašų standartų, dauguma integravimų veiks tinkamai. Tačiau kartais išrašo failo nepavyksta importuoti arba rezultatai yra neteisingi. Paprastai šios problemos kyla dėl mažų skirtumų banko išrašo faile. Šiame straipsnyje paaiškinama, kaip pašalinti šiuos skirtumus ir išspręsti problemas."
author: twheeloc
manager: AnnBe
ms.date: 04/04/2017
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 141273
ms.assetid: 3ee2f32b-02aa-420b-8990-e6aa5fc6bda3
ms.search.region: global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: eab840b2974f4e9e8cf542c146482ba8e4239079
ms.openlocfilehash: 9717cf2f36033efe8465906324966242977c6eb2
ms.lasthandoff: 03/31/2017


---

# <a name="bank-statement-file-import-troubleshooting"></a>Banko išrašo failo importavimo trikčių šalinimas

[!include[banner](../includes/banner.md)]


Svarbu, kad banko išrašo failas iš banko atitiktų maketą, kurį palaiko „Microsoft Dynamics 365 for Operations“. Dėl griežtų banko išrašų standartų, dauguma integravimų veiks tinkamai. Tačiau kartais išrašo failo nepavyksta importuoti arba rezultatai yra neteisingi. Paprastai šios problemos kyla dėl mažų skirtumų banko išrašo faile. Šiame straipsnyje paaiškinama, kaip pašalinti šiuos skirtumus ir išspręsti problemas.

<a name="what-is-the-error"></a>Kokia klaida?
------------------

Pabandę importuoti banko išrašo failą, atidarykite užduoties Duomenų valdymas retrospektyvą ir jos vykdymo informaciją, kad rastumėte klaidą. Klaida gali suteikti pagalbos, nurodydama išrašą, balansą arba išrašo eilutę. Tačiau nėra tikėtina, kad ji suteiks pakankamai informacijos, padėsiančios jums nustatyti lauką arba elementą, dėl kurio kyla problema.

## <a name="what-are-the-differences"></a>Kokie skirtumai?
Palyginkite banko failo maketo aprašą su „Microsoft Dynamics 365 for Operations“ importo aprašu ir pasižymėkite bet kokius laukų ir elementų skirtumus. Palyginkite banko išrašo failą su susijusiu „Dynamics 365 for Operations“ failo pavyzdžiu. ISO20022 failuose skirtumus pastebėti turėtų būti lengva.

## <a name="transformations"></a>Transformacijos
Paprastai keitimą reikia atlikti vienoje iš trijų transformacijų. Kiekviena transformacija parašyta konkrečiam standartui.

| Išteklių pavadinimas                                         | Failo vardas                          |
|-------------------------------------------------------|------------------------------------|
| BankStmtImport\_BAI2CSV\_to\_BAI2XML\_xslt            | BAI2CSV-to-BAI2XML.xslt            |
| BankStmtImport\_ISO20022XML\_to\_Reconciliation\_xslt | ISO20022XML-to-Reconciliation.xslt |
| BankStmtImport\_MT940TXT\_to\_MT940XML\_xslt          | MT940TXT-to-MT940XML.xslt          |

## <a name="debugging-transformations"></a>Transformacijų derinimas
### <a name="adjust-the-bai2-and-mt940-files"></a>BAI2 ir MT940 failų koregavimas

BAI2 ir MT940 failai yra tekstiniai failai ir juos reikia koreguoti, norint įjungti išplėstinės stiliaus aprašų kalbos transformacijų (XSLT) derinimą. Programa atlieka šį koregavimą, kai failas importuojamas.

1.  Kurkite XML failą ir į jį nukopijuokite tolesnį tekstą.

        <Batch><![CDATA[PASTESTATEMENTFILEHERE
        ]]></Batch>

2.  Nukopijuokite banko išrašo failo turinį ir įklijuokite jį į XML failą, kad jis pakeistų **PASTESTATEMENTFILEHERE**.

### <a name="debug-the-xslt"></a>XSLT derinimas

Daugiau informacijos žr. <https://msdn.microsoft.com/en-us/library/ms255605.aspx>.

1.  Paleiskite „Microsoft Visual Studio“.
2.  Kurkite konsolės programą.
3.  Atidarykite atitinkamą XSLT.
4.  Spustelėkite XLST ir jos ypatybių puslapį.
5.  Nustatykite įvestį į banko išrašo failo vietą.
6.  Nurodykite išvesties vietą ir failo vardą.
7.  Nustatykite reikiamus ribinius taškus.
8.  Meniu spustelėkite **XML** &gt; **Pradėti derinti XSLT**.

### <a name="format-the-xslt-output"></a>XSTL išvesties formatavimas

Kai transformacija paleidžiama, ji sukuria išvesties failą, kurį galima peržiūrėti „Visual Studio“. Naudokite CTRL + A, CTRL + K ir CTRL + D, norėdami greitai formatuoti išvesties failą.

### <a name="adjust-the-transformation"></a>Transformacijos koregavimas

Koreguokite transformaciją, norėdami banko išrašo faile gauti atitinkamą lauką arba elementą. Tada susiekite tą lauką arba elementą su atitinkamu „Dynamics 365 for Operations“ elementu.

### <a name="debitcredit-indicator"></a>Debeto / kredito indikatorius

Kartais debetai gali būti importuoti kaip kreditai, o kreditai gali importuoti kaip debetai. Norėdami išspręsti šią problemą, pakeiskite atitinkamą XSLT. Jeigu banko išrašai pateikiami iš kelių bankų, įsitikinkite, kad jie visi naudoja tą patį debeto / kredito metodą, arba sukurkite atskiras transformacijas.

-   BAI2XML-to-Reconciliation.xlst GetAmountCreditDebitIndicator šablonas
-   ISO20022XML-to-Reconcilation.xslt GetCreditDebit šablonas
-   MT940XML-to-Reconcilation.xslt GetCreditDebitIndicator šablonas

## <a name="examples-of-bank-statement-formats-and-technical-layouts"></a>Banko išrašų formatų ir techninių maketų pavyzdžiai
Tolesnėje lentelėje pateikiami išplėstinio banko derinimo importavimo failo techninio maketo aprašų pavyzdžiai ir trys susijusių banko išrašo failų pavyzdžiai. Failų ir techninių maketų pavyzdžius galite atsisiųsti čia: https://mbs.microsoft.com/customersource/northamerica/AX/learning/documentation/how-to-articles/exofbankstfotechlayouts  


| Techninio maketo aprašas                             | Banko išrašo failo pavyzdys          |
|---------------------------------------------------------|--------------------------------------|
| DynamicsAXMT940Layout                                   | MT940StatementExample                |
| DynamicsAXISO20022Layout                                | ISO20022StatementExample             |
| DynamicsAXBAI2Layout                                    | BAI2StatementExample                 |





