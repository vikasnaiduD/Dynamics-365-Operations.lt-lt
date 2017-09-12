--- 
title: "Nustatyti ir generuoti gautinų sumų skirstymo pagal terminus informaciją"
description: "Šis vadovas jums padės nustatyti skirstymo pagal terminus laikotarpio apibrėžtį, pagal terminus skirstyti klientų balansus ir peržiūrėti balansus sąraše Pagal terminus suskirstytas balansas ir puslapyje Mokėjimų priežiūra."
author: mikefalkner
manager: AnnBe
ms.date: 11/14/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Global
ms.author: mfalkner
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 2e9f393acaa47d485a583b99ace459474f30be6a
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-and-generate-accounts-receivable-aging-information"></a><span data-ttu-id="bf818-103">Nustatyti ir generuoti gautinų sumų skirstymo pagal terminus informaciją</span><span class="sxs-lookup"><span data-stu-id="bf818-103">Set up and generate accounts receivable aging information</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="bf818-104">Šis vadovas jums padės nustatyti skirstymo pagal terminus laikotarpio apibrėžtį, pagal terminus skirstyti klientų balansus ir peržiūrėti balansus sąraše Pagal terminus suskirstytas balansas ir puslapyje Mokėjimų priežiūra.</span><span class="sxs-lookup"><span data-stu-id="bf818-104">This guide will help you set up an aging period definition, age customer balances, and view balances in the Aged balance list and the Collections page.</span></span> <span data-ttu-id="bf818-105">Šiame įraše naudojama demonstracinė įmonė USMF.</span><span class="sxs-lookup"><span data-stu-id="bf818-105">This recording uses the USMF demo company.</span></span>


## <a name="create-an-aging-period-definition"></a><span data-ttu-id="bf818-106">Kurti skirstymo pagal terminus laikotarpio apibrėžtį</span><span class="sxs-lookup"><span data-stu-id="bf818-106">Create an aging period definition</span></span>
1. <span data-ttu-id="bf818-107">Pasirinkite Kreditas ir mokėjimai > Nustatymas > Skirstymo pagal terminus laikotarpių apibrėžtys.</span><span class="sxs-lookup"><span data-stu-id="bf818-107">Go to Credit and collections > Setup > Aging period definitions.</span></span>
2. <span data-ttu-id="bf818-108">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="bf818-108">Click New.</span></span>
3. <span data-ttu-id="bf818-109">Lauke Skirstymo pagal terminus laikotarpio apibrėžtis surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="bf818-109">In the Aging period definition field, type a value.</span></span>
4. <span data-ttu-id="bf818-110">Lauke Aprašas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="bf818-110">In the Description field, type a value.</span></span>
5. <span data-ttu-id="bf818-111">Spustelėję Įtraukti po, įterpsite naują skirstymo pagal terminus laikotarpį.</span><span class="sxs-lookup"><span data-stu-id="bf818-111">Click Add below to insert a new aging period.</span></span>
6. <span data-ttu-id="bf818-112">Lauke Laikotarpis įveskite aprašą, kuris bus rodomas skirstymo pagal terminus ataskaitose.</span><span class="sxs-lookup"><span data-stu-id="bf818-112">In the Period field, enter the description to show on aging reports.</span></span>
7. <span data-ttu-id="bf818-113">Lauke Vienetas įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="bf818-113">In the Unit field, enter a number.</span></span>
8. <span data-ttu-id="bf818-114">Lauke Intervalas pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="bf818-114">In the Interval field, select an option.</span></span>
    * <span data-ttu-id="bf818-115">DK laikotarpis suderina laikotarpį su DK kalendoriumi.</span><span class="sxs-lookup"><span data-stu-id="bf818-115">Ledger period matches the period to your ledger calendar.</span></span> <span data-ttu-id="bf818-116">Diena, savaite, mėnesiu, ketvirčiu ir metais pagal datos tipą apibrėžiamas intervalas.</span><span class="sxs-lookup"><span data-stu-id="bf818-116">Day, week, month, quarter and years define the size of the interval by date type.</span></span> <span data-ttu-id="bf818-117">Parinktis Neribotas pasirenka visas operacijas prieš ankstesnį laikotarpį arba po jo – tai priklauso nuo to, ar tai pirmas, ar paskutinis laikotarpis.</span><span class="sxs-lookup"><span data-stu-id="bf818-117">Unlimited selects all transactions before or after the previous period, depending on whether it is the first or last period.</span></span>  
9. <span data-ttu-id="bf818-118">Lauke Skirstymo pagal terminus indikatorius pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="bf818-118">In the Aging indicator field, select an option.</span></span>
10. <span data-ttu-id="bf818-119">Pasirinkite laikotarpį tinklelio viršuje.</span><span class="sxs-lookup"><span data-stu-id="bf818-119">Select the period at the top of the grid.</span></span> <span data-ttu-id="bf818-120">Atnaujinti aprašą, kad būtų apibūdintas seniausias skirstymo pagal terminus laikotarpio apibrėžties laikotarpis</span><span class="sxs-lookup"><span data-stu-id="bf818-120">Update the description to describe the oldest period in the aging period definition</span></span>
11. <span data-ttu-id="bf818-121">Lauke Laikotarpis įveskite naują skirstymo pagal terminus laikotarpio aprašą.</span><span class="sxs-lookup"><span data-stu-id="bf818-121">In the Period field, enter the new description of the aging period.</span></span>
12. <span data-ttu-id="bf818-122">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="bf818-122">Close the page.</span></span>

## <a name="age-the-balances"></a><span data-ttu-id="bf818-123">Balansus skirstyti pagal terminus</span><span class="sxs-lookup"><span data-stu-id="bf818-123">Age the balances</span></span>
1. <span data-ttu-id="bf818-124">Pasirinkite Kreditas ir mokėjimai > Periodinės užduotys > Pagal terminus suskirstyti klientų balansus.</span><span class="sxs-lookup"><span data-stu-id="bf818-124">Go to Credit and collections > Periodic tasks > Age customer balances.</span></span>
2. <span data-ttu-id="bf818-125">Lauke Skirstymo pagal terminus laikotarpio apibrėžtis pasirinkite savo sukurtą skirstymo pagal terminus laikotarpio apibrėžtį.</span><span class="sxs-lookup"><span data-stu-id="bf818-125">In the Aging period definition field, select the aging period definition that you created.</span></span>
    * <span data-ttu-id="bf818-126">Kiekvienos skirstymo pagal terminus laikotarpio apibrėžties galite turėti vieną momentinę kopiją.</span><span class="sxs-lookup"><span data-stu-id="bf818-126">You can have one active snapshot for each aging period definition.</span></span>  
    * <span data-ttu-id="bf818-127">Visi klientai apdorojami pagal numatytąsias nuostatas.</span><span class="sxs-lookup"><span data-stu-id="bf818-127">All customers are processed by default.</span></span> <span data-ttu-id="bf818-128">Šią pasirinktį galite naudoti apskaičiuoti vienam klientų mokėjimų priežiūros telkiniui.</span><span class="sxs-lookup"><span data-stu-id="bf818-128">You can use this selection to calculate a single collections pool of customers.</span></span>  
    * <span data-ttu-id="bf818-129">Iš operacijos pasirinkite datą, kurią naudosite skirstydami pagal terminus.</span><span class="sxs-lookup"><span data-stu-id="bf818-129">Select the date from the transaction that you will use for the aging.</span></span>  
    * <span data-ttu-id="bf818-130">Skirstymo pagal terminus datą pasirinkite „nuo‟.</span><span class="sxs-lookup"><span data-stu-id="bf818-130">Select an "as of" date for aging.</span></span> <span data-ttu-id="bf818-131">Numatytoji data yra šiandienos, tačiau, šį lauką pakeitę į Pasirinkta data, galėsite pasirinkti norimą datą.</span><span class="sxs-lookup"><span data-stu-id="bf818-131">The default is today but, if you change this field to Selected date, you will be able to pick the date that you want.</span></span> <span data-ttu-id="bf818-132">Paketiniam vykdymui naudokite šiandienos datą.</span><span class="sxs-lookup"><span data-stu-id="bf818-132">For batch processing, use Today's date.</span></span>  
3. <span data-ttu-id="bf818-133">Išplėskite įmonių diapazoną.</span><span class="sxs-lookup"><span data-stu-id="bf818-133">Expand the Company range.</span></span> <span data-ttu-id="bf818-134">Galite pasirinkti įmones, kurios bus įtrauktos į momentinę kopiją.</span><span class="sxs-lookup"><span data-stu-id="bf818-134">You can select the companies that will be included in the snapshot.</span></span> <span data-ttu-id="bf818-135">Dabartinė įmonė pasirenkama pagal numatytąsias nuostatas.</span><span class="sxs-lookup"><span data-stu-id="bf818-135">The current company is selected by default.</span></span>
4. <span data-ttu-id="bf818-136">Norėdami apdoroti momentinę kopiją, spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="bf818-136">Click Ok to process the snapshot.</span></span> <span data-ttu-id="bf818-137">Apdorojimas šiek tiek užtruks, tad palaukite, kol išnyks slankiklis ir patikrinkite, ar pranešimų centre nėra pranešimo.</span><span class="sxs-lookup"><span data-stu-id="bf818-137">It will take some time so wait for the slider to disappear and check the message center for a message.</span></span>

## <a name="view-the-balances-on-the-aged-balances-list-and-on-the-collection-page"></a><span data-ttu-id="bf818-138">Peržiūrėti balansus sąraše Pagal terminus suskirstyti balansai ir puslapyje Rinkinys</span><span class="sxs-lookup"><span data-stu-id="bf818-138">View the balances on the Aged balances list and on the Collection page</span></span>
1. <span data-ttu-id="bf818-139">Pasirinkite Kreditas ir rinkiniai > Rinkiniai > Pagal terminus suskirstyti balansai.</span><span class="sxs-lookup"><span data-stu-id="bf818-139">Go to Credit and collections > Collections > Aged balances.</span></span>
    * <span data-ttu-id="bf818-140">Sąrašo puslapyje rodomi kliento balansai.</span><span class="sxs-lookup"><span data-stu-id="bf818-140">The list page shows the balances for the customer.</span></span> <span data-ttu-id="bf818-141">Skirstymo pagal terminus piktograma rodo seniausios operacijos skirstymo pagal terminus laikotarpį.</span><span class="sxs-lookup"><span data-stu-id="bf818-141">The aging icon shows the aging period for the oldest transaction.</span></span>  
2. <span data-ttu-id="bf818-142">Pasirinkite klientą, turintį balansą.</span><span class="sxs-lookup"><span data-stu-id="bf818-142">Select a customer with a balance.</span></span>
3. <span data-ttu-id="bf818-143">Norėdami peržiūrėti pagal terminus suskirstytus balansus, išplėskite „FactBox‟ Skirstymas pagal terminus sritį.</span><span class="sxs-lookup"><span data-stu-id="bf818-143">Expand the Aging fact box area to view the aged balances.</span></span>
    * <span data-ttu-id="bf818-144">„FactBox‟ skirstymo pagal terminus laikotarpio apibrėžtis paimama iš numatytosios skirstymo pagal terminus apibrėžties, nurodytos parametruose.</span><span class="sxs-lookup"><span data-stu-id="bf818-144">The aging period definition for the fact box is taken from the default aging period definition specified in the parameters.</span></span> <span data-ttu-id="bf818-145">Ją keisti galite naudodami meniu Rinkti.</span><span class="sxs-lookup"><span data-stu-id="bf818-145">You can change it using the Collect menu.</span></span>  

