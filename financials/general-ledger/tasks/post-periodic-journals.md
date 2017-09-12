--- 
title: "Registruoti periodinius žurnalus"
description: "Periodiniai žurnalai kartais vadinami pasikartojančias žurnalais nes suma, tekstas ir kitą informaciją kartojasi kiekvieną kartą, kai periodinis žurnalas nuskaitomas."
author: aprilolson
manager: AnnBe
ms.date: 02/24/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 233d145a9d3441ffc2b816b8514e58988b517136
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="post-periodic-journals"></a><span data-ttu-id="984c9-103">Registruoti periodinius žurnalus</span><span class="sxs-lookup"><span data-stu-id="984c9-103">Post periodic journals</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="984c9-104">Periodiniai žurnalai kartais vadinami pasikartojančias žurnalais nes suma, tekstas ir kitą informaciją kartojasi kiekvieną kartą, kai periodinis žurnalas nuskaitomas.</span><span class="sxs-lookup"><span data-stu-id="984c9-104">Periodic journals are sometimes called recurring journals because the amount, text, and other information are repeated each time that the periodic journal is retrieved.</span></span> <span data-ttu-id="984c9-105">Sukūrę periodinį žurnalą, nurodote pasikartojimų laikotarpio intervalą pvz., dienas ar mėnesius.</span><span class="sxs-lookup"><span data-stu-id="984c9-105">When you create the periodic journal, you specify the period interval for the recurrence, such as days or months.</span></span> <span data-ttu-id="984c9-106">Šis užduočių vadovas sukurs tokį periodinį žurnalą, kurio pasikartojimas yra mėnesinis.</span><span class="sxs-lookup"><span data-stu-id="984c9-106">This task guide will create a periodic journal with a monthly recurrence.</span></span>



1. <span data-ttu-id="984c9-107">Eikite į Didžioji knyga > Periodinės užduotys > Periodiniai žurnalai.</span><span class="sxs-lookup"><span data-stu-id="984c9-107">Go to General ledger > Periodic tasks > Periodic journals.</span></span>
2. <span data-ttu-id="984c9-108">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="984c9-108">Click New.</span></span>
3. <span data-ttu-id="984c9-109">Lauke Pavadinimas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="984c9-109">In the Name field, enter or select a value.</span></span>
4. <span data-ttu-id="984c9-110">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="984c9-110">In the list, click the link in the selected row.</span></span>
5. <span data-ttu-id="984c9-111">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="984c9-111">In the Description field, type a value.</span></span>
    * <span data-ttu-id="984c9-112">Aprašą sudarys vėliau gauto periodinio žurnalo pavadinimas, todėl jį suteikite atitinkamą.</span><span class="sxs-lookup"><span data-stu-id="984c9-112">The description will be the name of the Periodic journal when retrieved later so make sure to give it a relevant name.</span></span>  
6. <span data-ttu-id="984c9-113">Spustelėkite Eilutės.</span><span class="sxs-lookup"><span data-stu-id="984c9-113">Click Lines.</span></span>
    * <span data-ttu-id="984c9-114">Periodinį žurnalą paprastai sudaro kelios eilutės.</span><span class="sxs-lookup"><span data-stu-id="984c9-114">A periodic journal will typically include several journal lines.</span></span> <span data-ttu-id="984c9-115">tačiau šis užduočių vadovas įtrauks tik vieną eilutę.</span><span class="sxs-lookup"><span data-stu-id="984c9-115">this task guide will however only add one line.</span></span>  
7. <span data-ttu-id="984c9-116">Lauke Data įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="984c9-116">In the Date field, enter a date.</span></span>
    * <span data-ttu-id="984c9-117">Lauke Data nurodyta kito perkėlimo į kasdienį žurnalą registravimo data.</span><span class="sxs-lookup"><span data-stu-id="984c9-117">The Date field contains the posting date for the next transfer to the daily journal.</span></span> <span data-ttu-id="984c9-118">Žurnaluose, kurie bus gaunami kiekvieną mėnesį, rekomenduojama naudoti datą tame mėnesyje, kada žurnlas bus registruojamas – paprastai tai pirmoji arba paskutinioji laikotarpio data.</span><span class="sxs-lookup"><span data-stu-id="984c9-118">For journals that will be retrieved each month it is recommended to use the date in the month when it will be posted, typically the first or last date in the period.</span></span> <span data-ttu-id="984c9-119">Galima lauką Data palikti tuščią, ir datą nurodyti, kai gaunamas žurnalas, naudojant lauką Tuščia data.</span><span class="sxs-lookup"><span data-stu-id="984c9-119">It is possible to leave the Date field blank and to give a date when the journal is retrieved, using the Empty date field.</span></span>    <span data-ttu-id="984c9-120">Kai operacijos nuskaitomos, laukas automatiškai atnaujinamas į kitą pasikartojančią datą.</span><span class="sxs-lookup"><span data-stu-id="984c9-120">The field is automatically updated to the next recurring date when transactions are retrieved.</span></span>  
8. <span data-ttu-id="984c9-121">Lauke Sąskaita nustatykite norimas reikšmes.</span><span class="sxs-lookup"><span data-stu-id="984c9-121">In the Account field, specify the desired values.</span></span>
9. <span data-ttu-id="984c9-122">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="984c9-122">In the Description field, type a value.</span></span>
10. <span data-ttu-id="984c9-123">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="984c9-123">Close the page.</span></span>
11. <span data-ttu-id="984c9-124">Lauke Debetas įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="984c9-124">In the Debit field, enter a number.</span></span>
12. <span data-ttu-id="984c9-125">Lauke Korespondentinė sąskaita nustatykite norimas reikšmes.</span><span class="sxs-lookup"><span data-stu-id="984c9-125">In the Offset account field, specify the desired values.</span></span>
13. <span data-ttu-id="984c9-126">Lauke Vienetas pasirinkite „Mėnesiai‟.</span><span class="sxs-lookup"><span data-stu-id="984c9-126">In the Unit field, select 'Months'.</span></span>
14. <span data-ttu-id="984c9-127">Lauke Vienetų skaičius įveskite „1‟.</span><span class="sxs-lookup"><span data-stu-id="984c9-127">In the Number of units field, enter '1'.</span></span>
15. <span data-ttu-id="984c9-128">Lauke Paskutinė data įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="984c9-128">In the Last date field, enter a date.</span></span>
    * <span data-ttu-id="984c9-129">Paskutinę datą įvedus į ankstesnį laikotarpį, nebus galima pasikartojančio žurnalo netyčia sukurti neteisingame pradžios laikotarpyje.</span><span class="sxs-lookup"><span data-stu-id="984c9-129">Entering last date in the preceding period will prevent that the recurring journal by mistake is created in the wrong starting period.</span></span> <span data-ttu-id="984c9-130">Paskutinė diena bus atnaujinama vėliau, kiekvieną kartą nuskaitant periodinį žurnalą.</span><span class="sxs-lookup"><span data-stu-id="984c9-130">Last date will later on be updated each time the periodic journal is retrieved.</span></span>  
16. <span data-ttu-id="984c9-131">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="984c9-131">Click Save.</span></span>
17. <span data-ttu-id="984c9-132">Eikite į Numatytoji ataskaitų sritis.</span><span class="sxs-lookup"><span data-stu-id="984c9-132">Go to Default dashboard.</span></span>
18. <span data-ttu-id="984c9-133">Pasirinkite Didžioji knyga > Žurnalų įrašai > Bendrieji žurnalai.</span><span class="sxs-lookup"><span data-stu-id="984c9-133">Go to General ledger > Journal entries > General journals.</span></span>
19. <span data-ttu-id="984c9-134">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="984c9-134">Click New.</span></span>
20. <span data-ttu-id="984c9-135">Lauke Pavadinimas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="984c9-135">In the Name field, enter or select a value.</span></span>
21. <span data-ttu-id="984c9-136">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="984c9-136">In the list, find and select the desired record.</span></span>
22. <span data-ttu-id="984c9-137">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="984c9-137">In the list, click the link in the selected row.</span></span>
23. <span data-ttu-id="984c9-138">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="984c9-138">In the Description field, type a value.</span></span>
24. <span data-ttu-id="984c9-139">Spustelėkite Eilutės.</span><span class="sxs-lookup"><span data-stu-id="984c9-139">Click Lines.</span></span>
25. <span data-ttu-id="984c9-140">Spustelėkite Periodinis žurnalas.</span><span class="sxs-lookup"><span data-stu-id="984c9-140">Click Period journal.</span></span>
26. <span data-ttu-id="984c9-141">Spustelėkite Nuskaityti žurnalą.</span><span class="sxs-lookup"><span data-stu-id="984c9-141">Click Retrieve journal.</span></span>
27. <span data-ttu-id="984c9-142">Lauke Pabaigos data įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="984c9-142">In the To date field, enter a date.</span></span>
    * <span data-ttu-id="984c9-143">Data Iki naudojama kaip periodinio kvito eilučių galutinė data.</span><span class="sxs-lookup"><span data-stu-id="984c9-143">The To date serves as the cutoff date for the periodic voucher lines.</span></span> <span data-ttu-id="984c9-144">Atsižvelgiant į pasikartojimo nuostatą, paskutinę datą ir datą Iki, gautame žurnale ta pati eilutė gali būti įtraukta daugiau nei vieną kartą.</span><span class="sxs-lookup"><span data-stu-id="984c9-144">Based on the recurrence setting, the Last date and To date the same line might be included more than once in the resulting journal.</span></span> <span data-ttu-id="984c9-145">Data Iki automatiškai atnaujinama pagal seanso datą, kada paskutinį kartą periodinė eilutė buvo perkelta į žurnalą.</span><span class="sxs-lookup"><span data-stu-id="984c9-145">To date is automatically updated based on  session date of the last time the periodic line was transferred to a journal.</span></span>  
28. <span data-ttu-id="984c9-146">Lauke Periodinio žurnalo numeris įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="984c9-146">In the Periodic journal number field, enter or select a value.</span></span>
29. <span data-ttu-id="984c9-147">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="984c9-147">In the list, click the link in the selected row.</span></span>
30. <span data-ttu-id="984c9-148">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="984c9-148">Click OK.</span></span>
    * <span data-ttu-id="984c9-149">Laikotarpio žurnalą dabar galima peržiūrėti, patvirtinti arba registruoti – tai priklauso nuo poreikio ir nustatymo.</span><span class="sxs-lookup"><span data-stu-id="984c9-149">The period journal can now be reviewed, approved or posted depending on requirement and setup.</span></span>  

