--- 
title: "Kurti konfigūracijos taisykles"
description: "Šia procedūra sukuriamos konfigūracijos taisyklės, pagal kurias, naudojant konfigūravimą pagal dimensijas, būtų galima taikyti arba neleisti taikyti tam tikrų KS eilučių kombinacijų."
author: BibiSp
manager: AnnBe
ms.date: 11/11/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Operations
ms.search.region: Global
ms.author: bis
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: c901ebea4fd7423db61ef2c33689e606e33e2434
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="create-configuration-rules"></a><span data-ttu-id="57e30-103">Kurti konfigūracijos taisykles</span><span class="sxs-lookup"><span data-stu-id="57e30-103">Create configuration rules</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="57e30-104">Šia procedūra sukuriamos konfigūracijos taisyklės, pagal kurias, naudojant konfigūravimą pagal dimensijas, būtų galima taikyti arba neleisti taikyti tam tikrų KS eilučių kombinacijų.</span><span class="sxs-lookup"><span data-stu-id="57e30-104">This procedure creates configuration rules that can be used for dimension-based configuration to enforce or prevent certain combinations of BOM lines.</span></span> <span data-ttu-id="57e30-105">Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.</span><span class="sxs-lookup"><span data-stu-id="57e30-105">The demo data company used to create this procedure is USMF.</span></span> <span data-ttu-id="57e30-106">Tai yra septintoji iš aštuonių procedūrų, kuriomis paaiškinama, kaip kurti konfigūravimo pagal dimensijas kombinacijas.</span><span class="sxs-lookup"><span data-stu-id="57e30-106">This is the seventh procedure out of eight that explains how to build combinations for dimension-based configuration.</span></span>

1. <span data-ttu-id="57e30-107">Pasirinkite Produkto informacijos valdymas > Komplektavimo specifikacijos ir formulės > Komplektavimo specifikacijos.</span><span class="sxs-lookup"><span data-stu-id="57e30-107">Go to Product information management > Bills of materials and formulas > Bills of materials.</span></span>
2. <span data-ttu-id="57e30-108">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="57e30-108">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="57e30-109">Raskite ir pasirinkite konfigūravimo pagal dimensijas KS.</span><span class="sxs-lookup"><span data-stu-id="57e30-109">Find and select the BOM for the dimension-based configuration.</span></span>  
3. <span data-ttu-id="57e30-110">Veiksmų srityje spustelėkite Parinktys.</span><span class="sxs-lookup"><span data-stu-id="57e30-110">On the Action Pane, click Options.</span></span>
4. <span data-ttu-id="57e30-111">Spustelėkite Keisti rodinį.</span><span class="sxs-lookup"><span data-stu-id="57e30-111">Click Change view.</span></span>
5. <span data-ttu-id="57e30-112">Spustelėkite antraštės rodinį.</span><span class="sxs-lookup"><span data-stu-id="57e30-112">Click Header view.</span></span>
    * <span data-ttu-id="57e30-113">Atidarykite antraštės rodinį, kad pasiektumėte konfigūracijos maršrutą „FastTab“.</span><span class="sxs-lookup"><span data-stu-id="57e30-113">Open the header view to access the Configuration route FastTab.</span></span>  
6. <span data-ttu-id="57e30-114">Išplėskite arba sutraukite sekciją Konfigūracijos maršrutas.</span><span class="sxs-lookup"><span data-stu-id="57e30-114">Expand or collapse the Configuration route section.</span></span>
    * <span data-ttu-id="57e30-115">Konfigūracijos maršrutas „FastTab“ turi būti išplėstiniame režime.</span><span class="sxs-lookup"><span data-stu-id="57e30-115">The Configuration route FastTab must be in the expanded mode.</span></span>  
7. <span data-ttu-id="57e30-116">Spustelėkite „Konfigūracijos taisyklės“.</span><span class="sxs-lookup"><span data-stu-id="57e30-116">Click Configuration rules.</span></span>
8. <span data-ttu-id="57e30-117">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="57e30-117">Click New.</span></span>
9. <span data-ttu-id="57e30-118">Sąraše pažymėkite pasirinktą eilutę.</span><span class="sxs-lookup"><span data-stu-id="57e30-118">In the list, mark the selected row.</span></span>
10. <span data-ttu-id="57e30-119">Lauke Prekės numeris spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="57e30-119">In the Item number field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="57e30-120">Rodomos prekės esamoje konfigūracijos grupėje.</span><span class="sxs-lookup"><span data-stu-id="57e30-120">The items in the current configuration group are displayed.</span></span> <span data-ttu-id="57e30-121">Pasirinkite tą, kuri atitinka taisyklės sąlygą.</span><span class="sxs-lookup"><span data-stu-id="57e30-121">Select the one that represents the condition in the rule.</span></span>  
11. <span data-ttu-id="57e30-122">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="57e30-122">In the list, click the link in the selected row.</span></span>
12. <span data-ttu-id="57e30-123">Lauke Metodas pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="57e30-123">In the Method field, select an option.</span></span>
    * <span data-ttu-id="57e30-124">Įmanoma žymėti arba atžymėti prekę iš kitos konfigūracijos grupės.</span><span class="sxs-lookup"><span data-stu-id="57e30-124">It is possible to enforce either a selection or a deselection of an item from another configuration group.</span></span>  
13. <span data-ttu-id="57e30-125">Lauke „Išvestinė grupė“ spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="57e30-125">In the Derived group field, click the drop-down button to open the lookup.</span></span>
14. <span data-ttu-id="57e30-126">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="57e30-126">In the list, find and select the desired record.</span></span>
15. <span data-ttu-id="57e30-127">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="57e30-127">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="57e30-128">Pasirinkite norimą konfigūracijos grupę.</span><span class="sxs-lookup"><span data-stu-id="57e30-128">Select the desired configuration group.</span></span>  
16. <span data-ttu-id="57e30-129">Lauke „Išvestinės prekės numeris“ spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="57e30-129">In the Derived item number field, click the drop-down button to open the lookup.</span></span>
17. <span data-ttu-id="57e30-130">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="57e30-130">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="57e30-131">Pasirinkite prekės numerį, kuris bus pažymėtas arba atžymėtas, atsižvelgiant į pasirinktą metodą.</span><span class="sxs-lookup"><span data-stu-id="57e30-131">Select the item number that will be either selected or deselected depending on the chosen method.</span></span>  
18. <span data-ttu-id="57e30-132">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="57e30-132">Close the page.</span></span>

