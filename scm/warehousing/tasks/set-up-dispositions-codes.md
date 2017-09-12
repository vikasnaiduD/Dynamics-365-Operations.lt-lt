--- 
title: Nustatyti perdavimo kodus
description: "Šios procedūros tikslas yra nustatyti perdavimo kodą, kuris gali būti naudojamas mobiliajame įrenginyje, vykdant grąžinimo užsakymo gavimo procesą."
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
ms.search.industry: Distribution
ms.author: bis
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: c004543188656dfd53d7539717cd6e93d0b9f47a
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-dispositions-codes"></a><span data-ttu-id="ac129-103">Nustatyti perdavimo kodus</span><span class="sxs-lookup"><span data-stu-id="ac129-103">Set up dispositions codes</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="ac129-104">Šios procedūros tikslas yra nustatyti perdavimo kodą, kuris gali būti naudojamas mobiliajame įrenginyje, vykdant grąžinimo užsakymo gavimo procesą.</span><span class="sxs-lookup"><span data-stu-id="ac129-104">This procedure focuses on the setup of a disposition code that can be used on a mobile device for the return order receiving process.</span></span> <span data-ttu-id="ac129-105">Perdavimo kodai yra rinkinys taisyklių, kurios gali būti taikomos gaunant prekes.</span><span class="sxs-lookup"><span data-stu-id="ac129-105">Disposition codes are a collection of rules that can be used when items are received.</span></span> <span data-ttu-id="ac129-106">Pvz., kai darbo vartotojas mobiliuoju įrenginiu priima pažeistas prekes, vartotojas turi nuskaityti pažeistų prekių perdavimo kodą.</span><span class="sxs-lookup"><span data-stu-id="ac129-106">For example, when a work user uses a mobile device to receive items that were damaged, the user must scan a disposition code for damaged items.</span></span> <span data-ttu-id="ac129-107">Nuskaičius perdavimo kodą galima nustatyti gautų prekių atsargų būseną, darbo šabloną ir vietos nurodymą.</span><span class="sxs-lookup"><span data-stu-id="ac129-107">The inventory status of the goods received, the work template, and the location directive can be determined from the scanned disposition code.</span></span> <span data-ttu-id="ac129-108">Perdavimo kodo neprivaloma naudoti pirkimo užsakymo gavimo procese ir gamybos užsakymo paskelbimo baigtu procese.</span><span class="sxs-lookup"><span data-stu-id="ac129-108">For the purchase order receiving process and the production order report as finished process, the use of a disposition code is optional.</span></span> <span data-ttu-id="ac129-109">Vykdant pardavimo užsakymo grąžinimo gavimo procesą, jei prekės registruotos mobiliuoju įrenginiu, naudoti perdavimo kodą yra privaloma.</span><span class="sxs-lookup"><span data-stu-id="ac129-109">For the sales order return receiving process, if the items are registered using a mobile device, the use of disposition code is mandatory.</span></span>  <span data-ttu-id="ac129-110">Šis vadovas buvo sukurtas naudojant demonstracinių duomenų įmonę USMF.</span><span class="sxs-lookup"><span data-stu-id="ac129-110">This guide was created using the demo data company USMF.</span></span> <span data-ttu-id="ac129-111">Ši procedūra skirta sandėlio vadovui.</span><span class="sxs-lookup"><span data-stu-id="ac129-111">This procedure is intended for the warehouse manager.</span></span> 

1. <span data-ttu-id="ac129-112">Pasirinkite > Sandėlio valdymas > Nustatymas > Mobilusis įrenginys > Perdavimo kodai.</span><span class="sxs-lookup"><span data-stu-id="ac129-112">Go to Warehouse management > Setup > Mobile device > Disposition codes.</span></span>
2. <span data-ttu-id="ac129-113">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="ac129-113">Click New.</span></span>
    * <span data-ttu-id="ac129-114">Sukurkite naują perdavimo kodą, naudojamą klientų grąžinamoms prekėms.</span><span class="sxs-lookup"><span data-stu-id="ac129-114">Create a new disposition code to use for customer returns.</span></span>  
3. <span data-ttu-id="ac129-115">Lauke „Perdavimo kodas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="ac129-115">In the Disposition code field, type a value.</span></span>
4. <span data-ttu-id="ac129-116">Lauke „Atsargų būsena“ pasirinkite atsargų būseną, kai taikomas atsargų blokavimas.</span><span class="sxs-lookup"><span data-stu-id="ac129-116">In the Inventory status field, select an inventory status where there is inventory blocking.</span></span>
    * <span data-ttu-id="ac129-117">Jei naudojate USMF, pasirinkite „Blokavimas“.</span><span class="sxs-lookup"><span data-stu-id="ac129-117">If you're using USMF, select 'Blocking'.</span></span> <span data-ttu-id="ac129-118">Į perdavimo kodą galima įtraukti atsargų būseną, kad būtų perrašyta užsakymo eilutėse esanti numatytoji būsena.</span><span class="sxs-lookup"><span data-stu-id="ac129-118">You can add an inventory status to the disposition code to override the default status that’s on the order lines.</span></span>  
5. <span data-ttu-id="ac129-119">Lauke „Darbo šablonas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="ac129-119">In the Work template field, type a value.</span></span>
    * <span data-ttu-id="ac129-120">Pasirinktinai: pasirinkite darbo šablono kodą, susijusį su grąžinimo užsakymu.</span><span class="sxs-lookup"><span data-stu-id="ac129-120">Optional: Select a work template code that is associated with a return order.</span></span> <span data-ttu-id="ac129-121">Jei nenurodyta jokia reikšmė, darbo šablonas bus išspręstas naudojant standartines jūsų sistemoje sukonfigūruotas taisykles.</span><span class="sxs-lookup"><span data-stu-id="ac129-121">If no value is provided, the work template will be resolved using the standard rules configured in your system.</span></span> <span data-ttu-id="ac129-122">Darbo šablono pasirinkimas apribos skaičių procesų, kuriuose galima naudoti šį perdavimo kodą.</span><span class="sxs-lookup"><span data-stu-id="ac129-122">Selecting a work template will limit the processes this disposition code can be used with.</span></span> <span data-ttu-id="ac129-123">Pvz., jei perdavimo kodas turi darbo šabloną su pirkimo užsakymo tipo darbo užsakymu, juo nebus galima registruoti prekių, kurias grąžina klientai.</span><span class="sxs-lookup"><span data-stu-id="ac129-123">For example, if a disposition code has a work template with a work order of type purchase order, it can’t be used to register items that are returned by customers.</span></span>  
6. <span data-ttu-id="ac129-124">Lauke „Grąžinti perdavimo kodą“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="ac129-124">In the Return disposition code field, type a value.</span></span>
    * <span data-ttu-id="ac129-125">Grąžinimo perdavimo kodas nulemia registruotų prekių grąžinimo užsakymo proceso likutį.</span><span class="sxs-lookup"><span data-stu-id="ac129-125">The return disposition code determines the remainder of the return order process for the items registered.</span></span> <span data-ttu-id="ac129-126">Šiame pavyzdyje klientas turėtų gauti kredito pažymą.</span><span class="sxs-lookup"><span data-stu-id="ac129-126">In this example, the customer should receive a credit note.</span></span> <span data-ttu-id="ac129-127">Įtraukite grąžinimo perdavimo kodą, kuriame yra veiksmas „Kreditas“.</span><span class="sxs-lookup"><span data-stu-id="ac129-127">Add a returns disposition code that contains an action Credit.</span></span>  

