--- 
title: "Atributais pagrįstos konfigūruojamų produktų kainodaros nustatymas"
description: "Šioje procedūroje parodoma, kaip nustatyti atributais pagrįstą kainodarą."
author: BibiSp
manager: AnnBe
ms.date: 10/12/2016
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
ms.openlocfilehash: b113fb639b5d7c50e519a0225b1e5d8315b7f3a9
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-attribute-based-pricing-for-configurable-products"></a><span data-ttu-id="4c969-103">Atributais pagrįstos konfigūruojamų produktų kainodaros nustatymas</span><span class="sxs-lookup"><span data-stu-id="4c969-103">Set up attribute-based pricing for configurable products</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="4c969-104">Šioje procedūroje parodoma, kaip nustatyti atributais pagrįstą kainodarą.</span><span class="sxs-lookup"><span data-stu-id="4c969-104">This procedure shows how to set up attribute-based pricing.</span></span> <span data-ttu-id="4c969-105">Būtina sąlyga – reikalingas produkto konfigūracijos modelis, kuriame yra vienas ar daugiau komponentų ir atributų.</span><span class="sxs-lookup"><span data-stu-id="4c969-105">As a prerequisite, you must have a product configuration model that has one or more components and attributes.</span></span> <span data-ttu-id="4c969-106">Šiame pavyzdyje naudojamas aukščiausios klasės garsiakalbio produkto modelis demonstracinių duomenų įmonėje USMF.</span><span class="sxs-lookup"><span data-stu-id="4c969-106">This example uses the High End Speaker product model in the USMF demo data company.</span></span> <span data-ttu-id="4c969-107">Paprastai šią procedūrą atlieka produktų vadovas.</span><span class="sxs-lookup"><span data-stu-id="4c969-107">Typically, a product manager uses this procedure.</span></span>


## <a name="create-a-new-price-model"></a><span data-ttu-id="4c969-108">Naujo kainos modelio kūrimas</span><span class="sxs-lookup"><span data-stu-id="4c969-108">Create a new price model</span></span>
1. <span data-ttu-id="4c969-109">Spustelėkite Produkto varianto modelio aprašą.</span><span class="sxs-lookup"><span data-stu-id="4c969-109">Click Product variant model definition.</span></span>
2. <span data-ttu-id="4c969-110">Spustelėkite Produkto konfigūracijos modeliai.</span><span class="sxs-lookup"><span data-stu-id="4c969-110">Click Product configuration models.</span></span>
3. <span data-ttu-id="4c969-111">Sąraše pasirinkite aukščiausios kokybės garsiakalbio eilutę, bet nespustelėkite pavadinimo nuorodos.</span><span class="sxs-lookup"><span data-stu-id="4c969-111">In the list, select the High End Speaker line, but don’t click the link for the name.</span></span>
4. <span data-ttu-id="4c969-112">Veiksmų srityje spustelėkite Modelis.</span><span class="sxs-lookup"><span data-stu-id="4c969-112">On the Action Pane, click Model.</span></span>
5. <span data-ttu-id="4c969-113">Spustelėkite Kainos modeliai.</span><span class="sxs-lookup"><span data-stu-id="4c969-113">Click Price models.</span></span>
6. <span data-ttu-id="4c969-114">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="4c969-114">Click New.</span></span>
7. <span data-ttu-id="4c969-115">Lauke Kainos modelio pavadinimas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="4c969-115">In the Price model name field, type a value.</span></span>
    * <span data-ttu-id="4c969-116">Naudokite pavadinimą, pagal kurį modelį būtų lengva identifikuoti.</span><span class="sxs-lookup"><span data-stu-id="4c969-116">Use a name that makes the model easy to identify.</span></span>  
8. <span data-ttu-id="4c969-117">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="4c969-117">In the Description field, type a value.</span></span>
9. <span data-ttu-id="4c969-118">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="4c969-118">Click Save.</span></span>

## <a name="add-price-elements"></a><span data-ttu-id="4c969-119">Kainos elementų įtraukimas</span><span class="sxs-lookup"><span data-stu-id="4c969-119">Add price elements</span></span>
1. <span data-ttu-id="4c969-120">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="4c969-120">Click Edit.</span></span>
    * <span data-ttu-id="4c969-121">Kiekviename produkto modelio komponente gali būti bazinės kainos elementas ir bet koks kainos išraiškos taisyklių skaičius.</span><span class="sxs-lookup"><span data-stu-id="4c969-121">Each component in a product model can have a base price element and any number of price expression rules.</span></span> <span data-ttu-id="4c969-122">Taip pat galite įtraukti kainas skirtingomis valiutomis.</span><span class="sxs-lookup"><span data-stu-id="4c969-122">You can also add prices in different currencies.</span></span>  
2. <span data-ttu-id="4c969-123">Lauke Bazinės kainos išraiška įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="4c969-123">In the Base price expression field, type a value.</span></span>
    * <span data-ttu-id="4c969-124">Pavyzdžiui, įveskite 100.</span><span class="sxs-lookup"><span data-stu-id="4c969-124">For example, type 100.</span></span>   <span data-ttu-id="4c969-125">Bazinės kainos išraiška gali būti skaitinė reikšmė arba ją gali sudaryti aritmetinė formulė, naudojanti vieną ar kelis atributus.</span><span class="sxs-lookup"><span data-stu-id="4c969-125">A base price expression can be a numerical value, or it can consist of an arithmetic calculation that involves one or more attributes.</span></span>  
3. <span data-ttu-id="4c969-126">Spustelėkite Pridėti.</span><span class="sxs-lookup"><span data-stu-id="4c969-126">Click Add.</span></span>
4. <span data-ttu-id="4c969-127">Lauke Pavadinimas įveskite Raudonmedžio.</span><span class="sxs-lookup"><span data-stu-id="4c969-127">In the Name field, type ‘Rosewood’.</span></span>
    * <span data-ttu-id="4c969-128">Kainos išraiškos pavadinimas padeda identifikuoti, ką nurodo kainos elementas.</span><span class="sxs-lookup"><span data-stu-id="4c969-128">The price expression name helps identify what the price element represents.</span></span> <span data-ttu-id="4c969-129">Šiame pavyzdyje kuriame kainos elementą, skirtą raudonmedžio garsiakalbio spintelės apdailos parinkčiai.</span><span class="sxs-lookup"><span data-stu-id="4c969-129">In this example, we are creating a price element for the Rosewood speaker cabinet finish option.</span></span>  
5. <span data-ttu-id="4c969-130">Spustelėkite Redaguoti sąlygą.</span><span class="sxs-lookup"><span data-stu-id="4c969-130">Click Edit condition.</span></span>
    * <span data-ttu-id="4c969-131">Kainos sąlyga padeda užtikrinti, kad kainos išraiškos elementas yra įtrauktas į pardavimo kainą tik esant konkrečiam atributų deriniui.</span><span class="sxs-lookup"><span data-stu-id="4c969-131">A price condition helps guarantee that a price expression element is included in the sales price only if a specific combination of attributes is present.</span></span>  
6. <span data-ttu-id="4c969-132">Lauke ConstraintBody įveskite CabinetFinish=="Rosewood".</span><span class="sxs-lookup"><span data-stu-id="4c969-132">In the ConstraintBody field, enter 'CabinetFinish=="Rosewood"'.</span></span>
7. <span data-ttu-id="4c969-133">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="4c969-133">Click OK.</span></span>
8. <span data-ttu-id="4c969-134">Lauke Išraiška įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="4c969-134">In the Expression field, type a value.</span></span>
    * <span data-ttu-id="4c969-135">Pavyzdžiui, įveskite 50.</span><span class="sxs-lookup"><span data-stu-id="4c969-135">For example, type 50.</span></span>  
9. <span data-ttu-id="4c969-136">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="4c969-136">Close the page.</span></span>
10. <span data-ttu-id="4c969-137">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="4c969-137">Close the page.</span></span>

