--- 
title: "Nustatyti vežėjo degalų indeksus"
description: "Šis vadovas parodo, kaip sukurti degalų indekso regioną, degalų indeksą ir vežėjo degalų indeksą."
author: BibiSp
manager: AnnBe
ms.date: 11/14/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: bis
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 81f3244ff42cf13cd93ac10656c47f8a9204ef99
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-a-carrier-fuel-index"></a><span data-ttu-id="e57b6-103">Nustatyti vežėjo degalų indeksus</span><span class="sxs-lookup"><span data-stu-id="e57b6-103">Set up a carrier fuel index</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="e57b6-104">Šis vadovas parodo, kaip sukurti degalų indekso regioną, degalų indeksą ir vežėjo degalų indeksą.</span><span class="sxs-lookup"><span data-stu-id="e57b6-104">This guide shows how to create a fuel index region, a fuel index and a carrier fuel index.</span></span> <span data-ttu-id="e57b6-105">Degalų indekso regionas nurodo, kuriam regionui turėtų būti taikomas degalų indeksas, o degalų indeksas tam tikro laikotarpio degalų kainą.</span><span class="sxs-lookup"><span data-stu-id="e57b6-105">The fuel index region specifies which region the fuel index should apply to, and the fuel index specifies a fuel price for a particular period of time.</span></span> <span data-ttu-id="e57b6-106">Norėdami įvertinti degalų kainų pokyčius per tam tikrą laiką, galite susieti vežėją su keliais degalų indeksais.</span><span class="sxs-lookup"><span data-stu-id="e57b6-106">To reflect the change in fuel prices over time, you can associate multiple fuel indexes with a carrier.</span></span>  <span data-ttu-id="e57b6-107">Šias užduotis paprastai atlieka transportavimo koordinatorius.</span><span class="sxs-lookup"><span data-stu-id="e57b6-107">These tasks are normally done by a transportation coordinator.</span></span> <span data-ttu-id="e57b6-108">Šią procedūrą galite atlikti demonstracinių duomenų įmonėje USMF arba naudodami savo duomenis.</span><span class="sxs-lookup"><span data-stu-id="e57b6-108">You can use this procedure in demo data company USMF or using your own data.</span></span>


## <a name="create-a-fuel-index-region"></a><span data-ttu-id="e57b6-109">Kurti degalų indekso regioną</span><span class="sxs-lookup"><span data-stu-id="e57b6-109">Create a fuel index region</span></span>
1. <span data-ttu-id="e57b6-110">Pasirinkite Transportavimo valdymas > Nustatymas > Degalų indeksai > Degalų indekso regionai.</span><span class="sxs-lookup"><span data-stu-id="e57b6-110">Go to Transportation management > Setup > Fuel indexes > Fuel index regions.</span></span>
    * <span data-ttu-id="e57b6-111">Pirmiausia turite sukurti skirtingus savo veiklos regionus ir apskaičiuoti skirtingus papildomus degalų mokesčius.</span><span class="sxs-lookup"><span data-stu-id="e57b6-111">First you have to create the different regions, where you operate and calculate different fuel surcharges.</span></span>  
2. <span data-ttu-id="e57b6-112">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="e57b6-112">Click New.</span></span>
3. <span data-ttu-id="e57b6-113">Lauke „Regionas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e57b6-113">In the Region field, type a value.</span></span>
4. <span data-ttu-id="e57b6-114">Lauke Pavadinimas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e57b6-114">In the Name field, type a value.</span></span>
5. <span data-ttu-id="e57b6-115">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="e57b6-115">Click Save.</span></span>

## <a name="create-a-fuel-index"></a><span data-ttu-id="e57b6-116">Degalų indekso kūrimas</span><span class="sxs-lookup"><span data-stu-id="e57b6-116">Create a fuel index</span></span>
1. <span data-ttu-id="e57b6-117">Pasirinkite Transportavimo valdymas > Nustatymas > Degalų indeksai > Degalų indeksai.</span><span class="sxs-lookup"><span data-stu-id="e57b6-117">Go to Transportation management > Setup > Fuel indexes > Fuel indexes.</span></span>
    * <span data-ttu-id="e57b6-118">Savo nustatytiems regionams turite įvesti dabartines degalų kainas.</span><span class="sxs-lookup"><span data-stu-id="e57b6-118">For the regions you have set up you need to enter the current prices for the fuel.</span></span>  
2. <span data-ttu-id="e57b6-119">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="e57b6-119">Click New.</span></span>
3. <span data-ttu-id="e57b6-120">Lauke „Regionas“ spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="e57b6-120">In the Region field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="e57b6-121">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="e57b6-121">In the list, click the link in the selected row.</span></span>
5. <span data-ttu-id="e57b6-122">Lauke „Kaina už galoną“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e57b6-122">In the Price per gallon field, enter a number.</span></span>
6. <span data-ttu-id="e57b6-123">Lauke „Įsigaliojimo pradžios data ir laikas“ įveskite datą ir laiką.</span><span class="sxs-lookup"><span data-stu-id="e57b6-123">In the Effective start date and time field, enter a date and time.</span></span>
7. <span data-ttu-id="e57b6-124">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="e57b6-124">Click Save.</span></span>

## <a name="create-a-carrier-fuel-index"></a><span data-ttu-id="e57b6-125">Kurti vežėjo degalų indeksą</span><span class="sxs-lookup"><span data-stu-id="e57b6-125">Create a Carrier fuel index</span></span>
1. <span data-ttu-id="e57b6-126">Pasirinkite Transportavimo valdymas > Nustatymas > Degalų indeksai > Vežėjo degalų indeksai.</span><span class="sxs-lookup"><span data-stu-id="e57b6-126">Go to Transportation management > Setup > Fuel indexes > Carrier fuel indexes.</span></span>
2. <span data-ttu-id="e57b6-127">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="e57b6-127">Click New.</span></span>
3. <span data-ttu-id="e57b6-128">Lauke „Vežėjo degalų indeksas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e57b6-128">In the Carrier fuel index field, type a value.</span></span>
4. <span data-ttu-id="e57b6-129">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e57b6-129">In the Description field, type a value.</span></span>
5. <span data-ttu-id="e57b6-130">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="e57b6-130">Click New.</span></span>
6. <span data-ttu-id="e57b6-131">Lauke „Įsigaliojimo pradžios data ir laikas“ įveskite datą ir laiką.</span><span class="sxs-lookup"><span data-stu-id="e57b6-131">In the Effective start date and time field, enter a date and time.</span></span>
7. <span data-ttu-id="e57b6-132">Lauke „PPG nuo“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e57b6-132">In the PPG From field, enter a number.</span></span>
    * <span data-ttu-id="e57b6-133">Šiame pavyzdyje laukui „PPG nuo“ galite nustatyti reikšmę 1.95.</span><span class="sxs-lookup"><span data-stu-id="e57b6-133">In this example, you can set PPG From field to 1.95.</span></span>  
8. <span data-ttu-id="e57b6-134">Lauke „PPG iki“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e57b6-134">In the PPG To field, enter a number.</span></span>
    * <span data-ttu-id="e57b6-135">Šiame pavyzdyje laukui „PPG iki“ galite nustatyti reikšmę 2.</span><span class="sxs-lookup"><span data-stu-id="e57b6-135">In this example you can set the PPG To field to 2.</span></span>  
9. <span data-ttu-id="e57b6-136">Lauke Procentas įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e57b6-136">In the Percentage field, enter a number.</span></span>
    * <span data-ttu-id="e57b6-137">Šiame pavyzdyje galite nustatyti procentinę reikšmę 3.</span><span class="sxs-lookup"><span data-stu-id="e57b6-137">In this example you can set the percentage to 3.</span></span>  
10. <span data-ttu-id="e57b6-138">Lauke Valiuta spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="e57b6-138">In the Currency field, click the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="e57b6-139">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="e57b6-139">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="e57b6-140">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="e57b6-140">In the list, click the link in the selected row.</span></span>
13. <span data-ttu-id="e57b6-141">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="e57b6-141">Click Save.</span></span>

