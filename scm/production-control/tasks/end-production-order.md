--- 
title: "Baigti gamybos užsakymą"
description: "Šioje procedūroje nurodoma, kaip pabaigti gamybos užsakymą."
author: johanhoffmann
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
ms.search.industry: Manufacturing
ms.author: johanho
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 75b91ea330258a5b57e9e58cb32539d57e458f28
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="end-a-production-order"></a><span data-ttu-id="0074a-103">Baigti gamybos užsakymą</span><span class="sxs-lookup"><span data-stu-id="0074a-103">End a production order</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="0074a-104">Šioje procedūroje nurodoma, kaip pabaigti gamybos užsakymą.</span><span class="sxs-lookup"><span data-stu-id="0074a-104">This procedure shows how to end a production order.</span></span> <span data-ttu-id="0074a-105">Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.</span><span class="sxs-lookup"><span data-stu-id="0074a-105">The demo data company used to create this procedure is USMF.</span></span> <span data-ttu-id="0074a-106">Tai yra paskutinė procedūra iš septynių, kurioje paaiškinamas gamybos užsakymo ciklas.</span><span class="sxs-lookup"><span data-stu-id="0074a-106">This is the final procedure out of seven which explains the production order lifecycle.</span></span>


## <a name="end-a-production-order"></a><span data-ttu-id="0074a-107">Baigti gamybos užsakymą</span><span class="sxs-lookup"><span data-stu-id="0074a-107">End a production order</span></span>
1. <span data-ttu-id="0074a-108">Pasirinkite Gamybos kontrolė > Gamybos užsakymai > Visi gamybos užsakymai.</span><span class="sxs-lookup"><span data-stu-id="0074a-108">Go to Production control > Production orders > All production orders.</span></span>
    * <span data-ttu-id="0074a-109">Pasirinkite gamybos užsakymą, kurio būsena yra Paskelbtas baigtu.</span><span class="sxs-lookup"><span data-stu-id="0074a-109">Select a production order that has the status Reported as finished.</span></span>  
2. <span data-ttu-id="0074a-110">Veiksmų srityje spustelėkite Gamybos užsakymas.</span><span class="sxs-lookup"><span data-stu-id="0074a-110">On the Action Pane, click Production order.</span></span>
3. <span data-ttu-id="0074a-111">Spustelėkite Baigti.</span><span class="sxs-lookup"><span data-stu-id="0074a-111">Click End.</span></span>
    * <span data-ttu-id="0074a-112">Šiame puslapyje galite patvirtinti, kad norite baigti gamybos užsakymą.</span><span class="sxs-lookup"><span data-stu-id="0074a-112">On this page, you can confirm that you want to end the production order.</span></span>  
4. <span data-ttu-id="0074a-113">Spustelėkite skirtuką Bendra.</span><span class="sxs-lookup"><span data-stu-id="0074a-113">Click the General tab.</span></span>
5. <span data-ttu-id="0074a-114">Lauke Data įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="0074a-114">In the Date field, enter a date.</span></span>
6. <span data-ttu-id="0074a-115">Lauke Nurašymo metodas pasirinkite „Paskirstymas“.</span><span class="sxs-lookup"><span data-stu-id="0074a-115">In the Scrap method field, select 'Allocation'.</span></span>
    * <span data-ttu-id="0074a-116">Pasirinkus metodą Paskirstymas, išlaidos už nurašytas medžiagas pridedamos prie pagamintų prekių.</span><span class="sxs-lookup"><span data-stu-id="0074a-116">When you select the Allocation method, costs from the scrapped materials are added to the finished goods.</span></span>  
7. <span data-ttu-id="0074a-117">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="0074a-117">Click OK.</span></span>

## <a name="validate-calculation-results"></a><span data-ttu-id="0074a-118">Skaičiavimo rezultatų tikrinimas</span><span class="sxs-lookup"><span data-stu-id="0074a-118">Validate calculation results</span></span>
1. <span data-ttu-id="0074a-119">Veiksmų srityje spustelėkite Valdyti išlaidas.</span><span class="sxs-lookup"><span data-stu-id="0074a-119">On the Action Pane, click Manage costs.</span></span>
2. <span data-ttu-id="0074a-120">Spustelėkite Peržiūrėti savikainos palyginimą.</span><span class="sxs-lookup"><span data-stu-id="0074a-120">Click View cost comparison.</span></span>
    * <span data-ttu-id="0074a-121">Pabaigę gamybos užsakymą galite palyginti įvertintą savikainą su realizuota savikaina ir peržiūrėti gamybos nuokrypius.</span><span class="sxs-lookup"><span data-stu-id="0074a-121">After you have ended the production order, you can compare the estimated cost price against the realized cost price to get an overview of the production variances.</span></span>  

