--- 
title: "Konfigūracijų peržiūra, kad elektroninėse ataskaitose (ER) būtų galima kurti ataskaitas „Microsoft Office“ formatais su įdėtaisiais vaizdais"
description: "Norėdami atlikti šiuos veiksmus, turite užbaigti veiksmus užduočių vedlyje „ER padaryti ataskaitas „MS Office“ formatais su įdėtaisiais vaizdais (1 dalis: nustatyti parametrus)“."
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
ms.openlocfilehash: dcc162a4c0ba81079eefb7564ab037c1287acd92
ms.contentlocale: lt-lt
ms.lasthandoff: 09/29/2017

---
# <a name="review-configurations-to-make-reports-in-microsoft-office-formats-with-embedded-images-for-electronic-reporting-er"></a>Konfigūracijų peržiūra, kad elektroninėse ataskaitose (ER) būtų galima kurti ataskaitas „Microsoft Office“ formatais su įdėtaisiais vaizdais

[!include[task guide banner](../../includes/task-guide-banner.md)]

Norėdami atlikti šiuos veiksmus, turite užbaigti veiksmus užduočių vedlyje „ER padaryti ataskaitas „MS Office“ formatais su įdėtaisiais vaizdais (1 dalis: nustatyti parametrus)“.

Ši procedūra parodo, kaip sukurti elektroninių ataskaitų kūrimo (ER) konfigūracijas, norint generuoti elektroninius dokumentus, kuriuose yra įdėtųjų vaizdų „Microsoft Excel“ ir „Microsoft Word“. Šiame pavyzdyje peržiūrėsite pavyzdinės įmonės „Litware, Inc.“ ER konfigūracijas. 

Ši procedūra skirta vartotojams, kuriems priskirtas sistemos administratoriaus arba elektroninių ataskaitų teikimo programuotojo vaidmuo. Šiuos veiksmus galima atlikti naudojant USMF duomenų rinkinį.


## <a name="review-the-imported-data-model"></a>Peržiūrėkite importuotų duomenų modelį
1. Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.
2. Medyje pasirinkite „Model for cheques“.
3. Spustelėkite Konstruktorius.
    * Šis modelis skirtas atstovauti mokėjimo čekius verslo požiūriu ir susieti šį modelį su programos duomenų šaltiniais. Peržiūrėkite šį modelį naudodami ER operacijų kūrimo priemonę. Atkreipkite dėmesį į pateiktus modelio elementų atributus: struktūrą, pavadinimą, aprašymą, duomenų tipą ir t.t.   
4. Medyje išplėskite „root“.
5. Medyje pasirinkite „root\cheques“.
6. Medyje išplėskite „root\cheques“.
7. Medyje išplėskite „root\cheques\attributes“.
8. Medyje išplėskite „root\payer“.
9. Medyje pasirinkite „root\istestrun“.
10. Medyje pasirinkite „root\layout“.
    * Šio modelio išdėstymo elementą sudaro pasirinktos banko sąskaitos čekio formos maketo spausdinimo informacija. Taip pat apima du konteinerio duomenų tipo mazgus vaizdams saugoti.   
11. Medyje išplėskite „root\layout“.
12. Medyje pasirinkite „root\layout\company logo“.
13. Medyje išplėskite „root\layout\company logo“.
14. Medyje pasirinkite „root\layout\company logo\image“.
15. Medyje pasirinkite „root\layout\company logo\isprinted“.
16. Medyje pasirinkite „root\layout\signature“.
17. Medyje išplėskite „root\layout\signature“.
18. Medyje pasirinkite „root\layout\signature\image“.
19. Medyje pasirinkite „root\layout\signature\isprinted“.
    * Atkreipkite dėmesį, kad du vaizdo duomenų modelio elementai susieti su lentelių laukais, kuriuose yra įmonės logotipas ir įgalioto asmens parašas dvejetainiu formatu.  
20. Medyje išplėskite „root\layout\watermark“.
21. Spustelėkite „Susieti modelį su duomenų šaltiniu“.
22. Spustelėkite Konstruktorius.
23. Medyje išplėskite „chequesselected“.
24. Medyje išplėskite „layout“.
25. Medyje išplėskite „layout\company logo“.
26. Medyje išplėskite „layout\signature“.
27. Medyje išplėskite „layout\watermark“.
28. Įjunkite „Rodyti išsamią informaciją”.
    * Atkreipkite dėmesį, kad čekių duomenų modelio elementas yra susietas su TmpChequePrintout lentele, kurioje vykdant bus čekių įrašai, kuriuos vartotojas pasirinko spausdinti.   
29. Uždarykite puslapį.
30. Uždarykite puslapį.
31. Uždarykite puslapį.

## <a name="review-the-imported-format"></a>Peržiūrėkite importuotą formatą
1. Medyje išplėskite „Model for cheques“.
2. Medyje pasirinkite „Model for cheques\Cheques printing format“.
3. Spustelėkite Konstruktorius.
4. Spustelėkite Priedai.
5. Spustelėkite Atidaryti.
    * Atidarykite pridėtą ataskaitos šabloną „Excel“.  
    * Peržiūrėkite pridėtos ataskaitos „Excel“ šabloną, kuris bus naudojamas čekiams spausdinti. Šablone yra du čekiai puslapyje, jis skirtas čekiams spausdinti iš anksto išspausdintoje formoje. Atkreipkite dėmesį, kad yra įdėti du tušti vaizdai. Šie tušti vaizdai skirti įmonės logotipui ir parašui asmens, kuris autorizuoja mokėjimą. Patikrinkite, ar vaizdai pavadinti CompLogo ir SignatureImage, atitinkamai, „Excel“.   
6. Uždarykite puslapį.
7. Medyje išplėskite „Report“.
8. Medyje išplėskite „Report\ChequeLines“.
9. Medyje pasirinkite „Report\ChequeLines\CompLogo“.
10. Įjunkite „Rodyti išsamią informaciją”.
    * Atkreipkite dėmesį, kad „CompLogo“ formato langelio elementas rodo „Excel“ elementą, naudojamą įmonės logotipo vaizdui įtraukti į ataskaitą. Šis formato elementas yra susietas su vaizdo duomenų modelio elementu, vykdant jame yra įmonės logotipo vaizdas dvejetainiu formatu.   
11. Spustelėkite skirtuką „Susiejimas“.
12. Spustelėkite Redagavimas įgalintas
    * Atkreipkite dėmesį, kad galite padaryti „CompLogo“ formato langelio elementą, kuris nebeįgalintas. Šiuo atveju susietas „Excel“ vaizdo elementas paslėps įmonės logotipą sugeneruotoje ataskaitoje. Jei įgalintos išraiškos rezultatas TRUE ir apibrėžtas susiejimas neteikia vaizdo, susietas „Excel“ vaizdo elementas rodys vaizdą, kuris buvo įrašytas „Excel“ šablone.   
13. Uždarykite puslapį.
14. Medyje išplėskite „labels: Container“.
    * Kai kurios etiketės, kurios pateikiamos iš anksto išspausdintoje čekio formoje, bus įtrauktos į ataskaitą, kai sukuriama bandymams. Tačiau tos etiketės nebus išspausdintos spausdinant iš tikrųjų, nes iš anksto išspausdintoje formoje jos jau yra.  
15. Uždarykite puslapį.


