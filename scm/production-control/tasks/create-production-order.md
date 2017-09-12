--- 
title: "Kurti gamybos užsakymą"
description: "Šioje procedūroje nurodoma, kaip kurti gamybos užsakymą."
author: johanhoffmann
manager: AnnBe
ms.date: 11/11/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: johanho
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 9b947a02be981155053e33a4ef20e19bf2a194a5
ms.openlocfilehash: ac2ee418082aa6579424fc9480478587b7c22c6d
ms.contentlocale: lt-lt
ms.lasthandoff: 07/27/2017

---
# <a name="create-a-production-order"></a><span data-ttu-id="afdf7-103">Kurti gamybos užsakymą</span><span class="sxs-lookup"><span data-stu-id="afdf7-103">Create a production order</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="afdf7-104">Šioje procedūroje nurodoma, kaip kurti gamybos užsakymą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-104">This procedure shows how to create a production order.</span></span> <span data-ttu-id="afdf7-105">Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.</span><span class="sxs-lookup"><span data-stu-id="afdf7-105">The demo data company used to create this procedure is USMF.</span></span> <span data-ttu-id="afdf7-106">Tai yra pirmoji procedūra iš septynių, kurioje paaiškinamas gamybos užsakymo ciklas.</span><span class="sxs-lookup"><span data-stu-id="afdf7-106">This is the first procedure out of seven which explains the production order lifecycle.</span></span>


## <a name="create-a-production-order"></a><span data-ttu-id="afdf7-107">Kurti gamybos užsakymą</span><span class="sxs-lookup"><span data-stu-id="afdf7-107">Create a production order</span></span>
1. <span data-ttu-id="afdf7-108">Pasirinkite Gamybos kontrolė > Gamybos užsakymai > Visi gamybos užsakymai.</span><span class="sxs-lookup"><span data-stu-id="afdf7-108">Go to Production control > Production orders > All production orders.</span></span>
2. <span data-ttu-id="afdf7-109">Spustelėkite Naujas gamybos užsakymas.</span><span class="sxs-lookup"><span data-stu-id="afdf7-109">Click New production order.</span></span>
3. <span data-ttu-id="afdf7-110">Lauke „Prekės numeris“ įveskite „D0001“.</span><span class="sxs-lookup"><span data-stu-id="afdf7-110">In the Item number field, type 'D0001'.</span></span>
4. <span data-ttu-id="afdf7-111">Lauke Pristatymas įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-111">In the Delivery field, enter a date.</span></span>
    * <span data-ttu-id="afdf7-112">Pristatymo data nurodo, kada turėtų baigtis gamybos užsakymas, kad būtų pristatyta laiku.</span><span class="sxs-lookup"><span data-stu-id="afdf7-112">The delivery date indicates when the production order should end in order to deliver on time.</span></span> <span data-ttu-id="afdf7-113">Šią datą galima naudoti planavimo procese.</span><span class="sxs-lookup"><span data-stu-id="afdf7-113">This date can be used in the scheduling process.</span></span> <span data-ttu-id="afdf7-114">Pavyzdžiui, užsakymą galite planuoti atgal nuo pristatymo datos.</span><span class="sxs-lookup"><span data-stu-id="afdf7-114">For example, you can schedule the order backward from the delivery date.</span></span>  
5. <span data-ttu-id="afdf7-115">Nustatykite kiekį – 20.</span><span class="sxs-lookup"><span data-stu-id="afdf7-115">Set Quantity to '20'.</span></span>
    * <span data-ttu-id="afdf7-116">Pastaba: KS skaičiaus lauke automatiškai rodomas visų aktyvių dabartinės prekės KS skaičius, tačiau gamybos užsakymo KS galite keisti iš patvirtintų KS versijų sąrašo pasirinkdami aktyvią KS.</span><span class="sxs-lookup"><span data-stu-id="afdf7-116">Note: The BOM number field automatically displays the number of any active BOM for the current item, but you can change the BOM for the production order by selecting an active BOM from the list of approved BOM versions.</span></span>    <span data-ttu-id="afdf7-117">Lauke Maršrutų skaičius automatiškai rodomas visų aktyvių dabartinės prekės maršrutų skaičius, tačiau gamybos užsakymo maršrutą galite keisti iš patvirtintų maršrutų versijų sąrašo pasirinkdami aktyvų maršrutą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-117">The Route number field automatically displays the number of any active Route for the current item, but you can change the Route for the production order by selecting an active Route from the list of approved Route versions.</span></span>  
6. <span data-ttu-id="afdf7-118">Spustelėkite Kurti.</span><span class="sxs-lookup"><span data-stu-id="afdf7-118">Click Create.</span></span>

## <a name="validate-the-production-order"></a><span data-ttu-id="afdf7-119">Tikrinti gamybos užsakymą</span><span class="sxs-lookup"><span data-stu-id="afdf7-119">Validate the production order</span></span>
1. <span data-ttu-id="afdf7-120">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="afdf7-120">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="afdf7-121">Spustelėkite gamybos užsakymo numerio, kurį ką tik sukūrėte, saitą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-121">Click the link for the production order number that you have just created.</span></span> <span data-ttu-id="afdf7-122">Bus atidarytas užsakymo informacijos puslapis.</span><span class="sxs-lookup"><span data-stu-id="afdf7-122">This will open the details page for the order.</span></span>  
2. <span data-ttu-id="afdf7-123">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="afdf7-123">Click Edit.</span></span>
3. <span data-ttu-id="afdf7-124">Lauke Pristatymas įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-124">In the Delivery field, enter a date.</span></span>
    * <span data-ttu-id="afdf7-125">Pavyzdžiui, galite keisti gamybos užsakymo pristatymo datą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-125">For example, you can change the delivery date for the production order.</span></span>  
4. <span data-ttu-id="afdf7-126">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="afdf7-126">Click Save.</span></span>
5. <span data-ttu-id="afdf7-127">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="afdf7-127">Close the page.</span></span>

## <a name="update-the-bom"></a><span data-ttu-id="afdf7-128">Naujinti KS</span><span class="sxs-lookup"><span data-stu-id="afdf7-128">Update the BOM</span></span>
1. <span data-ttu-id="afdf7-129">Veiksmų srityje spustelėkite Gamybos užsakymas.</span><span class="sxs-lookup"><span data-stu-id="afdf7-129">On the Action Pane, click Production order.</span></span>
2. <span data-ttu-id="afdf7-130">Spustelėkite KS.</span><span class="sxs-lookup"><span data-stu-id="afdf7-130">Click BOM.</span></span>
    * <span data-ttu-id="afdf7-131">Atidarykite KS puslapį, kad patikrintumėte KS duomenis, nukopijuotus iš numatytųjų duomenų kuriant gamybos užsakymą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-131">Open the BOM page to validate the BOM data that was copied from the default data when the production order was created.</span></span> <span data-ttu-id="afdf7-132">Atliekant šią procedūrą, reikia atnaujinti KS kiekį.</span><span class="sxs-lookup"><span data-stu-id="afdf7-132">In this procedure, you need to update the quantity for a BOM.</span></span>  
3. <span data-ttu-id="afdf7-133">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="afdf7-133">Click Edit.</span></span>
4. <span data-ttu-id="afdf7-134">Lauke Kiekis įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="afdf7-134">In the Quantity field, enter a number.</span></span>
    * <span data-ttu-id="afdf7-135">Kiekio KS eilutėje keitimas turi įtakos gamybos užsakymo medžiagų suvartojimo išlaidų įvertinimui.</span><span class="sxs-lookup"><span data-stu-id="afdf7-135">Changing the quantity on the BOM line affects the cost estimate of material consumption for the production order.</span></span>  
5. <span data-ttu-id="afdf7-136">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="afdf7-136">Click Save.</span></span>
6. <span data-ttu-id="afdf7-137">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="afdf7-137">Close the page.</span></span>

## <a name="update-the-production-route"></a><span data-ttu-id="afdf7-138">Naujinti gamybos maršrutą</span><span class="sxs-lookup"><span data-stu-id="afdf7-138">Update the production route</span></span>
1. <span data-ttu-id="afdf7-139">Veiksmų srityje spustelėkite Gamybos užsakymas.</span><span class="sxs-lookup"><span data-stu-id="afdf7-139">On the Action Pane, click Production order.</span></span>
2. <span data-ttu-id="afdf7-140">Spustelėkite Maršrutas.</span><span class="sxs-lookup"><span data-stu-id="afdf7-140">Click Route.</span></span>
    * <span data-ttu-id="afdf7-141">Atidarykite puslapį Maršrutas, kad patikrintumėte gamybos maršruto duomenis, nukopijuotus iš numatytųjų duomenų kuriant užsakymą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-141">Open the Route page to validate the data of the production route that was copied from the default data when the order was created.</span></span> <span data-ttu-id="afdf7-142">Atliekant šią procedūrą, reikia atnaujinti vienos iš gamybos maršruto operacijų kiekį.</span><span class="sxs-lookup"><span data-stu-id="afdf7-142">In this procedure, you need to update the quantity for one of the operations in the production route.</span></span>  
3. <span data-ttu-id="afdf7-143">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="afdf7-143">In the list, find and select the desired record.</span></span>
4. <span data-ttu-id="afdf7-144">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="afdf7-144">Click Edit.</span></span>
5. <span data-ttu-id="afdf7-145">Proceso kiekis.</span><span class="sxs-lookup"><span data-stu-id="afdf7-145">In the Process qty.</span></span> <span data-ttu-id="afdf7-146">įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="afdf7-146">field, enter a number.</span></span>
    * <span data-ttu-id="afdf7-147">Vykdymo laiko keitimas turi įtakos gamybos užsakymo apskaičiuotam maršruto suvartojimui ir išlaidoms.</span><span class="sxs-lookup"><span data-stu-id="afdf7-147">Changing the process time affects the estimated route consumption and the cost of the production order.</span></span>  
6. <span data-ttu-id="afdf7-148">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="afdf7-148">Click Save.</span></span>
7. <span data-ttu-id="afdf7-149">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="afdf7-149">Close the page.</span></span>

