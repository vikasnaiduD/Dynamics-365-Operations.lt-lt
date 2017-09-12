--- 
title: "Nustatyti mobiliojo įrenginio meniu elementą gautoms prekėms registruoti"
description: "Ši užduotis sutelkta į mobiliojo įrenginio meniu elemento nustatymą."
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
ms.openlocfilehash: de976f6bafbb3d4e2915ab56cdff625877f754f7
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-a-mobile-device-menu-item-to-register-received-items"></a><span data-ttu-id="e5e72-103">Nustatyti mobiliojo įrenginio meniu elementą gautoms prekėms registruoti</span><span class="sxs-lookup"><span data-stu-id="e5e72-103">Set up a mobile device menu item to register received items</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="e5e72-104">Ši užduotis sutelkta į mobiliojo įrenginio meniu elemento nustatymą.</span><span class="sxs-lookup"><span data-stu-id="e5e72-104">This task focuses on the setup of a mobile device menu item.</span></span> <span data-ttu-id="e5e72-105">Šis meniu elementas naudojamas registruojant naudojantis pirkimo užsakymais užsakytų prekių gavimą.</span><span class="sxs-lookup"><span data-stu-id="e5e72-105">This menu item is used for registration of the receipt of items ordered via purchase orders.</span></span> 

<span data-ttu-id="e5e72-106">Šį vadovą galite naudoti demonstracinių duomenų įmonėje USMF.</span><span class="sxs-lookup"><span data-stu-id="e5e72-106">You can use this guide in demo data company USMF.</span></span> <span data-ttu-id="e5e72-107">Ši procedūra skirta sandėlio vadovui.</span><span class="sxs-lookup"><span data-stu-id="e5e72-107">This procedure is intended for the warehouse manager.</span></span>


## <a name="create-a-mobile-device-menu-item"></a><span data-ttu-id="e5e72-108">Mobiliojo įrenginio meniu elemento kūrimas</span><span class="sxs-lookup"><span data-stu-id="e5e72-108">Create a mobile device menu item</span></span>
1. <span data-ttu-id="e5e72-109">Pasirinkite Sandėlio valdymas > Nustatymas > Mobilusis įrenginys > Mobiliojo įrenginio meniu elementai.</span><span class="sxs-lookup"><span data-stu-id="e5e72-109">Go to Warehouse management > Setup > Mobile device > Mobile device menu items.</span></span>
2. <span data-ttu-id="e5e72-110">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="e5e72-110">Click New.</span></span>
3. <span data-ttu-id="e5e72-111">Lauke Meniu elemento pavadinimas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e5e72-111">In the Menu item name field, type a value.</span></span>
    * <span data-ttu-id="e5e72-112">Tai šio mobiliojo įrenginio meniu elemento unikalus identifikatorius.</span><span class="sxs-lookup"><span data-stu-id="e5e72-112">This is the unique identifier for this mobile device menu item.</span></span> <span data-ttu-id="e5e72-113">Pavyzdžiui, galite įvesti „Mano PO registracija“.</span><span class="sxs-lookup"><span data-stu-id="e5e72-113">For example, you could type 'My PO registration'.</span></span>  
4. <span data-ttu-id="e5e72-114">Lauke Pavadinimas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e5e72-114">In the Title field, type a value.</span></span>
    * <span data-ttu-id="e5e72-115">Tai yra pavadinimas, kuris bus rodomas vartotojui mobiliajame įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="e5e72-115">This is the title, which will be displayed to the user on the mobile device.</span></span> <span data-ttu-id="e5e72-116">Pavyzdžiui, galite įvesti „PO registracija“.</span><span class="sxs-lookup"><span data-stu-id="e5e72-116">For example, you could type 'PO registration'.</span></span>  
5. <span data-ttu-id="e5e72-117">Lauke Režimas pasirinkite „Darbas“.</span><span class="sxs-lookup"><span data-stu-id="e5e72-117">In the Mode field, select 'Work'.</span></span>
    * <span data-ttu-id="e5e72-118">Užregistravus turimus kiekius, gautus pirkimo užsakymo eilutei, bus sukuriamas darbas, kad būtų galima perkelti prekes iš gavimo skyriaus į atsargas.</span><span class="sxs-lookup"><span data-stu-id="e5e72-118">Registration of on-hand quantities received for a purchase order line will create work to move the items from the receiving area into the inventory.</span></span> <span data-ttu-id="e5e72-119">Darbo nesukuriamas, kol prekės neužregistruojamos.</span><span class="sxs-lookup"><span data-stu-id="e5e72-119">Work isn’t created until the items are registered.</span></span>  <span data-ttu-id="e5e72-120">Todėl palikite nustatytą parinkties Naudoti esamą darbą padėtį Ne.</span><span class="sxs-lookup"><span data-stu-id="e5e72-120">Therefore, leave the Use existing work option set to No.</span></span>  
6. <span data-ttu-id="e5e72-121">Išplėskite arba sutraukite dalį Bendra.</span><span class="sxs-lookup"><span data-stu-id="e5e72-121">Expand or collapse the General section.</span></span>
7. <span data-ttu-id="e5e72-122">Lauke Darbo kūrimo procesas pasirinkite„Gaunama pirkimo užsakymo prekė“.</span><span class="sxs-lookup"><span data-stu-id="e5e72-122">In the Work creation process field, select 'Purchase order item receiving'.</span></span>
    * <span data-ttu-id="e5e72-123">Norint užregistruoti turimą kiekį sandėlyje, pirkimo užsakymo eilutė turi būti unikaliai identifikuota.</span><span class="sxs-lookup"><span data-stu-id="e5e72-123">A purchase order line must be uniquely identified before on-hand can be registered in the warehouse.</span></span> <span data-ttu-id="e5e72-124">Šiuo atveju mobilusis įrenginys užregistruos pirkimo užsakymo numerį ir prekės numerį ir taip sistema galės identifikuoti PO eilutę.</span><span class="sxs-lookup"><span data-stu-id="e5e72-124">In this scenario, the mobile device will register the purchase order number and item number, and this will allow the system to identify the PO line.</span></span> <span data-ttu-id="e5e72-125">Bus sukurtas atidėjimo laikas ir galės išrinkti kitas darbuotojas.</span><span class="sxs-lookup"><span data-stu-id="e5e72-125">Put away work will be created and can be picked up by another worker.</span></span>    <span data-ttu-id="e5e72-126">Jūsų pasirinktas darbo kūrimo metodas nurodo, kurie laukai tampa pasiekiami skirtuke Bendra.</span><span class="sxs-lookup"><span data-stu-id="e5e72-126">The work creation method that you select determines which fields become available on the General fast tab.</span></span>  
    * <span data-ttu-id="e5e72-127">Jei pasirinksite pasirinktį Naudoti numatytuosius duomenis, įgalinamas mygtukas Numatytieji duomenys.</span><span class="sxs-lookup"><span data-stu-id="e5e72-127">If you select the Use default data option, the Default data button is enabled.</span></span> <span data-ttu-id="e5e72-128">Čia galite pasirinkti laukus, kuriuose bus rodomi duomenys, paprastai reikalingi darbuotojui kasdieniame jo darbe, kad šios reikšmės būtų rodomos mobiliajame įrenginyje.</span><span class="sxs-lookup"><span data-stu-id="e5e72-128">Here you can select fields to display data that a worker typically needs in their daily work, so that these values are shown on the mobile device.</span></span>  
    * <span data-ttu-id="e5e72-129">Numerio lentelių grupavimo parametras veikia kartu su vienetų sekų grupe, priskirta prie gaunamos prekės.</span><span class="sxs-lookup"><span data-stu-id="e5e72-129">The License plate grouping parameter  works in combination with the unit sequence group that’s assigned to the item that’s being received.</span></span> <span data-ttu-id="e5e72-130">Galite nurodyti, ar gavimus, mažesnius arba didesnius nei vienas padėklas, reikia grupuoti į vieną numerio lentelę, ar skaidyti į atskiras numerio lenteles kiekvienam vienetui.</span><span class="sxs-lookup"><span data-stu-id="e5e72-130">You can specify whether receipts of less than or more than one pallet should be grouped into one license plate, or divided into a separate license plate for each unit.</span></span>  
    * <span data-ttu-id="e5e72-131">Jei pasirinksite pasirinktį Generuoti numerio lentelę, pagal numeracijos pasirinkimą bus sugeneruotas unikalus numerio lentelės numeris.</span><span class="sxs-lookup"><span data-stu-id="e5e72-131">If you select the Generate license plate  option, this generates a unique license plate number based on the number sequence selection.</span></span>   
    * <span data-ttu-id="e5e72-132">Galite pasirinkti šabloną, kuris bus naudojamas kuriant darbą.</span><span class="sxs-lookup"><span data-stu-id="e5e72-132">You can select the template that will be used when work is created.</span></span> <span data-ttu-id="e5e72-133">Pavyzdžiui, jei registruojate pirkimo užsakymo prekę, atidėjimo darbas bus sugeneruotas remiantis darbo šablonu.</span><span class="sxs-lookup"><span data-stu-id="e5e72-133">For example, if you register an item for a purchase order, the put away work will be generated based on the work template.</span></span> <span data-ttu-id="e5e72-134">Jei čia nepasirinksite darbo šablono, sistema priskirs šabloną pagal užklausos kriterijus, kurie yra susieti su šablonais.</span><span class="sxs-lookup"><span data-stu-id="e5e72-134">If you don’t select a work template here, the system will assign a template based on the query criteria that are associated with the templates.</span></span>  
    * <span data-ttu-id="e5e72-135">Jei perdavimo kodai rodomi mobiliajame įrenginyje, darbuotojai gali įvertinti prekių būseną arba kokybę ir pasirinkti tinkamą kodą.</span><span class="sxs-lookup"><span data-stu-id="e5e72-135">If disposition codes are displayed on the mobile device, workers can evaluate the status or quality of the items, and select the appropriate code.</span></span> <span data-ttu-id="e5e72-136">Perdavimo kodo taisyklėse nurodoma, ar prekės bus pasiekiamos kitiems sandėlio procesams.</span><span class="sxs-lookup"><span data-stu-id="e5e72-136">The rules for  the disposition code determine whether the items will be available to other warehouse processes.</span></span> <span data-ttu-id="e5e72-137">Taisyklėse taip pat nurodoma, kuris sukurto darbo vietos nurodymas naudojamas.</span><span class="sxs-lookup"><span data-stu-id="e5e72-137">The rules also determine which location directive is used for the work that’s created.</span></span>   
    * <span data-ttu-id="e5e72-138">Jei pasirinksite parinktį Paketo perdavimo kodai, darbuotojai galės įvertinti paketo būseną arba kokybę ir pasirinkti tinkamą perdavimo kodą.</span><span class="sxs-lookup"><span data-stu-id="e5e72-138">If you select the Batch disposition codes option, workers can evaluate the status or quality of a batch, and select the appropriate disposition code.</span></span>  <span data-ttu-id="e5e72-139">Nustatytos paketo perdavimo kodo taisyklės lemia, ar paketas bus pasiekiamas kitiems sandėlio procesams.</span><span class="sxs-lookup"><span data-stu-id="e5e72-139">The rules that are set on the batch disposition code determine whether the batch will be available to other warehouse processes.</span></span>  
    * <span data-ttu-id="e5e72-140">Jei pasirinksite parinktį Spausdinti etiketes, numerio lentelės etiketė bus spausdinama automatiškai, kai gaunamos prekės.</span><span class="sxs-lookup"><span data-stu-id="e5e72-140">If you select the Print labels option a license plate label will be printed automatically when items are received.</span></span>  
8. <span data-ttu-id="e5e72-141">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="e5e72-141">Click Save.</span></span>
9. <span data-ttu-id="e5e72-142">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="e5e72-142">Close the page.</span></span>

## <a name="add-the-menu-item-to-a-mobile-device-menu"></a><span data-ttu-id="e5e72-143">Meniu elemento įtraukimas į mobiliojo įrenginio meniu</span><span class="sxs-lookup"><span data-stu-id="e5e72-143">Add the menu item to a mobile device menu</span></span>
1. <span data-ttu-id="e5e72-144">Pasirinkite Sandėlio valdymas > Nustatymas > Mobilusis įrenginys > Mobiliojo įrenginio meniu.</span><span class="sxs-lookup"><span data-stu-id="e5e72-144">Go to Warehouse management > Setup > Mobile device > Mobile device menu.</span></span>
2. <span data-ttu-id="e5e72-145">Naudokite spartųjį filtrą, kad atfiltruotumėte lauką Pavadinimas pagal reikšmę „gaunami“.</span><span class="sxs-lookup"><span data-stu-id="e5e72-145">Use the Quick Filter to filter on the Name field with a value of 'inbound'.</span></span>
3. <span data-ttu-id="e5e72-146">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="e5e72-146">Click Edit.</span></span>
4. <span data-ttu-id="e5e72-147">Medyje pasirinkite „Medyje Galimi meniu ir prekės pasirinkite anksčiau sukurtą meniu elementą.‟.</span><span class="sxs-lookup"><span data-stu-id="e5e72-147">In the tree, select 'In the Available menu's and items tree, select the menu item that you created before.'.</span></span>
    * <span data-ttu-id="e5e72-148">Pasirinkite meniu elementą, kurį sukūrėte anksčiau.</span><span class="sxs-lookup"><span data-stu-id="e5e72-148">Select the menu item that you created before.</span></span>  
5. <span data-ttu-id="e5e72-149">Spustelėkite į dešinę pusę rodančią rodyklę.</span><span class="sxs-lookup"><span data-stu-id="e5e72-149">Click on the arrow that points to the right.</span></span>
6. <span data-ttu-id="e5e72-150">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="e5e72-150">Click Save.</span></span>
7. <span data-ttu-id="e5e72-151">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="e5e72-151">Close the page.</span></span>

