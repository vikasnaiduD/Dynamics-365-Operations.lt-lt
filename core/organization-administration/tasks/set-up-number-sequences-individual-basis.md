--- 
title: "Atskirų numeracijų nustatymas"
description: "Numerių sekos naudojamos generuojant perskaitomus, unikalius identifikatorius bendrųjų duomenų įrašams ir operacijų įrašams, kuriems jie reikalingi."
author: sericks007
manager: AnnBe
ms.date: 06/07/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: sericks
ms.search.scope: Operations
ms.search.region: Global
ms.author: sericks
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 4e2808e57dc8d137fac892d48e99d7687ff1bf81
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-number-sequences-on-an-individual-basis"></a><span data-ttu-id="7a972-103">Atskirų numeracijų nustatymas</span><span class="sxs-lookup"><span data-stu-id="7a972-103">Set up number sequences on an individual basis</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="7a972-104">Numerių sekos naudojamos generuojant perskaitomus, unikalius identifikatorius bendrųjų duomenų įrašams ir operacijų įrašams, kuriems jie reikalingi.</span><span class="sxs-lookup"><span data-stu-id="7a972-104">Number sequences are used to generate readable, unique identifiers for master data records and transaction records that require them.</span></span> <span data-ttu-id="7a972-105">Pagrindinių duomenų arba operacijų įrašas, kuriam reikia identifikatoriaus, vadinamas nuoroda.</span><span class="sxs-lookup"><span data-stu-id="7a972-105">A master data or transaction record that requires an identifier is referred to as a reference.</span></span> <span data-ttu-id="7a972-106">Kad galėtumėte kurti naujus įrašus kaip nuorodas, turite nustatyti numeraciją ir susieti ją su nuoroda.</span><span class="sxs-lookup"><span data-stu-id="7a972-106">Before you can create new records for a reference, you must set up a number sequence and associate it with the reference.</span></span> <span data-ttu-id="7a972-107">Galite nustatyti visas reikiamas numeracijas tuo pačiu metu naudodami vedlį Numeracijų nustatymas arba galite sukurti ar modifikuoti atskiras numeracijas naudodami puslapį Numeracijos.</span><span class="sxs-lookup"><span data-stu-id="7a972-107">You can set up all required number sequences at the same time by using the Set up number sequences wizard, or you can create or modify individual number sequences by using the Number sequences page.</span></span>

1. <span data-ttu-id="7a972-108">Pasirinkite Organizacijos administravimas > Numeracijos > Numeracijos.</span><span class="sxs-lookup"><span data-stu-id="7a972-108">Go to Organization administration > Number sequences > Number sequences.</span></span>
2. <span data-ttu-id="7a972-109">Spustelėkite Numeracija.</span><span class="sxs-lookup"><span data-stu-id="7a972-109">Click Number sequence.</span></span>
3. <span data-ttu-id="7a972-110">Lauke Numeracijos kodas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="7a972-110">In the Number sequence code field, type a value.</span></span>
4. <span data-ttu-id="7a972-111">Lauke Pavadinimas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="7a972-111">In the Name field, type a value.</span></span>
5. <span data-ttu-id="7a972-112">Išplėskite dalį Aprėpties parametrai.</span><span class="sxs-lookup"><span data-stu-id="7a972-112">Expand the Scope parameters section.</span></span>
    * <span data-ttu-id="7a972-113">„FastTab“ skirtuke Aprėpties parametrai pasirinkite numeracijos aprėptį ir aprėpties reikšmes.</span><span class="sxs-lookup"><span data-stu-id="7a972-113">On the Scope parameters FastTab, select a scope for the number sequence and select scope values.</span></span>     <span data-ttu-id="7a972-114">Apimtis nustato, kokios organizacijos naudoja numeraciją.</span><span class="sxs-lookup"><span data-stu-id="7a972-114">The scope defines which organizations use the number sequence.</span></span> <span data-ttu-id="7a972-115">Be to, numeracijose, kurių aprėptis ne Bendrai naudojama, o kitokia, gali būti segmentų, atitinkančių jų aprėptį.</span><span class="sxs-lookup"><span data-stu-id="7a972-115">In addition, number sequences that have a scope other than Shared can have segments that correspond to their scope.</span></span> <span data-ttu-id="7a972-116">Pvz., numeracijoje, kurios aprėptis Juridinio subjekto, gali būti juridinio subjekto segmentas.</span><span class="sxs-lookup"><span data-stu-id="7a972-116">For example, a number sequence with a scope of Legal entity can have a legal entity segment.</span></span> <span data-ttu-id="7a972-117">Daugiau informacijos apie aprėptis žr. žinyno temoje „Numeracijos apžvalga“.</span><span class="sxs-lookup"><span data-stu-id="7a972-117">For more information about scopes, see the "Number sequence overview" help topic.</span></span>  
6. <span data-ttu-id="7a972-118">Išplėskite skyrių Segmentai.</span><span class="sxs-lookup"><span data-stu-id="7a972-118">Expand the Segments section.</span></span>
    * <span data-ttu-id="7a972-119">„FastTab“ skirtuke Segmentai apibrėžkite numeracijos formatą įtraukdami, pašalindami ir pertvarkydami segmentus.</span><span class="sxs-lookup"><span data-stu-id="7a972-119">On the Segments FastTab, define the format for the number sequence by adding, removing, and rearranging segments.</span></span>  
    * <span data-ttu-id="7a972-120">Visų aprėpčių numeracijose gali būti pastoviųjų segmentų ir raidinių-skaitinių segmentų.</span><span class="sxs-lookup"><span data-stu-id="7a972-120">Number sequences of all scopes can contain Constant segments and Alphanumeric segments.</span></span> <span data-ttu-id="7a972-121">Pastoviuosiuose segmentuose yra raidinių-skaitinių simbolių, kurie nekinta.</span><span class="sxs-lookup"><span data-stu-id="7a972-121">Constant segments contain a set of alphanumeric characters that do not change.</span></span> <span data-ttu-id="7a972-122">Naudokite šį segmentų tipą, kad tarp numeracijos segmentų įtrauktumėte brūkšnelį ar kitų skyriklių.</span><span class="sxs-lookup"><span data-stu-id="7a972-122">Use this segment type to add a hyphen or other separators between number sequence segments.</span></span> <span data-ttu-id="7a972-123">Skaitiniuose-raidiniuose segmentuose yra skaičių ženklų (#) ir ampersandų (&).</span><span class="sxs-lookup"><span data-stu-id="7a972-123">Alphanumeric segments contain a combination of number signs (#) and ampersands (&).</span></span> <span data-ttu-id="7a972-124">Šie simboliai nurodo raides ir skaičius, kurie padidėja kaskart panaudojus skaičių iš sekos.</span><span class="sxs-lookup"><span data-stu-id="7a972-124">These characters represent letters and numbers that increment every time that a number from the sequence is used.</span></span> <span data-ttu-id="7a972-125">Naudokite skaičiaus ženklą (#) norėdami nurodyti didėjančius skaičius ir ampersandus (&) norėdami nurodyti didėjančias raides.</span><span class="sxs-lookup"><span data-stu-id="7a972-125">Use a number sign (#) to indicate incrementing numbers and an ampersand (&) to indicate incrementing letters.</span></span> <span data-ttu-id="7a972-126">Pvz., pagal formatą #####_2014 sukuriamos sekos 00001_2014, 00002_2014 ir t.t.</span><span class="sxs-lookup"><span data-stu-id="7a972-126">For example, the format #####_2014 creates the sequence 00001_2014, 00002_2014, and so on.</span></span>     <span data-ttu-id="7a972-127">Turi būti bent vienas segmentas, sudarytas ir raidžių ir skaitmenų.</span><span class="sxs-lookup"><span data-stu-id="7a972-127">At least one alphanumeric segment must be present.</span></span> <span data-ttu-id="7a972-128">Apimties segmentai, pvz., įmonė arba juridinis subjektas, nėra būtini.</span><span class="sxs-lookup"><span data-stu-id="7a972-128">Scope segments, such as company or legal entity, are not required.</span></span> <span data-ttu-id="7a972-129">Tačiau jei neįtrauksite apimties segmentų į formatą, pasirinktos nuorodos skaičiai bus vis tiek generuojami pagal apimtį.</span><span class="sxs-lookup"><span data-stu-id="7a972-129">However, if you do not include scope segments in the format, numbers for the selected reference are still generated per scope.</span></span>  
7. <span data-ttu-id="7a972-130">Išplėskite dalį Nuorodos.</span><span class="sxs-lookup"><span data-stu-id="7a972-130">Expand the References section.</span></span>
    * <span data-ttu-id="7a972-131">„FastTab“ skirtuke Nuorodos pasirinkite dokumento tipą arba įrašą, kuriam norite priskirti šią numeraciją.</span><span class="sxs-lookup"><span data-stu-id="7a972-131">On the References FastTab, select the document type or record to assign this number sequence to.</span></span>     <span data-ttu-id="7a972-132">Šis veiksmas nėra būtinas dirbant su sekomis, kurios nurodomos pagal specialius programos naudojimo modelius.</span><span class="sxs-lookup"><span data-stu-id="7a972-132">This step is optional for sequences that are defined for special application usage patterns.</span></span> <span data-ttu-id="7a972-133">Šiais scenarijais naujas skaičius generuojamas naudojant numeracijos kodo arba ID reikšmę nenaudojant nuorodos.</span><span class="sxs-lookup"><span data-stu-id="7a972-133">In these scenarios, a new number is generated by using the value of a number sequence code or ID, without using a reference.</span></span> <span data-ttu-id="7a972-134">Specialiojo programos naudojimo modelio pavyzdys yra kvitų seriją, kuri naudojama konkrečiuose žurnalo pavadinimuose.</span><span class="sxs-lookup"><span data-stu-id="7a972-134">An example of a special application usage pattern is a voucher series that is used for specific journal names.</span></span> <span data-ttu-id="7a972-135">Tačiau nerekomenduojama naudoti tokių modelių.</span><span class="sxs-lookup"><span data-stu-id="7a972-135">However, we do not recommend that you use such patterns.</span></span>  
8. <span data-ttu-id="7a972-136">Išplėskite skyrių Bendra.</span><span class="sxs-lookup"><span data-stu-id="7a972-136">Expand the General section.</span></span>
    * <span data-ttu-id="7a972-137">„FastTab“ skirtuke Bendra nurodykite, ar numeracija yra neautomatinė, ar tęstinė, ar netęstinė.</span><span class="sxs-lookup"><span data-stu-id="7a972-137">On the General FastTab, specify whether the number sequence is manual, and continuous or non-continuous.</span></span> <span data-ttu-id="7a972-138">Be to, galite įvesti mažiausią ir didžiausią skaičius, kuriuos galima naudoti numeracijoje.</span><span class="sxs-lookup"><span data-stu-id="7a972-138">In addition, enter the lowest and highest numbers that can be used in the number sequence.</span></span>     <span data-ttu-id="7a972-139">Nerekomenduojama keisti netęstinių numeracijų į tęstines numeracijas.</span><span class="sxs-lookup"><span data-stu-id="7a972-139">We do not recommend changing a non-continuous number sequence to a continuous number sequence.</span></span> <span data-ttu-id="7a972-140">Numeracija nebus tikrai tęstinė.</span><span class="sxs-lookup"><span data-stu-id="7a972-140">The number sequence will not be truly continuous.</span></span> <span data-ttu-id="7a972-141">Dėl tokio keitimo taip pat gali įvykti besidubliuojančių raktų pažeidimų duomenų bazėje.</span><span class="sxs-lookup"><span data-stu-id="7a972-141">This change may also cause duplicate key violations in the database.</span></span> <span data-ttu-id="7a972-142">Be to, tęstinės numeracijos turi daugiau įtakos našumui.</span><span class="sxs-lookup"><span data-stu-id="7a972-142">In addition, continuous number sequences have a larger effect on performance.</span></span>   
9. <span data-ttu-id="7a972-143">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="7a972-143">Click Save.</span></span>

