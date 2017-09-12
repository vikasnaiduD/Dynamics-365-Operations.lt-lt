--- 
title: "Kurti vartojimo paraišką"
description: "Ši procedūra žingsnis po žingsnio supažindins su paraiškos kūrimo procesu."
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
ms.openlocfilehash: 07fe007005fcbbac1beecadb14dbd752376a0bd4
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="create-a-requisition-for-consumption"></a><span data-ttu-id="e6097-103">Kurti vartojimo paraišką</span><span class="sxs-lookup"><span data-stu-id="e6097-103">Create a requisition for consumption</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="e6097-104">Ši procedūra žingsnis po žingsnio supažindins su paraiškos kūrimo procesu.</span><span class="sxs-lookup"><span data-stu-id="e6097-104">This procedure walks you through the process of creating a requisition.</span></span> <span data-ttu-id="e6097-105">Ji parodo skirtingus produktų paieškos įsigijimo kataloge būdus ir kaip įtraukti produktą, kurio nėra kataloge.</span><span class="sxs-lookup"><span data-stu-id="e6097-105">It shows you different ways to search for products in your procurement catalogue and how to add a product that isn’t in your catalogue.</span></span> <span data-ttu-id="e6097-106">Prieš pradėdami šią procedūrą, pirkimo strategiją numatytuoju paraiškos tipu turite nustatyti suvartojimą.</span><span class="sxs-lookup"><span data-stu-id="e6097-106">Before you start this procedure, you must have a purchasing policy set up with Consumption as the default type of requisition.</span></span> <span data-ttu-id="e6097-107">Šią procedūrą galite atlikti naudodami demonstracinių duomenų įmonę USMF arba savo duomenis.</span><span class="sxs-lookup"><span data-stu-id="e6097-107">You can walk through this procedure in demo data company USMF, or using your own data.</span></span> <span data-ttu-id="e6097-108">Procedūrą galima atlikti tik iš vartotojo profilio, kuris nustatytas kaip darbuotojo.</span><span class="sxs-lookup"><span data-stu-id="e6097-108">The procedure can only be carried out by a user profile that is set up as worker.</span></span>  <span data-ttu-id="e6097-109">Šiią užduotį paprastai atlieka darbuotojas.</span><span class="sxs-lookup"><span data-stu-id="e6097-109">This task would normally be carried out by an employee.</span></span> <span data-ttu-id="e6097-110">Užduotis galėsite atlikti per darbuotojo saugos vaidmenį arba, jei naudojate USMF, galite prisijungti kaip Alicia.</span><span class="sxs-lookup"><span data-stu-id="e6097-110">The Employee employ security role will allow you to carry out the tasks, or if you’re using USMF, you can log in as Alicia.</span></span>


## <a name="create-a-new-requisition"></a><span data-ttu-id="e6097-111">Kurti naują paraišką</span><span class="sxs-lookup"><span data-stu-id="e6097-111">Create a new requisition</span></span>
1. <span data-ttu-id="e6097-112">Pasirinkite Pirkimai ir tiekėjų parinkimas > Pirkimo paraiškos > Mano parengtos pirkimo paraiškos.</span><span class="sxs-lookup"><span data-stu-id="e6097-112">Go to Procurement and sourcing > Purchase requisitions > Purchase requisitions prepared by me.</span></span>
2. <span data-ttu-id="e6097-113">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="e6097-113">Click New.</span></span>
3. <span data-ttu-id="e6097-114">Lauke „Pavadiniams“ suteikite paraiškai pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="e6097-114">In the Name field, give the requisition a name.</span></span>
4. <span data-ttu-id="e6097-115">Lauke „Pageidaujama data“ įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="e6097-115">In the Requested date field, enter a date.</span></span>
    * <span data-ttu-id="e6097-116">Pagal numatytuosius nustatymus, pageidaujama data ir apskaitos data nukopijuojamos į pirkimo paraiškos eilutes.</span><span class="sxs-lookup"><span data-stu-id="e6097-116">By default, the requested date and accounting date are copied to the purchase requisition lines.</span></span> <span data-ttu-id="e6097-117">Jas galima keisti eilučių lygmeniu.</span><span class="sxs-lookup"><span data-stu-id="e6097-117">They can be changed at the line level.</span></span> <span data-ttu-id="e6097-118">Pareikalauta data – tai pageidaujama pristatymo data.</span><span class="sxs-lookup"><span data-stu-id="e6097-118">The requested date is the requested delivery date.</span></span>  
5. <span data-ttu-id="e6097-119">Lauke „Apskaitos data“ įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="e6097-119">In the Accounting date field, enter a date.</span></span>
    * <span data-ttu-id="e6097-120">Apskaitos data naudojama įrašant apskaitos įrašą didžiojoje knygoje bei tikrinant, ar yra biudžeto lėšų.</span><span class="sxs-lookup"><span data-stu-id="e6097-120">The accounting date is used to record the accounting entry in the general ledger, and to validate whether budget funds are available.</span></span>  
6. <span data-ttu-id="e6097-121">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="e6097-121">Click OK.</span></span>
7. <span data-ttu-id="e6097-122">Lauke „Priežastis“ spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="e6097-122">In the Reason field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="e6097-123">Pagal nustatytuosius parametrus, jūsų pasirinkta verslo pagrindimo priežastis rodoma pirkimo paraiškos eilutėse, bet galite ją pakeisti eilutės lygmeniu.</span><span class="sxs-lookup"><span data-stu-id="e6097-123">By default, the business justification reason that you select appears for the purchase requisition lines, but you can change it at the line level.</span></span>    
8. <span data-ttu-id="e6097-124">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="e6097-124">In the list, find and select the desired record.</span></span>
9. <span data-ttu-id="e6097-125">Pasirinkti priežastį</span><span class="sxs-lookup"><span data-stu-id="e6097-125">Select the reason</span></span>
10. <span data-ttu-id="e6097-126">Informacija lauke įveskite išsamesnį paraiškos pagrindimą</span><span class="sxs-lookup"><span data-stu-id="e6097-126">In the details field enter a more descriptive justification for the requisition</span></span>

## <a name="add-a-line-to-the-requisition"></a><span data-ttu-id="e6097-127">Įtraukti eilutę į paraišką</span><span class="sxs-lookup"><span data-stu-id="e6097-127">Add a line to the requisition</span></span>
1. <span data-ttu-id="e6097-128">Spustelėkite Pridėti eilutę.</span><span class="sxs-lookup"><span data-stu-id="e6097-128">Click Add line.</span></span>
    * <span data-ttu-id="e6097-129">Pridėti eilutes į pirkimo paraišką galima dviem būdais.</span><span class="sxs-lookup"><span data-stu-id="e6097-129">There are two ways of adding lines to the purchase requisition.</span></span> <span data-ttu-id="e6097-130">Jei jau žinote produkto numerį arba jau žinote, kad jums reikalingo produkto kataloge nėra, galite pridėti eilutę tiesiogiai, paspaudę „Įtraukti eilutę“.</span><span class="sxs-lookup"><span data-stu-id="e6097-130">If you already know the product number or you already  know that you are requesting a product that is not in the product catalogueue, then you can add the line directly with "Add line".</span></span> <span data-ttu-id="e6097-131">Kitas būdas yra paspausti „Pridėti produktus“, kur galite naudoti paiešką ir filtravimą, kad rastumėte prekes produktų kataloge.</span><span class="sxs-lookup"><span data-stu-id="e6097-131">The other way is to use "Add products" where you can use searching and filtering to find items in the product catalogueue.</span></span>    
2. <span data-ttu-id="e6097-132">Spustelėkite eilutę, kurią ką tik sukūrėte.</span><span class="sxs-lookup"><span data-stu-id="e6097-132">Click on the row you just created.</span></span>
    * <span data-ttu-id="e6097-133">Prašytojas yra darbuotojas, kuris paprašė leisti rengti paraišką.</span><span class="sxs-lookup"><span data-stu-id="e6097-133">The requester is the worker that has requested the requisition.</span></span>   
    * <span data-ttu-id="e6097-134">Pagal numatytuosius nustatymus, paraišką rengiantis asmuo yra to prašęs darbuotojas.</span><span class="sxs-lookup"><span data-stu-id="e6097-134">By default the person preparing the requisition is the worker who has requested it.</span></span> <span data-ttu-id="e6097-135">Norėdami parengti paraiškos eilutę kito darbuotojo vardu turėsite gauti leidimą.</span><span class="sxs-lookup"><span data-stu-id="e6097-135">You have to be given permission to prepare a requisition line on behalf of another worker.</span></span> <span data-ttu-id="e6097-136">Jei tokius leidimus turite, tada šioje paieškoje bus rodomi kiti darbuotojai.</span><span class="sxs-lookup"><span data-stu-id="e6097-136">If you have such permissions then the other workers will show up in this lookup.</span></span>  
3. <span data-ttu-id="e6097-137">Lauke Prekės numeris surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e6097-137">In the Item number field, type a value.</span></span>
    * <span data-ttu-id="e6097-138">Prekes, iš kurių galite rinktis, riboja kategorijos prieigos strategija ir perkančio juridinio subjekto įsigijimo katalogas.</span><span class="sxs-lookup"><span data-stu-id="e6097-138">The items that are available for you to choose are limited by the category access policy and the procurement catalogue for the buying legal entity.</span></span>   
4. <span data-ttu-id="e6097-139">Lauke Kiekis įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e6097-139">In the Quantity field, enter a number.</span></span>

## <a name="add-more-products-to-the-requisition"></a><span data-ttu-id="e6097-140">Įtraukti daugiau produktų į paraišką</span><span class="sxs-lookup"><span data-stu-id="e6097-140">Add more products to the requisition</span></span>
1. <span data-ttu-id="e6097-141">Spustelėkite „Įtraukti produktus“.</span><span class="sxs-lookup"><span data-stu-id="e6097-141">Click Add products.</span></span>
    * <span data-ttu-id="e6097-142">Ši parinktis leidžia ieškoti produktų kataloge.</span><span class="sxs-lookup"><span data-stu-id="e6097-142">This is the option where you can search for products in the product catalogueue.</span></span>    
2. <span data-ttu-id="e6097-143">Lauke „Rasti įsigijimo kategorijos mazgą“ įveskite pirmąją jūsų ieškomos kategorijos pavadinimo dalį, tada paspauskite „Įvesti“.</span><span class="sxs-lookup"><span data-stu-id="e6097-143">In the Find procurement category node field, type the first part of the name of the category that you are looking for, and then click Enter.</span></span>
    * <span data-ttu-id="e6097-144">Pvz., įveskite „kompiut“.</span><span class="sxs-lookup"><span data-stu-id="e6097-144">For example, type comput.</span></span>  
3. <span data-ttu-id="e6097-145">Naudokite InvokeDefaultButton sparčiuosius klavišus.</span><span class="sxs-lookup"><span data-stu-id="e6097-145">Use the InvokeDefaultButton shortcut.</span></span>
4. <span data-ttu-id="e6097-146">Naudokite filtrą pasirinktos kategorijos produktų sąrašui filtruoti.</span><span class="sxs-lookup"><span data-stu-id="e6097-146">Use the Filter to filter the list of products in the selected category.</span></span>
5. <span data-ttu-id="e6097-147">Pasirinkite produkto kortelę, kurią norite įtraukti į paraišką.</span><span class="sxs-lookup"><span data-stu-id="e6097-147">Select the product card that you want to add to the requisition.</span></span>
6. <span data-ttu-id="e6097-148">Spustelėkite „Įtraukti į eilutes“.</span><span class="sxs-lookup"><span data-stu-id="e6097-148">Click Add to lines.</span></span>
7. <span data-ttu-id="e6097-149">Lauke Kiekis įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e6097-149">In the Quantity field, enter a number.</span></span>
8. <span data-ttu-id="e6097-150">Lauke „Rasti įsigijimo kategorijos mazgą“ įveskite pirmąją jūsų ieškomos kategorijos pavadinimo dalį, tada paspauskite „Įvesti“.</span><span class="sxs-lookup"><span data-stu-id="e6097-150">In the Find procurement category node field, type the first part of the name of the category that you are looking for, and then click Enter.</span></span>
    * <span data-ttu-id="e6097-151">Pvz., įveskite „žym“ (žymekliai).</span><span class="sxs-lookup"><span data-stu-id="e6097-151">For example, type High (highlighters).</span></span>  
9. <span data-ttu-id="e6097-152">Naudokite InvokeDefaultButton sparčiuosius klavišus.</span><span class="sxs-lookup"><span data-stu-id="e6097-152">Use the InvokeDefaultButton shortcut.</span></span>
10. <span data-ttu-id="e6097-153">Spustelėkite „Įtraukti į eilutes produktą ne iš sąrašo“, kad pridėtumėte produktą, kurio nėra įsigijimo kataloge.</span><span class="sxs-lookup"><span data-stu-id="e6097-153">Click Add unlisted product to lines to add a product that’s not listed in the procurement catalogue.</span></span>
11. <span data-ttu-id="e6097-154">Lauke Produkto pavadinimas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e6097-154">In the Product name field, type a value.</span></span>
12. <span data-ttu-id="e6097-155">Lauke „Vienetas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e6097-155">In the Unit field, type a value.</span></span>
13. <span data-ttu-id="e6097-156">Spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="e6097-156">Click OK.</span></span>
14. <span data-ttu-id="e6097-157">Lauke „Prekės aprašas“ pridėkite produkto aprašą.</span><span class="sxs-lookup"><span data-stu-id="e6097-157">In the Item description field, add a description of the product.</span></span>
15. <span data-ttu-id="e6097-158">Lauke Kiekis įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e6097-158">In the Quantity field, enter a number.</span></span>
16. <span data-ttu-id="e6097-159">Lauke Vieneto kaina įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="e6097-159">In the Unit price field, enter a number.</span></span>
    * <span data-ttu-id="e6097-160">Jei žinote konkretaus tiekėjo kainą (kurią pasirenkate tiekėjo sąskaitos lauke), tada galite įvesti šią kainą</span><span class="sxs-lookup"><span data-stu-id="e6097-160">If you know the price for a particular vendor (that you select in the vendor account field) then that price can be entered</span></span>   
17. <span data-ttu-id="e6097-161">Lauke Tiekėjo sąskaita spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="e6097-161">In the Vendor account field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="e6097-162">Kokie tiekėjai bus šiame lauke priklauso nuo pirkimo strategijų ir tiekėjo būsenos esamoje įsigijimo kategorijoje.</span><span class="sxs-lookup"><span data-stu-id="e6097-162">The vendors that are available in this field depend on the purchasing policies and the status that the vendor has for the current procurement category.</span></span> <span data-ttu-id="e6097-163">Tiekėją galite pasirinkti ne tik čia – taip pat galite spustelėti mygtuką „Siūlyti tiekėją“.</span><span class="sxs-lookup"><span data-stu-id="e6097-163">As an alternative to selecting a vendor here, you can click the Suggest vendor button.</span></span>    
18. <span data-ttu-id="e6097-164">Sąrašo pasirinkite tiekėją, kurį norite naudoti.</span><span class="sxs-lookup"><span data-stu-id="e6097-164">In the list, select the vendor you want to use.</span></span>
19. <span data-ttu-id="e6097-165">Lauke „Išorinis prekės numeris“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="e6097-165">In the External item number field, type a value.</span></span>
    * <span data-ttu-id="e6097-166">Tai yra produkto nuorodos numeris, kurį žino tiekėjas.</span><span class="sxs-lookup"><span data-stu-id="e6097-166">This is a reference number for the product that is known by the vendor.</span></span> <span data-ttu-id="e6097-167">Pvz., tai gali būti prekės numeris tiekėjo produktų kataloge.</span><span class="sxs-lookup"><span data-stu-id="e6097-167">For example, this could be the item number of the product in the vendor's own catalogue.</span></span>  
20. <span data-ttu-id="e6097-168">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="e6097-168">Click OK.</span></span>

## <a name="distribute-amounts"></a><span data-ttu-id="e6097-169">Paskirstyti sumas</span><span class="sxs-lookup"><span data-stu-id="e6097-169">Distribute amounts</span></span>
1. <span data-ttu-id="e6097-170">Spustelėkite Finansai.</span><span class="sxs-lookup"><span data-stu-id="e6097-170">Click Financials.</span></span>
2. <span data-ttu-id="e6097-171">Spustelėkite „Paskirstyti sumas“.</span><span class="sxs-lookup"><span data-stu-id="e6097-171">Click Distribute amounts.</span></span>
    * <span data-ttu-id="e6097-172">Šis procesas nurodo, kaip paskirstyti pirmos eilutės išlaidas 2 sąskaitoms.</span><span class="sxs-lookup"><span data-stu-id="e6097-172">This process shows you how to distribute the cost for the first line between 2 accounts.</span></span> <span data-ttu-id="e6097-173">Tą taip pat galima atlikti vėliau, kai paraiška bus peržiūrima.</span><span class="sxs-lookup"><span data-stu-id="e6097-173">This can also be done later when the requisition is in review.</span></span>  
3. <span data-ttu-id="e6097-174">Spustelėkite „Skaidyti“, kad sukurtumėte naują paskirstymo eilutę.</span><span class="sxs-lookup"><span data-stu-id="e6097-174">Click Split to create a new distribution line.</span></span>
4. <span data-ttu-id="e6097-175">Lauke „DK sąskaita“ pasirinkite pirmą išlaidų centrą, kuris turėtų prisiimti dalį išlaidų.</span><span class="sxs-lookup"><span data-stu-id="e6097-175">In the Ledger account field select the first cost centre that should take part of the cost.</span></span>
5. <span data-ttu-id="e6097-176">Pasirinkite kitą paskirstymo eilutę.</span><span class="sxs-lookup"><span data-stu-id="e6097-176">Select the other distribution line.</span></span>
6. <span data-ttu-id="e6097-177">Lauke „DK sąskaita“ nurodykite kitą išlaidų centrą.</span><span class="sxs-lookup"><span data-stu-id="e6097-177">In the Ledger account field specify the other cost centre.</span></span>
7. <span data-ttu-id="e6097-178">Spustelėkite „Paskirstyti tolygiai“.</span><span class="sxs-lookup"><span data-stu-id="e6097-178">Click Distribute equally.</span></span>
8. <span data-ttu-id="e6097-179">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="e6097-179">Close the page.</span></span>

## <a name="view-line-details"></a><span data-ttu-id="e6097-180">Peržiūrėti eilutės informaciją</span><span class="sxs-lookup"><span data-stu-id="e6097-180">View line details</span></span>
1. <span data-ttu-id="e6097-181">Perjunkite dalies Išsami eilučių informacija išplėtimą.</span><span class="sxs-lookup"><span data-stu-id="e6097-181">Toggle the expansion of the Line details section.</span></span>

## <a name="submit-the-requisition"></a><span data-ttu-id="e6097-182">Pateikti paraišką</span><span class="sxs-lookup"><span data-stu-id="e6097-182">Submit the requisition</span></span>
1. <span data-ttu-id="e6097-183">Spustelėkite „Darbo eiga“, kad atidarytumėte išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="e6097-183">Click Workflow to open the drop dialog.</span></span>
2. <span data-ttu-id="e6097-184">Spustelėkite Pateikti.</span><span class="sxs-lookup"><span data-stu-id="e6097-184">Click Submit.</span></span>
3. <span data-ttu-id="e6097-185">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="e6097-185">Close the page.</span></span>
4. <span data-ttu-id="e6097-186">Lauke „Komentaras“ įveskite pastabą paraiškos tvirtintojui.</span><span class="sxs-lookup"><span data-stu-id="e6097-186">In the Comment field, type a note for the approver of the requisition.</span></span>
5. <span data-ttu-id="e6097-187">Spustelėkite Pateikti.</span><span class="sxs-lookup"><span data-stu-id="e6097-187">Click Submit.</span></span>
6. <span data-ttu-id="e6097-188">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="e6097-188">Close the page.</span></span>
7. <span data-ttu-id="e6097-189">Atnaujinkite puslapį.</span><span class="sxs-lookup"><span data-stu-id="e6097-189">Refresh the page.</span></span>

