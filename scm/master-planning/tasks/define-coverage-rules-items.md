--- 
title: "Apibrėžti prekių padengimo taisykles"
description: "Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF."
author: YuyuScheller
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
ms.author: yuyus
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 14f56c30753da9458d66a46da8935305619fd0b8
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="define-coverage-rules-for-items"></a><span data-ttu-id="2ec83-103">Apibrėžti prekių padengimo taisykles</span><span class="sxs-lookup"><span data-stu-id="2ec83-103">Define coverage rules for items</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="2ec83-104">Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.</span><span class="sxs-lookup"><span data-stu-id="2ec83-104">The demo data company used to create this procedure is USMF.</span></span> <span data-ttu-id="2ec83-105">Šioje procedūroje nurodoma, kaip kurti padengimo taisykles ir nepaisyti konkrečios prekės padengimo parametrų.</span><span class="sxs-lookup"><span data-stu-id="2ec83-105">This procedure shows how to create coverage rules and override coverage settings for a specific item.</span></span> <span data-ttu-id="2ec83-106">Jis taip pat parodo, kaip nurodyti numatytąsias atsargų nuostatas.</span><span class="sxs-lookup"><span data-stu-id="2ec83-106">It also shows how to specify default inventory settings.</span></span>


## <a name="create-a-coverage-group"></a><span data-ttu-id="2ec83-107">Padengimo grupės kūrimas</span><span class="sxs-lookup"><span data-stu-id="2ec83-107">Create a coverage group</span></span>
1. <span data-ttu-id="2ec83-108">Eikite į Padengimo grupės.</span><span class="sxs-lookup"><span data-stu-id="2ec83-108">Go to Coverage groups.</span></span>
2. <span data-ttu-id="2ec83-109">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="2ec83-109">Click New.</span></span>
3. <span data-ttu-id="2ec83-110">Lauke Padengimo grupė įveskite vertę.</span><span class="sxs-lookup"><span data-stu-id="2ec83-110">In the Coverage group field, type a value.</span></span>
4. <span data-ttu-id="2ec83-111">Lauke Pavadinimas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="2ec83-111">In the Name field, type a value.</span></span>
5. <span data-ttu-id="2ec83-112">Lauke Kalendorius įveskite vertę.</span><span class="sxs-lookup"><span data-stu-id="2ec83-112">In the Calendar field, type a value.</span></span>
    * <span data-ttu-id="2ec83-113">Pasirinkite kalendorių, kurį bendrasis planavimas naudos norėdamas sukurti šios grupės prekių papildymo pasiūlymus.</span><span class="sxs-lookup"><span data-stu-id="2ec83-113">Choose the calendar that master planning uses to create replenishment suggestions for items in this group.</span></span>  
6. <span data-ttu-id="2ec83-114">Lauke Padengimo kodas pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="2ec83-114">In the Coverage code field, select an option.</span></span>
    * <span data-ttu-id="2ec83-115">Pasirinkite Reikalavimai šiai procedūrai.</span><span class="sxs-lookup"><span data-stu-id="2ec83-115">Select Requirement for this procedure.</span></span>  
7. <span data-ttu-id="2ec83-116">Lauke Padengimo laiko ribos (dienomis) įveskite „90‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-116">In the Coverage time fence (days) field, enter '90'.</span></span>
    * <span data-ttu-id="2ec83-117">Prekėms šioje grupėje bendrasis planavimas iki 90 dienų ateityje kurs papildymo pasiūlymus.</span><span class="sxs-lookup"><span data-stu-id="2ec83-117">For items in this group, master planning will create replenishment suggestions for up to 90 days in the future.</span></span>  
8. <span data-ttu-id="2ec83-118">Lauke Neigiamos dienos įveskite „1‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-118">In the Negative days field, enter '1'.</span></span>
9. <span data-ttu-id="2ec83-119">Lauke Teigiamos dienos įveskite „1‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-119">In the Positive days field, enter '1'.</span></span>
10. <span data-ttu-id="2ec83-120">Išplėskite arba sutraukite sekciją Kita.</span><span class="sxs-lookup"><span data-stu-id="2ec83-120">Expand or collapse the Other section.</span></span>
11. <span data-ttu-id="2ec83-121">Lauke Gavimo laiko rezervas, pridėtas prie pareikalavimo datos įveskite „1‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-121">In the Receipt margin added to requirement date field, enter '1'.</span></span>
    * <span data-ttu-id="2ec83-122">Pavyzdžiui, jei nustatytas 1 dienos gavimo laiko rezervas, o pirkimo užsakymo eilutę planuojama gauti gegužės 15 d., bendrajame planavime gavimo data bus pakoreguota į gegužės 16 d.</span><span class="sxs-lookup"><span data-stu-id="2ec83-122">For example, if the receipt margin is set to 1 day, and a purchase order line is scheduled for receipt on May 15, master planning calculates the adjusted receipt date as May 16.</span></span>  
12. <span data-ttu-id="2ec83-123">Lauke Išdavimo laiko rezervas, atimtas iš pareikalavimo datos įveskite „1‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-123">In the Issue margin deducted from requirement date field, enter '1'.</span></span>
    * <span data-ttu-id="2ec83-124">Pavyzdžiui, jei nustatytas 1 dienos laiko rezervas, o pardavimo užsakymo eilutę planuojama pristatyti gegužės 15 d., bendrajame planavime pristatymo data bus pakoreguota į gegužės 14 d.</span><span class="sxs-lookup"><span data-stu-id="2ec83-124">For example, if the safety margin is set to 1 day, and a sales order line is scheduled for delivery on May 15, master scheduling calculates the adjusted delivery date as May 14.</span></span>  
13. <span data-ttu-id="2ec83-125">Lauke Keisti maržos, įtrauktos į prekės gamybos laiką, tvarką įveskite „1‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-125">In the Reorder margin added to item lead time field, enter '1'.</span></span>
14. <span data-ttu-id="2ec83-126">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="2ec83-126">Click Save.</span></span>

## <a name="create-a-new-product"></a><span data-ttu-id="2ec83-127">Kurti naują produktą</span><span class="sxs-lookup"><span data-stu-id="2ec83-127">Create a new product</span></span>
1. <span data-ttu-id="2ec83-128">Eikite į Išleisti produktai.</span><span class="sxs-lookup"><span data-stu-id="2ec83-128">Go to Released products.</span></span>
2. <span data-ttu-id="2ec83-129">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="2ec83-129">Click New.</span></span>
3. <span data-ttu-id="2ec83-130">Lauke „Produkto numeris“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="2ec83-130">In the Product number field, type a value.</span></span>
4. <span data-ttu-id="2ec83-131">Lauke Produkto pavadinimas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="2ec83-131">In the Product name field, type a value.</span></span>
5. <span data-ttu-id="2ec83-132">Lauke Prekių modelių grupė spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-132">In the Item model group field, click the drop-down button to open the lookup.</span></span>
6. <span data-ttu-id="2ec83-133">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-133">In the list, find and select the desired record.</span></span>
7. <span data-ttu-id="2ec83-134">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="2ec83-134">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="2ec83-135">Lauke Prekių grupė spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-135">In the Item group field, click the drop-down button to open the lookup.</span></span>
9. <span data-ttu-id="2ec83-136">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-136">In the list, find and select the desired record.</span></span>
10. <span data-ttu-id="2ec83-137">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="2ec83-137">In the list, click the link in the selected row.</span></span>
11. <span data-ttu-id="2ec83-138">Lauke Saugojimo dimensijų grupė spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-138">In the Storage dimension group field, click the drop-down button to open the lookup.</span></span>
12. <span data-ttu-id="2ec83-139">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-139">In the list, find and select the desired record.</span></span>
13. <span data-ttu-id="2ec83-140">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="2ec83-140">In the list, click the link in the selected row.</span></span>
14. <span data-ttu-id="2ec83-141">Lauke Sekimo dimensijų grupė spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-141">In the Tracking dimension group field, click the drop-down button to open the lookup.</span></span>
15. <span data-ttu-id="2ec83-142">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-142">In the list, find and select the desired record.</span></span>
16. <span data-ttu-id="2ec83-143">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="2ec83-143">In the list, click the link in the selected row.</span></span>
17. <span data-ttu-id="2ec83-144">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="2ec83-144">Click OK.</span></span>

## <a name="setup-default-order-settings"></a><span data-ttu-id="2ec83-145">Nustatyti numatytąsias užsakymo nuostatas</span><span class="sxs-lookup"><span data-stu-id="2ec83-145">Setup default order settings</span></span>
1. <span data-ttu-id="2ec83-146">Veiksmų srityje spustelėkite Planuoti.</span><span class="sxs-lookup"><span data-stu-id="2ec83-146">On the Action Pane, click Plan.</span></span>
2. <span data-ttu-id="2ec83-147">Spustelėkite Numatytosios užsakymo nuostatos.</span><span class="sxs-lookup"><span data-stu-id="2ec83-147">Click Default order settings.</span></span>
3. <span data-ttu-id="2ec83-148">Lauke Pirkimo teritorija įveskite teritoriją, kuri naudojama kaip numatytoji, kai kuriami pirkimo užsakymai.</span><span class="sxs-lookup"><span data-stu-id="2ec83-148">In the Purchase site field, type the site used as default when purchase orders are created.</span></span>
4. <span data-ttu-id="2ec83-149">Lauke Atsargų vieta įveskite vietą, kurioje saugoma prekė.</span><span class="sxs-lookup"><span data-stu-id="2ec83-149">In the Inventory site field, type the site where the item is stored.</span></span>
5. <span data-ttu-id="2ec83-150">Išplėskite arba sutraukite sekciją Atsargos.</span><span class="sxs-lookup"><span data-stu-id="2ec83-150">Expand or collapse the Inventory section.</span></span>
6. <span data-ttu-id="2ec83-151">Kartotinį nustatykite į „10‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-151">Set Multiple to '10'.</span></span>
7. <span data-ttu-id="2ec83-152">Min.</span><span class="sxs-lookup"><span data-stu-id="2ec83-152">Set Min.</span></span> <span data-ttu-id="2ec83-153">užsakymų kiekį nustatykite į „10‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-153">order quantity to '10'.</span></span>
8. <span data-ttu-id="2ec83-154">Maks.</span><span class="sxs-lookup"><span data-stu-id="2ec83-154">Set Max.</span></span> <span data-ttu-id="2ec83-155">užsakymų kiekį nustatykite į „100‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-155">order quantity to '100'.</span></span>
9. <span data-ttu-id="2ec83-156">Standartinį užsakymų kiekį nustatykite į „10‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-156">Set Standard order quantity to '10'.</span></span>
10. <span data-ttu-id="2ec83-157">Lauke Pirkimo vykdymo laikas įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="2ec83-157">In the Purchase lead time field, enter a number.</span></span>
11. <span data-ttu-id="2ec83-158">Pažymėkite arba išvalykite žymės langelį Darbo dienos.</span><span class="sxs-lookup"><span data-stu-id="2ec83-158">Select or clear the Working days check box.</span></span>
12. <span data-ttu-id="2ec83-159">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="2ec83-159">Click Save.</span></span>
13. <span data-ttu-id="2ec83-160">Lauke Numatytasis užsakymo tipas pasirinkite „Pirkimo užsakymas“.</span><span class="sxs-lookup"><span data-stu-id="2ec83-160">In the Default order type field select 'Purchase order'.</span></span>
14. <span data-ttu-id="2ec83-161">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="2ec83-161">Click Save.</span></span>
15. <span data-ttu-id="2ec83-162">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="2ec83-162">Close the page.</span></span>
    * <span data-ttu-id="2ec83-163">Uždarykite puslapį Numatytieji užsakymo parametrai.</span><span class="sxs-lookup"><span data-stu-id="2ec83-163">Close the Default order settings page.</span></span>  

## <a name="add-an-item-to-a-coverage-group"></a><span data-ttu-id="2ec83-164">Pridėti prekę į padengimo grupę</span><span class="sxs-lookup"><span data-stu-id="2ec83-164">Add an item to a coverage group</span></span>
1. <span data-ttu-id="2ec83-165">Išplėskite arba sutraukite sekciją Planas.</span><span class="sxs-lookup"><span data-stu-id="2ec83-165">Expand or collapse the Plan section.</span></span>
2. <span data-ttu-id="2ec83-166">Lauke Padengimo grupė spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="2ec83-166">In the Coverage group field, click the drop-down button to open the lookup.</span></span>
3. <span data-ttu-id="2ec83-167">Sąraše raskite padengimo grupę, kurią sukūrėte.</span><span class="sxs-lookup"><span data-stu-id="2ec83-167">In the list, find the Coverage group you have created.</span></span>
4. <span data-ttu-id="2ec83-168">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="2ec83-168">In the list, click the link in the selected row.</span></span>

## <a name="create-item-coverage-rules"></a><span data-ttu-id="2ec83-169">Kurti prekių padengimo taisykles</span><span class="sxs-lookup"><span data-stu-id="2ec83-169">Create item coverage rules</span></span>
1. <span data-ttu-id="2ec83-170">Veiksmų srityje spustelėkite Planuoti.</span><span class="sxs-lookup"><span data-stu-id="2ec83-170">On the Action Pane, click Plan.</span></span>
2. <span data-ttu-id="2ec83-171">Spustelėkite Prekės padengimas.</span><span class="sxs-lookup"><span data-stu-id="2ec83-171">Click Item coverage.</span></span>
3. <span data-ttu-id="2ec83-172">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="2ec83-172">Click New.</span></span>
4. <span data-ttu-id="2ec83-173">Spustelėkite skirtuką Bendra.</span><span class="sxs-lookup"><span data-stu-id="2ec83-173">Click the General tab.</span></span>
5. <span data-ttu-id="2ec83-174">Pažymėkite funkcijos Nepaisyti padengimo grupės parametrų antraštės langelį.</span><span class="sxs-lookup"><span data-stu-id="2ec83-174">Check the box on the header of Override coverage group settings.</span></span>
6. <span data-ttu-id="2ec83-175">Lauke Padengimo laiko ribos (dienomis) įveskite „60‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-175">In the Coverage time fence (days) field, enter '60'.</span></span>
    * <span data-ttu-id="2ec83-176">Nors prekės padengimo grupėje Poreikis yra planuojamos 90 dienų į priekį, ši prekė bus planuojama 60 dienų į priekį.</span><span class="sxs-lookup"><span data-stu-id="2ec83-176">Although items in coverage group Requiremen are planned 90 days ahead, this item will be planned 60 days ahead.</span></span>  
7. <span data-ttu-id="2ec83-177">Lauke Neigiamos dienos įveskite „2‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-177">In the Negative days field, enter '2'.</span></span>
8. <span data-ttu-id="2ec83-178">Lauke Teigiamos dienos įveskite „2‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-178">In the Positive days field, enter '2'.</span></span>
9. <span data-ttu-id="2ec83-179">Spustelėkite skirtuką Gamybos laikas.</span><span class="sxs-lookup"><span data-stu-id="2ec83-179">Click the Lead time tab.</span></span>
10. <span data-ttu-id="2ec83-180">Pažymėkite antraštės Pirkimas langelį.</span><span class="sxs-lookup"><span data-stu-id="2ec83-180">Check the box on the header of Purchase.</span></span>
11. <span data-ttu-id="2ec83-181">Lauke Pirkimo laikas įveskite „5‟.</span><span class="sxs-lookup"><span data-stu-id="2ec83-181">In the Purchase time field, enter '5'.</span></span>
12. <span data-ttu-id="2ec83-182">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="2ec83-182">Click Save.</span></span>

