--- 
title: Kurti pirkimo strategijas
description: "Šioje procedūroje parodoma, kaip kurti pirkimo strategijas ir suderinti jas su pirkimo verslo procesais."
author: mkirknel
manager: AnnBe
ms.date: 08/23/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: c2b3a66443394f5bfbe51b6685513281025d68fd
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="create-purchasing-policies"></a><span data-ttu-id="c714a-103">Kurti pirkimo strategijas</span><span class="sxs-lookup"><span data-stu-id="c714a-103">Create purchasing policies</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="c714a-104">Šioje procedūroje parodoma, kaip kurti pirkimo strategijas ir suderinti jas su pirkimo verslo procesais.</span><span class="sxs-lookup"><span data-stu-id="c714a-104">This procedure shows you how to create purchasing policies to align with your business processes for purchasing.</span></span> <span data-ttu-id="c714a-105">Prieš kurdami pirkimo strategijas turite nustatyti pirkimo strategijos parametrus.</span><span class="sxs-lookup"><span data-stu-id="c714a-105">Before you can create purchasing policies, you must set up the purchasing policy parameters.</span></span> <span data-ttu-id="c714a-106">Galima kurti, modifikuoti ir nurašyti pirkimo strategiją, bet pirkimo strategijos negalima naikinti.</span><span class="sxs-lookup"><span data-stu-id="c714a-106">It’s possible to create, modify, and retire a purchasing policy, but you can’t delete a purchasing policy.</span></span> <span data-ttu-id="c714a-107">Šią procedūrą paprastai atlieka pirkimo vadovas.</span><span class="sxs-lookup"><span data-stu-id="c714a-107">This procedure would typically be carried out by a purchasing manager.</span></span> <span data-ttu-id="c714a-108">Šią procedūrą galite atlikti demonstracinių duomenų įmonėje USMF arba su savo duomenimis.</span><span class="sxs-lookup"><span data-stu-id="c714a-108">You can use this procedure in demo data company USMF or on your own data.</span></span>


## <a name="set-up-policy-parameters"></a><span data-ttu-id="c714a-109">Strategijos parametrų nustatymas</span><span class="sxs-lookup"><span data-stu-id="c714a-109">Set up policy parameters</span></span>
1. <span data-ttu-id="c714a-110">Pasirinkite Pirkimo strategijos.</span><span class="sxs-lookup"><span data-stu-id="c714a-110">Go to Purchasing policies.</span></span>
2. <span data-ttu-id="c714a-111">Spustelėkite Parametrai.</span><span class="sxs-lookup"><span data-stu-id="c714a-111">Click Parameters.</span></span>
    * <span data-ttu-id="c714a-112">Strategijos pirmumo taisyklės taikomos skirtingiems jūsų organizacijos lygiams.</span><span class="sxs-lookup"><span data-stu-id="c714a-112">Policy precedence rules apply to different levels in your organization.</span></span> <span data-ttu-id="c714a-113">Rodomi organizacijos vienetai priklauso nuo jūsų organizacijos hierarchijos ir nuo to, kuriems hierarchijos lygiams priskirta paskirtis Įsigijimo vidinė kontrolė.</span><span class="sxs-lookup"><span data-stu-id="c714a-113">The organizational units that are shown depend on your organizational hierarchy, and on which levels in the hierarchy have been assigned the purpose of Procurement internal control.</span></span> <span data-ttu-id="c714a-114">Pvz., organizacijoje gali būti juridiniai subjektai, išlaidų centrai, regionai ir padaliniai, bet galbūt tik kai kuriems iš jų priskirta hierarchijos paskirtis Įsigijimo vidinė kontrolė.</span><span class="sxs-lookup"><span data-stu-id="c714a-114">For example, your organization might have legal entities, cost centers, regions, and departments, but it may be that only some of these have a hierarchy purpose of Procurement internal control.</span></span> <span data-ttu-id="c714a-115">Pagal numatytuosius parametrus galimas organizacijos tipas Įmonė.</span><span class="sxs-lookup"><span data-stu-id="c714a-115">As a default, the organization of type Company is available.</span></span>  
3. <span data-ttu-id="c714a-116">Spustelėkite skirtuką Strategijos taisyklės tipo parametrai.</span><span class="sxs-lookup"><span data-stu-id="c714a-116">Click the Policy rule type parameters tab.</span></span>
4. <span data-ttu-id="c714a-117">Medyje pasirinkite Pirkimo strategija\Pirkimo paraiškos kontrolės taisyklė.</span><span class="sxs-lookup"><span data-stu-id="c714a-117">In the tree, select 'Purchasing policy\Purchase requisition control rule'.</span></span>
    * <span data-ttu-id="c714a-118">Strategijos taikymo pirmumo tvarką galite nurodyti strategijos lygiu.</span><span class="sxs-lookup"><span data-stu-id="c714a-118">You define the order of precedence for policy resolution at the policy level.</span></span> <span data-ttu-id="c714a-119">Tačiau naudodami kai kurių tipų strategijas galite nepaisyti atskirų tipų strategijos taisyklių pirmumo tvarkos.</span><span class="sxs-lookup"><span data-stu-id="c714a-119">However, for some policy types, you can override the order of precedence for individual policy rule types.</span></span> <span data-ttu-id="c714a-120">Pvz., galite nustatyto tokią pirkimo strategijų pirmumo tvarką: išlaidų centras, padalinys, įmonė.</span><span class="sxs-lookup"><span data-stu-id="c714a-120">For example, you might define the order of precedence for purchasing policies to be: cost center, department, company.</span></span> <span data-ttu-id="c714a-121">Taikydami katalogo strategijos taisyklę galite nustatyti tokią pirmumo tvarką: padalinys, išlaidų centras, įmonė.</span><span class="sxs-lookup"><span data-stu-id="c714a-121">For the catalog policy rule, you might want the order of precedence to be: department, cost center, company.</span></span> <span data-ttu-id="c714a-122">Galite pakeisti katalogo strategijos taisyklės pirmumo tvarką.</span><span class="sxs-lookup"><span data-stu-id="c714a-122">You can change the order of precedence for the Catalog policy rule.</span></span> <span data-ttu-id="c714a-123">Kai darbuotojas sukuria paraišką, rodomas katalogas priklauso nuo strategijų, susijusių su darbuotojo padaliniu, tada – su jo išlaidų centru ir su įmone.</span><span class="sxs-lookup"><span data-stu-id="c714a-123">When a worker creates a requisition, the catalog that is displayed is determined by the policies that are associated with the worker’s department, then their cost center, and then their company.</span></span>  
    * <span data-ttu-id="c714a-124">Jei nurodytas daugiau nei vienas organizacinis lygis, galite naudoti rodyklę Aukštyn / Žemyn, kad nustatytumėte taisyklės Pirkimo paraiškos kontrolė pirmumo tvarką.</span><span class="sxs-lookup"><span data-stu-id="c714a-124">If there’s more than one organizational level listed, you can use the Up/Down arrows to set the order of precedence for the Purchase requisition control rule.</span></span>  
5. <span data-ttu-id="c714a-125">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="c714a-125">Close the page.</span></span>

## <a name="create-a-new-policy"></a><span data-ttu-id="c714a-126">Kurti naują strategiją</span><span class="sxs-lookup"><span data-stu-id="c714a-126">Create a new policy</span></span>
1. <span data-ttu-id="c714a-127">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="c714a-127">Click New.</span></span>
2. <span data-ttu-id="c714a-128">Lauke Pavadinimas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c714a-128">In the Name field, type a value.</span></span>
3. <span data-ttu-id="c714a-129">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c714a-129">In the Description field, type a value.</span></span>
    * <span data-ttu-id="c714a-130">Viena pirkimo strategija gali būti taikoma tik vienai organizacijos hierarchijai.</span><span class="sxs-lookup"><span data-stu-id="c714a-130">A single purchasing policy can only apply to one organization hierarchy.</span></span> <span data-ttu-id="c714a-131">Pvz., viena hierarchija vadinasi „Geografinė“, o kita – „Padalinys“, o joms priskirtos pirkimo strategijos skiriasi.</span><span class="sxs-lookup"><span data-stu-id="c714a-131">For example, you could have one hierarchy called “Geographic” and one called “Department”, and have a different purchasing policy for each.</span></span>  
    * <span data-ttu-id="c714a-132">Pasirinkite organizaciją, kuriai turėtų būti taikoma strategija.</span><span class="sxs-lookup"><span data-stu-id="c714a-132">Select an organization that the policy should apply to.</span></span>  
4. <span data-ttu-id="c714a-133">Norėdami įtraukti pasirinktą organizaciją, spustelėkite rodyklę.</span><span class="sxs-lookup"><span data-stu-id="c714a-133">Click the arrow to add the selected organization.</span></span>
    * <span data-ttu-id="c714a-134">Galite pakartoti šį procesą, norėdami įtraukti daugiau organizacijų.</span><span class="sxs-lookup"><span data-stu-id="c714a-134">You can repeat this process to add more organizations.</span></span>  

## <a name="add-a-policy-rule"></a><span data-ttu-id="c714a-135">Įtraukti strategijos taisyklę</span><span class="sxs-lookup"><span data-stu-id="c714a-135">Add a policy rule</span></span>
1. <span data-ttu-id="c714a-136">Sąraše Strategijos taisyklės tipas pasirinkite paraiškos paskirties taisyklę.</span><span class="sxs-lookup"><span data-stu-id="c714a-136">In the Policy rule type list, select Requisition purpose rule.</span></span>
    * <span data-ttu-id="c714a-137">Sukursite taisyklę, kuri numatytąją paraiškos paskirtį nustato į tipą Suvartojimas, bet suteikia galimybę jį pakeisti į tipą Papildymas.</span><span class="sxs-lookup"><span data-stu-id="c714a-137">You’ll create a rule that sets the default requisition purpose to type Consumption but allows the Replenishment type to be selected instead.</span></span>  
2. <span data-ttu-id="c714a-138">Spustelėkite Kurti strategijos taisyklę.</span><span class="sxs-lookup"><span data-stu-id="c714a-138">Click Create policy rule.</span></span>
3. <span data-ttu-id="c714a-139">Lauke Leisti neautomatiškai perrašyti pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="c714a-139">Select Yes in the Allow manual override field.</span></span>
4. <span data-ttu-id="c714a-140">Spustelėkite Uždaryti.</span><span class="sxs-lookup"><span data-stu-id="c714a-140">Click Close.</span></span>
    * <span data-ttu-id="c714a-141">Dabar galite nustatyti kitas pirkimo strategijos taisykles.</span><span class="sxs-lookup"><span data-stu-id="c714a-141">Now you can set up other policy rules for the purchasing policy.</span></span>   <span data-ttu-id="c714a-142">Atkreipkite dėmesį, tipe Strategijos taisyklė negali būti persidengiančių taisyklių, kurios vienu metu yra aktyvios vienoje įsigijimo strategijoje.</span><span class="sxs-lookup"><span data-stu-id="c714a-142">Note that a Policy rule type cannot have overlapping rules that are active at the same time within a single procurement policy.</span></span>  
5. <span data-ttu-id="c714a-143">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="c714a-143">Close the page.</span></span>
6. <span data-ttu-id="c714a-144">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="c714a-144">Close the page.</span></span>

