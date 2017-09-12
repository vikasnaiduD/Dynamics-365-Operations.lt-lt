---
title: "Nustatyti gaunamų prekių apžvalgos profilį"
description: "Šios užduoties tikslas yra nustatyti gaunamų prekių apžvalgos profilį."
author: perlynne
manager: AnnBe
ms.date: 11/14/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: bis
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 0e7f66cccd76e5326fce75d1a13aff294c16fb9b
ms.openlocfilehash: 9d4377f4ebf777258de13a2d2cd0a3a095f98fdd
ms.contentlocale: lt-lt
ms.lasthandoff: 09/12/2017

---
# <a name="set-up-an-item-arrival-overview-profile"></a><span data-ttu-id="1fcfe-103">Nustatyti gaunamų prekių apžvalgos profilį</span><span class="sxs-lookup"><span data-stu-id="1fcfe-103">Set up an item arrival overview profile</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="1fcfe-104">Šios užduoties tikslas yra nustatyti gaunamų prekių apžvalgos profilį.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-104">This task focuses on the setup of an arrival overview profile.</span></span> <span data-ttu-id="1fcfe-105">Gaunamų prekių apžvalgos profilis yra rinkinys taisyklių, kurios taikomos, kai vartotojas atidaro puslapį „Gaunamų prekių apžvalga“.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-105">The arrival overview profile is a collection of rules that will be applied when the Arrival overview page is opened by a user.</span></span> <span data-ttu-id="1fcfe-106">Šią procedūrą galite naudoti demonstracinių duomenų įmonėje USMF.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-106">You can use this procedure in demo data company USMF.</span></span> <span data-ttu-id="1fcfe-107">Šią procedūrą paprastai atlieka gavimo klerkas.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-107">This procedure would typically be carried out by a receiving clerk.</span></span>





1. <span data-ttu-id="1fcfe-108">Pasirinkite Atsargų valdymas > Nustatymas > Paskirstymas > Gaunamų prekių apžvalgos profiliai.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-108">Go to Inventory management > Setup > Distribution > Arrival overview profiles.</span></span>
2. <span data-ttu-id="1fcfe-109">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-109">Click New.</span></span>
    * <span data-ttu-id="1fcfe-110">Beveik visada teks dirbti tame pačiame sandėlyje iškraunant krovinių pilnus sunkvežimius, todėl turėtumėte sukurti gaunamų prekių apžvalgos profilį, kad supaprastintumėte gautų prekių registravimo procesą.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-110">Because you will almost always work in the same warehouse offloading full truck loads, you should create an arrival overview profile to simplify the process of registering received items.</span></span>  
3. <span data-ttu-id="1fcfe-111">Lauke „Gaunamų prekių apžvalgos profilio pavadinimas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-111">In the Arrival overview profile name field, type a value.</span></span>
4. <span data-ttu-id="1fcfe-112">Lauke „Rodyti eilutes“ pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-112">In the Show lines field, select an option.</span></span>
    * <span data-ttu-id="1fcfe-113">Pasirinkite, kurias gaunamų prekių eilutes rodyti: Visos – rodyti visas eilutes, neatsižvelgiant į būseną.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-113">Select which lines to show for the receipts:   All – Show all lines, regardless of status.</span></span>   <span data-ttu-id="1fcfe-114">Vykdoma – rodyti gaunamų prekių eilutes, kurių vykdymo būsena yra „Baigta“ arba „Iš dalies“.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-114">In progress – Show lines for receipts in which the progress is Complete or Partly.</span></span> <span data-ttu-id="1fcfe-115">Tai reiškia, kad kiekvienai eilutei gaunamų prekių žurnale užregistruotas visas kiekis arba dalis kiekio.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-115">This means that for each line, either the full quantity or part of the quantity has been registered in an arrival journal.</span></span>   <span data-ttu-id="1fcfe-116">Nebaigta – rodyti gaunamų prekių eilutes, kurių vykdymo būsena yra „Nėra“ arba „Iš dalies“.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-116">Not complete – Show lines for receipts in which the progress is None or Partly.</span></span> <span data-ttu-id="1fcfe-117">Tai reiškia, kad kiekvienai eilutei gavimo žurnale buvo užregistruota dalis kiekio arba kiekio užregistruota nebuvo.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-117">This means that for each line, nothing or only part of the quantity has been registered in an arrival journal.</span></span>  
5. <span data-ttu-id="1fcfe-118">Išplėskite arba sutraukite skyrių Gavimo parinktys.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-118">Expand or collapse the Arrival options section.</span></span>
6. <span data-ttu-id="1fcfe-119">Lauke „Dienos nuo šiandienos“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-119">In the Days forward field, type a value.</span></span>
    * <span data-ttu-id="1fcfe-120">Nustato filtrą, kad būtų rodomos per artimiausias kelias dienas numatomų gauti gaunamų prekių eilutės (atsižvelgiant į jūsų nustatytą skaičių).</span><span class="sxs-lookup"><span data-stu-id="1fcfe-120">This sets a filter to show the receipt lines expected to be received within the next few days (depending on the number you set).</span></span>  
7. <span data-ttu-id="1fcfe-121">Lauke „Dienos iki šiandienos“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-121">In the Days back field, type a value.</span></span>
    * <span data-ttu-id="1fcfe-122">Nustato filtrą, kad būtų rodomos prieš kelias dienas numatytų gauti gaunamų prekių eilutės.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-122">This sets a filter to show the receipt lines expected to be received a number of days before today.</span></span>  
8. <span data-ttu-id="1fcfe-123">Lauke „Sandėliai“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-123">In the Warehouses field, type a value.</span></span>
    * <span data-ttu-id="1fcfe-124">Filtruokite vieną ar daugiau sandėlių.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-124">Filter on one or more warehouses.</span></span>  
9. <span data-ttu-id="1fcfe-125">Lauke Pristatymo būdas pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-125">In the Mode of delivery field, select a value.</span></span>
    * <span data-ttu-id="1fcfe-126">Nustato filtrą, kad būtų rodomos tik šio pristatymo būdo gaunamų prekių eilutės.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-126">This sets a filter to show only the receipt lines with this Mode of delivery.</span></span>  
10. <span data-ttu-id="1fcfe-127">Lauke Pavadinimas pasirinkite WHS.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-127">In the Name field, select WHS.</span></span>
11. <span data-ttu-id="1fcfe-128">Lauke Sandėlis pasirinkite 24-ąjį sandėlį.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-128">In the Warehouse field, select warehouse 24.</span></span>
    * <span data-ttu-id="1fcfe-129">Tai numatytasis sandėlis, kuris bus naudojamas registruotoms šio profilio gaunamų prekių eilutėms.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-129">This is the default warehouse that will be used for registered receipt lines that use this profile.</span></span>  
12. <span data-ttu-id="1fcfe-130">Lauke Vieta pasirinkite Baydoor.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-130">In the Location field, select Baydoor.</span></span>
    * <span data-ttu-id="1fcfe-131">Tai numatytoji vieta, kuri bus naudojama registruotoms šio profilio gaunamų prekių eilutėms.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-131">This is the default location that will be used for registered receipt lines that use this profile.</span></span>  
13. <span data-ttu-id="1fcfe-132">Išplėskite arba sutraukite skyrių Gavimo užklausos informacija.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-132">Expand or collapse the Arrival query details section.</span></span>
14. <span data-ttu-id="1fcfe-133">Lauke Apribota teritorija pasirinkite 2-ąją teritoriją.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-133">In the Restrict to site field, select site 2.</span></span>
    * <span data-ttu-id="1fcfe-134">Nustato filtrą, kad būtų rodomos tik šios teritorijos gaunamų prekių eilutės.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-134">This sets a filter to show only the receipt lines with this site.</span></span>  
15. <span data-ttu-id="1fcfe-135">Nustatykite parinktį Pirkimo užsakymai į Taip.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-135">Set the Purchase orders option to Yes.</span></span>
    * <span data-ttu-id="1fcfe-136">Pasirinkite gaunamų prekių eilutes iš pirkimo užsakymų.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-136">Select receipt lines from purchase orders.</span></span>  
16. <span data-ttu-id="1fcfe-137">Nustatykite parinktį Perkėlimo užsakymai į Taip.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-137">Set the Transfer orders option to Yes.</span></span>
    * <span data-ttu-id="1fcfe-138">Pasirinkite gaunamų prekių eilutes iš perkėlimo užsakymų.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-138">Select receipt lines from transfer orders.</span></span>  
17. <span data-ttu-id="1fcfe-139">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-139">Click Save.</span></span>
18. <span data-ttu-id="1fcfe-140">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="1fcfe-140">Close the page.</span></span>
