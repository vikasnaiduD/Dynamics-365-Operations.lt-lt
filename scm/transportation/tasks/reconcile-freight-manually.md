--- 
title: "Transportavimo derinimas neautomatiniu būdu"
description: "Šioje procedūroje parodoma, kaip transportavimą derinti neautomatiniu būdu."
author: BibiSp
manager: AnnBe
ms.date: 10/13/2016
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
ms.openlocfilehash: 15148725664d839694ede8419213d881c7be83dd
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="reconcile-freight-manually"></a><span data-ttu-id="31afd-103">Transportavimo derinimas neautomatiniu būdu</span><span class="sxs-lookup"><span data-stu-id="31afd-103">Reconcile freight manually</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="31afd-104">Šioje procedūroje parodoma, kaip transportavimą derinti neautomatiniu būdu.</span><span class="sxs-lookup"><span data-stu-id="31afd-104">This procedure shows how to reconcile freight manually.</span></span> <span data-ttu-id="31afd-105">Paprastai tą daro transportavimo koordinatorius.</span><span class="sxs-lookup"><span data-stu-id="31afd-105">This is typically done by a transportation coordinator.</span></span> <span data-ttu-id="31afd-106">Šią procedūrą galite naudoti USMF demonstracinių duomenų įmonėje.</span><span class="sxs-lookup"><span data-stu-id="31afd-106">You can use this procedure in the USMF demo data company.</span></span>


## <a name="select-a-load-to-reconcile"></a><span data-ttu-id="31afd-107">Derintinos apkrovos pasirinkimas</span><span class="sxs-lookup"><span data-stu-id="31afd-107">Select a load to reconcile</span></span>
1. <span data-ttu-id="31afd-108">Pasirinkite Transportavimo valdymas > Planavimas > Krovinio planavimo darbo sritis.</span><span class="sxs-lookup"><span data-stu-id="31afd-108">Go to Transportation management > Planning > Load planning workbench.</span></span>
2. <span data-ttu-id="31afd-109">Išvalykite žymės langelį Slėpti išsiųstus ir gautus.</span><span class="sxs-lookup"><span data-stu-id="31afd-109">Clear the Hide shipped and received check box.</span></span> 
3. <span data-ttu-id="31afd-110">Sąraše pasirinkite krovinį, kurio krovinio ID yra 00006.</span><span class="sxs-lookup"><span data-stu-id="31afd-110">In the list, select the load that has load ID 00006.</span></span>

## <a name="create-a-carrier-invoice"></a><span data-ttu-id="31afd-111">Vežėjo SF kūrimas</span><span class="sxs-lookup"><span data-stu-id="31afd-111">Create a carrier invoice</span></span>
    * <span data-ttu-id="31afd-112">Jei transportavimą derinate neautomatiniu būdu ir negaunate vežėjo SF automatiškai, galite kurti SF pagal transportavimo sąskaitą.</span><span class="sxs-lookup"><span data-stu-id="31afd-112">If you reconcile freight manually and don’t receive carrier invoices automatically, you can create an invoice based on the freight bill.</span></span>  
1. <span data-ttu-id="31afd-113">Spustelėkite Susijusi informacija.</span><span class="sxs-lookup"><span data-stu-id="31afd-113">Click Related information.</span></span>
2. <span data-ttu-id="31afd-114">Spustelėkite Transportavimo sąskaitos informacija</span><span class="sxs-lookup"><span data-stu-id="31afd-114">Click Freight bill details.</span></span>
3. <span data-ttu-id="31afd-115">Spustelėkite Generuoti krovinio atsiskaitymo SF.</span><span class="sxs-lookup"><span data-stu-id="31afd-115">Click Generate freight bill invoice.</span></span>
4. <span data-ttu-id="31afd-116">Lauke Sąskaita faktūra surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="31afd-116">In the Invoice field, type a value.</span></span>
5. <span data-ttu-id="31afd-117">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="31afd-117">Click OK.</span></span>

## <a name="reconcile-the-invoice"></a><span data-ttu-id="31afd-118">SF derinimas</span><span class="sxs-lookup"><span data-stu-id="31afd-118">Reconcile the invoice</span></span>
    * <span data-ttu-id="31afd-119">Vežėjo SF ir transportavimo sąskaitos derinimas atliekamas kiekvienoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="31afd-119">When you reconcile a carrier invoice and a freight bill, this is done line by line.</span></span>  
1. <span data-ttu-id="31afd-120">Spustelėkite Gretinti transportavimo sąskaitas ir SF.</span><span class="sxs-lookup"><span data-stu-id="31afd-120">Click Match freight bills and invoices.</span></span>
2. <span data-ttu-id="31afd-121">Išplėskite skyrių SF informacija.</span><span class="sxs-lookup"><span data-stu-id="31afd-121">Expand the Invoice details section.</span></span>
3. <span data-ttu-id="31afd-122">Išplėskite skyrių Nesugretinta transportavimo sąskaitos informacija.</span><span class="sxs-lookup"><span data-stu-id="31afd-122">Expand the Unmatched freight bill details section.</span></span>
4. <span data-ttu-id="31afd-123">Sąraše pažymėkite pasirinktą eilutę.</span><span class="sxs-lookup"><span data-stu-id="31afd-123">In the list, mark the selected row.</span></span>
5. <span data-ttu-id="31afd-124">Spustelėkite Gretinti.</span><span class="sxs-lookup"><span data-stu-id="31afd-124">Click Match.</span></span>
6. <span data-ttu-id="31afd-125">Išplėskite skyrių Sugretinta transportavimo sąskaitos informacija.</span><span class="sxs-lookup"><span data-stu-id="31afd-125">Expand the Matched freight bill details section.</span></span>

## <a name="submit-the-invoice-for-approval"></a><span data-ttu-id="31afd-126">Pateikti SF patvirtinti</span><span class="sxs-lookup"><span data-stu-id="31afd-126">Submit the invoice for approval</span></span>
1. <span data-ttu-id="31afd-127">Spustelėkite Pateikti patvirtinti.</span><span class="sxs-lookup"><span data-stu-id="31afd-127">Click Submit for approval.</span></span>
2. <span data-ttu-id="31afd-128">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="31afd-128">Close the page.</span></span>
3. <span data-ttu-id="31afd-129">Išvalykite žymės langelį Slėpti patvirtintus.</span><span class="sxs-lookup"><span data-stu-id="31afd-129">Clear the Hide approved check box.</span></span> 
4. <span data-ttu-id="31afd-130">Spustelėkite Tiekėjo SF žurnalai.</span><span class="sxs-lookup"><span data-stu-id="31afd-130">Click Vendor invoice journals.</span></span>
5. <span data-ttu-id="31afd-131">Spustelėkite, kad būtumėte nukreipti pagal saitą lauke Nuorodų žurnalo numeris.</span><span class="sxs-lookup"><span data-stu-id="31afd-131">Click to follow the link in the Reference journal number field.</span></span>
6. <span data-ttu-id="31afd-132">Spustelėkite Eilutės.</span><span class="sxs-lookup"><span data-stu-id="31afd-132">Click Lines.</span></span>

