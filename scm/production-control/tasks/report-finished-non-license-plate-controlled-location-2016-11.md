--- 
title: "Skelbimas baigtais į ne pagal numerio lentelę kontroliuojamą vietą "
description: "Šiame užduoties vadove parodytas skelbimo baigtu vietoje, kuri nėra kontroliuojama pagal numerio lentelę, pavyzdys."
author: ChristianRytt
manager: AnnBe
ms.date: 06/23/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: a14efeda12cdb677bf9e82f251d1cb91e36337fb
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="report-as-finished-to-a-plate-controlled-location"></a><span data-ttu-id="31cfb-103">Skelbimas baigtais į ne pagal numerio lentelę kontroliuojamą vietą </span><span class="sxs-lookup"><span data-stu-id="31cfb-103">Report as finished to a plate-controlled location</span></span> 

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="31cfb-104">Šiame užduoties vadove parodytas skelbimo baigtu vietoje, kuri nėra kontroliuojama pagal numerio lentelę, pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="31cfb-104">This task guide shows an example of reporting as finished to a location that isn't license plate–controlled.</span></span> <span data-ttu-id="31cfb-105">Norint atlikti šią užduotį, būtina tinkama darbo strategija.</span><span class="sxs-lookup"><span data-stu-id="31cfb-105">An applicable work policy is the prerequisite for this task.</span></span> <span data-ttu-id="31cfb-106">Kaip nustatyti darbo strategiją, parodyta ankstesniame užduoties vadove.</span><span class="sxs-lookup"><span data-stu-id="31cfb-106">A previous task guide showed the setup of the work policy.</span></span> <span data-ttu-id="31cfb-107">Norint atlikti šį užduoties vediklį, reikia „Dynamics AX‟ programos 7.0.1 arba naujesnės versijos.</span><span class="sxs-lookup"><span data-stu-id="31cfb-107">This task guide requires Dynamics AX application 7.0.1 or later.</span></span>




## <a name="set-up-an-output-location"></a><span data-ttu-id="31cfb-108">Išeigos vietos nustatymas</span><span class="sxs-lookup"><span data-stu-id="31cfb-108">Set up an output location</span></span>
1. <span data-ttu-id="31cfb-109">Pasirinkite Organizacijos administravimas > Ištekliai > Išteklių grupės.</span><span class="sxs-lookup"><span data-stu-id="31cfb-109">Go to Organization administration > Resources > Resource groups.</span></span>
2. <span data-ttu-id="31cfb-110">Sąraše pasirinkite išteklių grupę 5102.</span><span class="sxs-lookup"><span data-stu-id="31cfb-110">In the list, select resource group '5102'.</span></span>
3. <span data-ttu-id="31cfb-111">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="31cfb-111">Click Edit.</span></span>
4. <span data-ttu-id="31cfb-112">Lauke Išeigos sandėlis įveskite „51‟.</span><span class="sxs-lookup"><span data-stu-id="31cfb-112">In the Output warehouse field, enter '51'.</span></span>
5. <span data-ttu-id="31cfb-113">Lauke Išeigos vieta įveskite „001‟.</span><span class="sxs-lookup"><span data-stu-id="31cfb-113">In the Output location field, enter '001'.</span></span>
    * <span data-ttu-id="31cfb-114">001 vieta nėra kontroliuojama pagal numerio lentelę.</span><span class="sxs-lookup"><span data-stu-id="31cfb-114">Location 001 isn't a license plate–controlled location.</span></span> <span data-ttu-id="31cfb-115">Ne pagal numerio lentelę kontroliuojamą išeigos vietą galite nustatyti tik jei yra tinkama vietos darbo strategija.</span><span class="sxs-lookup"><span data-stu-id="31cfb-115">You can set up a non–license plate output location only if an applicable work policy exists for the location.</span></span>  

## <a name="create-a-production-order-and-report-it-as-finished"></a><span data-ttu-id="31cfb-116">Gamybos užsakymo sukūrimas ir jo skelbimas baigtu</span><span class="sxs-lookup"><span data-stu-id="31cfb-116">Create a production order and report it as finished</span></span>
1. <span data-ttu-id="31cfb-117">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="31cfb-117">Close the page.</span></span>
2. <span data-ttu-id="31cfb-118">Pasirinkite Gamybos kontrolė > Gamybos užsakymai > Visi gamybos užsakymai.</span><span class="sxs-lookup"><span data-stu-id="31cfb-118">Go to Production control > Production orders > All production orders.</span></span>
3. <span data-ttu-id="31cfb-119">Spustelėkite Naujas gamybos užsakymas.</span><span class="sxs-lookup"><span data-stu-id="31cfb-119">Click New production order.</span></span>
4. <span data-ttu-id="31cfb-120">Lauke Prekės numeris įveskite „L0101‟.</span><span class="sxs-lookup"><span data-stu-id="31cfb-120">In the Item number field, enter 'L0101'.</span></span>
5. <span data-ttu-id="31cfb-121">Spustelėkite Kurti.</span><span class="sxs-lookup"><span data-stu-id="31cfb-121">Click Create.</span></span>
6. <span data-ttu-id="31cfb-122">Srityje Veiksmas spustelėkite Gamybos užsakymas.</span><span class="sxs-lookup"><span data-stu-id="31cfb-122">On the Action Pane, click Production order.</span></span>
7. <span data-ttu-id="31cfb-123">Spustelėkite Įvertinti.</span><span class="sxs-lookup"><span data-stu-id="31cfb-123">Click Estimate.</span></span>
8. <span data-ttu-id="31cfb-124">Spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="31cfb-124">Click OK.</span></span>
9. <span data-ttu-id="31cfb-125">Spustelėkite Pradėti.</span><span class="sxs-lookup"><span data-stu-id="31cfb-125">Click Start.</span></span>
10. <span data-ttu-id="31cfb-126">Spustelėkite skirtuką Bendra.</span><span class="sxs-lookup"><span data-stu-id="31cfb-126">Click the General tab.</span></span>
11. <span data-ttu-id="31cfb-127">Lauke Automatinis KS suvartojimas pasirinkite Niekada.</span><span class="sxs-lookup"><span data-stu-id="31cfb-127">In the Automatic BOM consumption field, select 'Never'.</span></span>
12. <span data-ttu-id="31cfb-128">Spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="31cfb-128">Click OK.</span></span>
13. <span data-ttu-id="31cfb-129">Spustelėkite Skelbti baigtu.</span><span class="sxs-lookup"><span data-stu-id="31cfb-129">Click Report as finished.</span></span>
14. <span data-ttu-id="31cfb-130">Spustelėkite skirtuką Bendra.</span><span class="sxs-lookup"><span data-stu-id="31cfb-130">Click the General tab.</span></span>
15. <span data-ttu-id="31cfb-131">Lauke Leisti klaidą pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="31cfb-131">Select Yes in the Accept error field.</span></span>
16. <span data-ttu-id="31cfb-132">Spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="31cfb-132">Click OK.</span></span>
17. <span data-ttu-id="31cfb-133">Veiksmų srityje spustelėkite Sandėlis.</span><span class="sxs-lookup"><span data-stu-id="31cfb-133">On the Action Pane, click Warehouse.</span></span>
18. <span data-ttu-id="31cfb-134">Spustelėkite Darbo informacija.</span><span class="sxs-lookup"><span data-stu-id="31cfb-134">Click Work details.</span></span>
    * <span data-ttu-id="31cfb-135">Kai gamybos užsakymas buvo paskelbtas baigtu, nebuvo sugeneruota jokio padėjimo darbo.</span><span class="sxs-lookup"><span data-stu-id="31cfb-135">When the production order was reported as finished, no work was generated for put-away.</span></span> <span data-ttu-id="31cfb-136">Taip nutinka, nes yra apibrėžta darbo strategija, pagal kurią negalima generuoti darbo, kai produktas L0101 paskebiamas baigtu 001 vietoje.</span><span class="sxs-lookup"><span data-stu-id="31cfb-136">This occurs because a work policy is defined that prevents work from being generated when product L0101 is reported as finished to location 001.</span></span>  

