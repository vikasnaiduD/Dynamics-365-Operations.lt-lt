--- 
title: "Ataskaitų generavimas „Microsoft Office“ formatais su įdėtaisiais vaizdais elektroninėse ataskaitose (ER)"
description: "Šie veiksmai paaiškina, kaip sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmenį turintis vartotojas gali sukurti naują elektroninių ataskaitų teikimo (ER) konfigūraciją, skirtą elektroninių dokumentų, turinčių įdėtųjų vaizdų, generavimui „MS office“ formatais („Excel“ ir „Word“)."
author: NickSelin
manager: AnnBe
ms.date: 06/13/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: f827b4787506cfdec8b9a91c4a68f3293190158a
ms.openlocfilehash: 4fa27996e59164126f7900edf4a509ca9273e7c1
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="generate-reports-in-microsoft-office-formats-with-embedded-images-for-electronic-reporting-er"></a>Ataskaitų generavimas „Microsoft Office“ formatais su įdėtaisiais vaizdais elektroninėse ataskaitose (ER)

[!include[task guide banner](../../includes/task-guide-banner.md)]

Šie veiksmai paaiškina, kaip sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmenį turintis vartotojas gali sukurti naują elektroninių ataskaitų teikimo (ER) konfigūraciją, skirtą elektroninių dokumentų, turinčių įdėtųjų vaizdų, generavimui „MS office“ formatais („Excel“ ir „Word“).

Šiame pavyzdyje naudosite sukurtas pavyzdinės įmonės „Litware, Inc.“ ER konfigūracijas.  Norėdami atlikti šiuos veiksmus, turite užbaigti veiksmus užduočių vedlyje „ER padaryti ataskaitas „MS Office“ formatais su įdėtaisiais vaizdais (2 dalis: peržiūrėti konfigūracijas)“. Šiuos veiksmus galima atlikti USMF įmonėje.


## <a name="run-format-with-initial-model-mapping"></a>Paleiskite formatą pradiniu modelio susiejimu
1. Pasirinkite Grynųjų pinigų ir banko valdymas > Banko kodai > Banko kodai.
2. Naudokite spartųjį filtrą, kad filtruotumėte lauką Banko sąskaita reikšme „USMF OPER‟.
3. Veiksmų srityje spustelėkite Nustatyti.
4. Spustelėkite Tikrinti.
5. Spustelėkite Spausdinti testą.
    * Paleiskite formatą bandymams.  
6. Lauke Perduodamo čekio formatas pasirinkite Taip.
7. Spustelėkite GERAI.
    * Peržiūrėkite sukurtą išvestį. Atkreipkite dėmesį, kad įmonės logotipas pateikiamas ataskaitoje, taip pat ir įgalioto asmens parašas. Parašo vaizdas paimamas iš čekio išdėstymo įrašo duomenų tipo „Konteineris“ lauko, kuris susietas su pasirinkta banko sąskaita.  
8. Išplėskite skyrių Kopijos.
9. Spustelėkite Redaguoti.
10. Lauke Vandenženklis įveskite „Spausdinti vandenženklį kaip anuliuotą“.
    * Pakeisti vandenženklio išdėstymo nustatymą, kad būtų rodomas vandenženklio tekstas generuojant dokumentą „Excel“ formos elemente.  
11. Spustelėkite Spausdinti testą.
12. Spustelėkite GERAI.
    * Peržiūrėkite sukurtą išvestį. Atkreipkite dėmesį, kad vandenženklis rodomas sukurtoje ataskaitoje pagal žymėjimo parinktį.  
13. Uždarykite puslapį.
14. Veiksmų srityje spustelėkite Valdyti mokėjimus.
15. Spustelėkite Tikrinimai.
16. Spustelėkite Rodyti filtrus.
17. Taikykite šiuos filtrus: įveskite filtro reikšmę „381“, „385“, „389“ lauke „Čekio numeris“, naudodami filtro operatorių „vienas iš“
18. Sąraše pažymėkite visas eilutes.
19. Spustelėkite Spausdinti čekio kopiją.
    * Paleiskite formatą iš naujo spausdinti pasirinktus čekius.  
    * Peržiūrėkite sukurtą išvestį. Atkreipkite dėmesį, kad turite iš naujo išspausdinti pasirinktus čekius. Įmonės logotipas ir etiketės nespausdinamos, nes jos pateikiamos iš anksto išspausdintoje formoje.  

## <a name="modify-the-mapping-of-the-imported-data-model"></a>Pakeiskite importuoto duomenų modelio susiejimą
1. Uždarykite puslapį.
2. Uždarykite puslapį.
3. Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.
4. Medyje pasirinkite „Model for cheques“.
5. Spustelėkite Konstruktorius.
6. Spustelėkite „Susieti modelį su duomenų šaltiniu“.
7. Spustelėkite Konstruktorius.
    * Mes pakeisime duomenų modelio parašo elemento susiejimą, kad gautume parašo vaizdą iš failo, pridėto prie čekio maketo įrašo, susieto su pasirinkta banko sąskaita.  
8. Išjunkite Rodyti išsamią informaciją.
9. Medyje išplėskite „layout“.
10. Medyje išplėskite „layout\signature“.
11. Medyje pasirinkite „layout\signature\image = chequesaccount.'<Relations'.BankChequeLayout.Signature1Bmp“.
12. Medyje išplėskite „chequesaccount“.
13. Medyje išplėskite „chequesaccount\<Relations“.
14. Medyje pasirinkite „chequesaccount\<Relations\BankChequeLayout“.
15. Medyje išplėskite „chequesaccount\<Relations\BankChequeLayout\<Relations“.
16. Medyje išplėskite „chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents“.
17. Medyje pasirinkite „chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents\getFileContentAsContainer()“.
18. Spustelėkite Susieti.
19. Spustelėkite Įrašyti.
20. Uždarykite puslapį.
21. Uždarykite puslapį.
22. Uždarykite puslapį.
23. Uždarykite puslapį.

## <a name="run-format-using-the-adjusted-model-mapping"></a>Vykdykite formatą, naudodami pakoreguotą modelio susiejimą
1. Pasirinkite Grynųjų pinigų ir banko valdymas > Banko kodai > Banko kodai.
2. Norėdami rasti įrašus, naudokite spartųjį filtrą. Pavyzdžiui, filtruokite lauką Banko sąskaita, naudodami reikšmę „USMF OPER“.
3. Veiksmų srityje spustelėkite Nustatyti.
4. Spustelėkite Tikrinti.
5. Spustelėkite Spausdinti testą.
6. Spustelėkite GERAI.
    * Peržiūrėkite sukurtą išvestį. Atkreipkite dėmesį, kad vaizdas iš dokumentų valdymo priedo pateikiamas kaip įgalioto asmens parašas.  

## <a name="use-ms-word-document-as-a-template-in-the-imported-format"></a>Naudokite „MS Word“ dokumentą kaip šabloną importuotame formate
1. Uždarykite puslapį.
2. Uždarykite puslapį.
3. Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.
4. Medyje išplėskite „Model for cheques“.
5. Medyje pasirinkite „Model for cheques\Cheques printing format“.
6. Spustelėkite Konstruktorius.
7. Spustelėkite Priedai.
8. Spustelėkite Naikinti.
9. Spustelėkite Taip.
10. Spustelėkite Naujas.
11. Spustelėkite Failas.
    * Spustelėkite Naršyti ir pasirinkite atsisiųstą iš anksto „Cheque template Word.docx" failą.  
12. Uždarykite puslapį.
13. Lauke Šablonas įveskite arba pasirinkite reikšmę.
14. Spustelėkite Įrašyti.
15. Uždarykite puslapį.
16. Spustelėkite Redaguoti.
17. Lauke Paleisti juodraštį pasirinkite Taip.
18. Uždarykite puslapį.
19. Pasirinkite Grynųjų pinigų ir banko valdymas > Banko kodai > Banko kodai.
20. Naudokite spartųjį filtrą, kad filtruotumėte lauką Banko sąskaita reikšme „USMF OPER‟.
21. Spustelėkite Tikrinti.
22. Spustelėkite Spausdinti testą.
23. Spustelėkite GERAI.
    * Peržiūrėkite sukurtą išvestį. Atkreipkite dėmesį, kad išvestis sugeneruota kaip „Microsoft Word“ dokumentas su įdėtaisiais vaizdais, pateikiant įmonės logotipą, įgalioto asmens parašą ir pažymėtą vandenženklio tekstą.  


