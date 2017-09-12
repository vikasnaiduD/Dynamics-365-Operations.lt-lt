--- 
title: "Kurti pirkimo sutartį"
description: "Ši procedūra padės jums sukurti pirkimo sutartį."
author: mkirknel
manager: AnnBe
ms.date: 11/14/2016
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
ms.openlocfilehash: 0d0cc6508071bea3f622bc21f06aa55d2b757b6f
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="create-a-purchase-agreement"></a><span data-ttu-id="a4266-103">Kurti pirkimo sutartį</span><span class="sxs-lookup"><span data-stu-id="a4266-103">Create a purchase agreement</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="a4266-104">Ši procedūra padės jums sukurti pirkimo sutartį.</span><span class="sxs-lookup"><span data-stu-id="a4266-104">This procedure guides you through the creation of a purchase agreement.</span></span> <span data-ttu-id="a4266-105">Paprastai tai atlieka pirkimo vadybininkas.</span><span class="sxs-lookup"><span data-stu-id="a4266-105">This would typically be done by a purchasing manager.</span></span> <span data-ttu-id="a4266-106">Šią procedūrą galite atlikti demonstracinių duomenų įmonėje USMF arba su savo duomenimis.</span><span class="sxs-lookup"><span data-stu-id="a4266-106">You can use this procedure in demo data company USMF or on your own data.</span></span> <span data-ttu-id="a4266-107">Prieš pradėdami turite nustatyti pirkimo sutarčių klasifikacijas.</span><span class="sxs-lookup"><span data-stu-id="a4266-107">You need to have set up purchase agreement classifications before you start.</span></span> <span data-ttu-id="a4266-108">Sukūrę sutartį, galėsite ją naudoti, kai sukursite PU – pirkimo sutarties sąlygos bus nukopijuotos į antraštę ir į visas užsakymo eilutes, susijusias su šia sutartimi.</span><span class="sxs-lookup"><span data-stu-id="a4266-108">Once you've created an agreement you can use it when you create a PO, and this will copy the purchase agreement conditions to the header and to any lines in the order that are affected by the agreement.</span></span>


## <a name="create-a-new-purchase-agreement"></a><span data-ttu-id="a4266-109">Kurti naują pirkimo sutartį</span><span class="sxs-lookup"><span data-stu-id="a4266-109">Create a new purchase agreement</span></span>
1. <span data-ttu-id="a4266-110">Pasirinkite Pirkimai ir tiekėjų parinkimas > Pirkimo sutartys > Pirkimo sutartys.</span><span class="sxs-lookup"><span data-stu-id="a4266-110">Go to Procurement and sourcing > Purchase agreements > Purchase agreements.</span></span>
2. <span data-ttu-id="a4266-111">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="a4266-111">Click New.</span></span>
3. <span data-ttu-id="a4266-112">Lauke Tiekėjo sąskaita spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="a4266-112">In the Vendor account field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="a4266-113">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="a4266-113">In the list, find and select the desired record.</span></span>
5. <span data-ttu-id="a4266-114">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="a4266-114">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="a4266-115">Lauke „Pirkimo sutarties klasifikacija“ spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="a4266-115">In the Purchase agreement classification field, click the drop-down button to open the lookup.</span></span>
7. <span data-ttu-id="a4266-116">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="a4266-116">In the list, find and select the desired record.</span></span>
8. <span data-ttu-id="a4266-117">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="a4266-117">In the list, click the link in the selected row.</span></span>
9. <span data-ttu-id="a4266-118">Išplėskite skyrių Bendra.</span><span class="sxs-lookup"><span data-stu-id="a4266-118">Expand the General section.</span></span>
10. <span data-ttu-id="a4266-119">Lauke „Galiojimo data“ įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="a4266-119">In the Expiration date field, enter a date.</span></span>
    * <span data-ttu-id="a4266-120">Ši galiojimo data bus numatytoji visose įsipareigojimų eilutėse ir nulems, kiek laiko galios kiekvienas konkretus įsipareigojimas.</span><span class="sxs-lookup"><span data-stu-id="a4266-120">This expiration date will be the default for all commitment lines and will determine how long each specific commitment is valid.</span></span>  
11. <span data-ttu-id="a4266-121">Lauke „Dokumento pavadinimas“ įveskite pirkimo sutarties pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="a4266-121">In the Document title field, type a name for your purchase agreement.</span></span>
    * <span data-ttu-id="a4266-122">Palikite lauką „Numatytasis įsipareigojimas“ nustatytą kaip „Produkto kiekio įsipareigojimas“ (arba pakeiskite jį, jei jo nustatymas kitas).</span><span class="sxs-lookup"><span data-stu-id="a4266-122">Leave the Default commitment field set to Product quantity commitment (or change it if it’s not set to this).</span></span>  
    * <span data-ttu-id="a4266-123">Numatytoji įsipareigojimo reikšmė nurodo jūsų parinktis sutarties eilutėse.</span><span class="sxs-lookup"><span data-stu-id="a4266-123">The default commitment value determines your options on the agreement lines.</span></span> <span data-ttu-id="a4266-124">Jei jums reikia naujo įsipareigojimo tipo kuriant sutarties eilutes, turite pakeisti numatytąjį įsipareigojimą antraštėje.</span><span class="sxs-lookup"><span data-stu-id="a4266-124">If you need a new commitment type when you’re creating the agreement lines, you need to change the default commitment on the header.</span></span>  <span data-ttu-id="a4266-125">Yra 4 tipų įsipareigojimai: produkto kiekio įsipareigojimas – dėl konkretaus produkto kiekio; produkto vertės įsipareigojimas – dėl konkrečios produkto valiutos sumos; produkto kategorijos vertės įsipareigojimas – dėl konkrečios valiutos sumos įsigijimo kategorijoje, kurioje suma gali būti skirta kataloginei prekei arba nekataloginei prekei; vertės įsipareigojimas – dėl konkrečios valiutos sumos, kurią galima skirti bet kokiam produktui arba bet kokiai įsigijimo kategorijai.</span><span class="sxs-lookup"><span data-stu-id="a4266-125">There are 4 types of commitments: Product quantity commitment - for a specific quantity of a product; Product value commitment - for a specific currency amount of a product; Product category value commitment - for a specific currency amount in a procurement category where the amount can be for a catalog item or a non-catalog item; Value commitment - for a specific currency amount which can be fulfilled by any product or by any procurement category.</span></span>  
12. <span data-ttu-id="a4266-126">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="a4266-126">Click OK.</span></span>

## <a name="add-a-commitment"></a><span data-ttu-id="a4266-127">Įtraukti įsipareigojimą</span><span class="sxs-lookup"><span data-stu-id="a4266-127">Add a commitment</span></span>
1. <span data-ttu-id="a4266-128">Spustelėkite Pridėti eilutę.</span><span class="sxs-lookup"><span data-stu-id="a4266-128">Click Add line.</span></span>
2. <span data-ttu-id="a4266-129">Sąraše pažymėkite pasirinktą eilutę.</span><span class="sxs-lookup"><span data-stu-id="a4266-129">In the list, mark the selected row.</span></span>
3. <span data-ttu-id="a4266-130">Lauke Prekės numeris spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="a4266-130">In the Item number field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="a4266-131">Pasirinkite produktą, prie kurio norite pridėti įsipareigojimą.</span><span class="sxs-lookup"><span data-stu-id="a4266-131">Select the product you want to add a commitment for.</span></span>
5. <span data-ttu-id="a4266-132">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="a4266-132">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="a4266-133">Lauke Kiekis įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="a4266-133">In the Quantity field, enter a number.</span></span>
    * <span data-ttu-id="a4266-134">Tai yra bendras kiekis, kurį susitarėte pirkti iš tiekėjo.</span><span class="sxs-lookup"><span data-stu-id="a4266-134">This is the total quantity that you have agreed to buy from your vendor.</span></span>  
7. <span data-ttu-id="a4266-135">Lauke Vieneto kaina įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="a4266-135">In the Unit price field, enter a number.</span></span>
8. <span data-ttu-id="a4266-136">Išplėskite skyrių Eilutės informacija.</span><span class="sxs-lookup"><span data-stu-id="a4266-136">Expand the Line details section.</span></span>
9. <span data-ttu-id="a4266-137">Nustatykite parinkties „Maksimaliai vykdoma“ reikšmę „Taip“.</span><span class="sxs-lookup"><span data-stu-id="a4266-137">Set the Max is enforced option to Yes.</span></span>
    * <span data-ttu-id="a4266-138">Parinktis „Maksimaliai vykdoma“ riboja įsipareigojimų naudojimą.</span><span class="sxs-lookup"><span data-stu-id="a4266-138">The Max is enforced option limits the use of the commitment.</span></span> <span data-ttu-id="a4266-139">Galite pirkti tik tokį kiekį, kuris nurodytas eilutės lauke „Kiekis“.</span><span class="sxs-lookup"><span data-stu-id="a4266-139">You can only purchase up to the quantity that's specified in the Quantity field for the line.</span></span>  
10. <span data-ttu-id="a4266-140">Sutraukite skyrių „Eilutės informacija“.</span><span class="sxs-lookup"><span data-stu-id="a4266-140">Collapse the Line details section.</span></span>

## <a name="add-header-conditions"></a><span data-ttu-id="a4266-141">Įtraukti antraštės sąlygas</span><span class="sxs-lookup"><span data-stu-id="a4266-141">Add header conditions</span></span>
1. <span data-ttu-id="a4266-142">Veiksmų srityje spustelėkite Parinktys.</span><span class="sxs-lookup"><span data-stu-id="a4266-142">On the Action Pane, click Options.</span></span>
2. <span data-ttu-id="a4266-143">Spustelėkite Keisti rodinį.</span><span class="sxs-lookup"><span data-stu-id="a4266-143">Click Change view.</span></span>
3. <span data-ttu-id="a4266-144">Spustelėkite antraštės rodinį.</span><span class="sxs-lookup"><span data-stu-id="a4266-144">Click Header view.</span></span>
4. <span data-ttu-id="a4266-145">Išplėskite skyrių Sąlygos.</span><span class="sxs-lookup"><span data-stu-id="a4266-145">Expand the Terms section.</span></span>
5. <span data-ttu-id="a4266-146">Lauke Mokėjimo būdas spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="a4266-146">In the Method of payment field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="a4266-147">Čia pagal numatytuosius nustatymus rodomos mokėjimo sąlygos iš tiekėjo sąskaitos.</span><span class="sxs-lookup"><span data-stu-id="a4266-147">The payment terms from the vendor account are shown here by default.</span></span>       
6. <span data-ttu-id="a4266-148">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="a4266-148">In the list, find and select the desired record.</span></span>
7. <span data-ttu-id="a4266-149">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="a4266-149">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="a4266-150">Lauke „Pristatymo būdas“ spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="a4266-150">In the Mode of delivery field, click the drop-down button to open the lookup.</span></span>
9. <span data-ttu-id="a4266-151">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="a4266-151">In the list, click the link in the selected row.</span></span>
10. <span data-ttu-id="a4266-152">Lauke „Pristatymo sąlygos“ spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="a4266-152">In the Delivery terms field, click the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="a4266-153">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="a4266-153">In the list, click the link in the selected row.</span></span>

## <a name="confirm-and-activate-the-agreement"></a><span data-ttu-id="a4266-154">Patvirtinti ir aktyvinti sutartį</span><span class="sxs-lookup"><span data-stu-id="a4266-154">Confirm and activate the agreement</span></span>
1. <span data-ttu-id="a4266-155">Veiksmų srityje spustelėkite „Pardavimo sutartis“.</span><span class="sxs-lookup"><span data-stu-id="a4266-155">On the Action Pane, click Purchase agreement.</span></span>
2. <span data-ttu-id="a4266-156">Spustelėkite „Patvirtinimas“.</span><span class="sxs-lookup"><span data-stu-id="a4266-156">Click Confirmation.</span></span>
    * <span data-ttu-id="a4266-157">Nustatykite parinkties „Pažymėti sutartį kaip galiojančią“ reikšmę „Taip“.</span><span class="sxs-lookup"><span data-stu-id="a4266-157">Set the Mark agreement as effective option to Yes.</span></span>  
3. <span data-ttu-id="a4266-158">Spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="a4266-158">Click OK.</span></span>
4. <span data-ttu-id="a4266-159">Veiksmų srityje spustelėkite „Pardavimo sutartis“.</span><span class="sxs-lookup"><span data-stu-id="a4266-159">On the Action Pane, click Purchase agreement.</span></span>
5. <span data-ttu-id="a4266-160">Spustelėkite „Pirkimo sutarties patvirtinimai“.</span><span class="sxs-lookup"><span data-stu-id="a4266-160">Click Purchase agreement confirmations.</span></span>
    * <span data-ttu-id="a4266-161">Parinktis „Peržiūrėti / spausdinti“ leidžia generuoti pirkimo sutarties dokumentą, kurį paskui galite atspausdinti arba nusiųsti tiekėjui.</span><span class="sxs-lookup"><span data-stu-id="a4266-161">The Preview/Print option allows you to generate a document for the purchase agreement which you can then print or send to the vendor.</span></span> <span data-ttu-id="a4266-162">Jei vėliau sutartį atnaujinsite ir iš naujo patvirtinsite, abi jos versijos bus rodomas čia.</span><span class="sxs-lookup"><span data-stu-id="a4266-162">If you update the agreement later on and re-confirm it, both versions will be shown here.</span></span>  
6. <span data-ttu-id="a4266-163">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="a4266-163">Close the page.</span></span>

