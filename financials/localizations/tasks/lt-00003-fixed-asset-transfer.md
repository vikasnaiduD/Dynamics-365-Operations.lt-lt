--- 
title: "Generuoti ilgalaikio turto perkėlimo iš vieno sandėlio į kitą dokumentą (Lietuva)"
description: "Jei jūsų organizacijai reikia perkelti ilgalaikį turtą iš vieno padalinio į kitą ir du padaliniai nėra toje pačioje vietoje, perkėlimas turi būti patvirtintas važtaraščiu."
author: KimANelson
manager: AnnBe
ms.date: 02/17/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Lithuania
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: aa2214a9ca9517913cdb1034646b6f39f8fb0d92
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="generate-a-fixed-asset-transfer-between-warehouses-document-lithuania"></a><span data-ttu-id="28ad9-103">Generuoti ilgalaikio turto perkėlimo iš vieno sandėlio į kitą dokumentą (Lietuva)</span><span class="sxs-lookup"><span data-stu-id="28ad9-103">Generate a fixed asset transfer between warehouses document (Lithuania)</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="28ad9-104">Jei jūsų organizacijai reikia perkelti ilgalaikį turtą iš vieno padalinio į kitą ir du padaliniai nėra toje pačioje vietoje, perkėlimas turi būti patvirtintas važtaraščiu.</span><span class="sxs-lookup"><span data-stu-id="28ad9-104">If your organization needs to move a fixed asset from one department to another and the two departments are not in the same location, the transfer must be verified by a packing slip.</span></span> <span data-ttu-id="28ad9-105">Taip pat reikia generuoti perkėlimo važtaraštį pakeitus darbuotoją, atsakingą už ilgalaikio turto perdavimą.</span><span class="sxs-lookup"><span data-stu-id="28ad9-105">You also need to generate a transfer packing slip if the employee responsible for the fixed asset is changed.</span></span> <span data-ttu-id="28ad9-106">Priklausomai nuo įgalintų parametrų, važtaraštis gali būti numeruojamas automatiškai arba neautomatiniu būdu.</span><span class="sxs-lookup"><span data-stu-id="28ad9-106">Depending on the parameters that are enabled, the packing slip can be numbered automatically or manually.</span></span>

<span data-ttu-id="28ad9-107">Ši procedūra taikoma tik Lietuvai skirtoms funkcijoms.</span><span class="sxs-lookup"><span data-stu-id="28ad9-107">This procedure applies only for Lithuanian functionality.</span></span> 

<span data-ttu-id="28ad9-108">Procedūra buvo sukurta naudojant demonstracinių duomenų įmonę USMF, todėl prieš pradedant reikia rankiniu būdu pakeisti USMF juridinio subjekto pirminį adresą į LTU.</span><span class="sxs-lookup"><span data-stu-id="28ad9-108">The procedure was created using the demo data company USMF and requires changing USMF legal entity primary address to LTU manually before starting.</span></span> 

<span data-ttu-id="28ad9-109">Ši procedūra skirta už ilgalaikį turtą atsakingiems buhalteriams.</span><span class="sxs-lookup"><span data-stu-id="28ad9-109">This procedure is intended for accountants who are responsible for fixed assets.</span></span>


## <a name="preset-vehicle-models"></a><span data-ttu-id="28ad9-110">Iš naujo nustatyti transporto priemonių modelius</span><span class="sxs-lookup"><span data-stu-id="28ad9-110">Preset vehicle models</span></span>
1. <span data-ttu-id="28ad9-111">Eikite į Organizacijos administravimas > Nustatymas > Transporto priemonė > Transporto priemonių modeliai.</span><span class="sxs-lookup"><span data-stu-id="28ad9-111">Go to Organization administration > Setup > Vehicle > Vehicle models.</span></span>
2. <span data-ttu-id="28ad9-112">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="28ad9-112">Click New.</span></span>
3. <span data-ttu-id="28ad9-113">Lauke Modelis įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-113">In the Model field, type a value.</span></span>
    * <span data-ttu-id="28ad9-114">Ši vertė bus spausdinama važtaraštyje.</span><span class="sxs-lookup"><span data-stu-id="28ad9-114">This value will be printed on the packing slip.</span></span>  
4. <span data-ttu-id="28ad9-115">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-115">In the Description field, type a value.</span></span>
5. <span data-ttu-id="28ad9-116">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-116">Click Save.</span></span>

## <a name="set-up-packing-slip-auto-numbering"></a><span data-ttu-id="28ad9-117">Nustatyti automatinį važtaraščio numeravimą</span><span class="sxs-lookup"><span data-stu-id="28ad9-117">Set up packing slip auto-numbering</span></span>
1. <span data-ttu-id="28ad9-118">Eikite į Organizacijos administravimas > Numeracijos > Skaitiklių valdymas.</span><span class="sxs-lookup"><span data-stu-id="28ad9-118">Go to Organization administration > Number sequences > Counters management.</span></span>
2. <span data-ttu-id="28ad9-119">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-119">Click Edit.</span></span>
3. <span data-ttu-id="28ad9-120">Lauke Modulis pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="28ad9-120">In the Module field, select an option.</span></span>
4. <span data-ttu-id="28ad9-121">Lauke Sąskaitos kodas pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="28ad9-121">In the Account code field, select an option.</span></span>
5. <span data-ttu-id="28ad9-122">Pažymėkite žymės langelį Automatinis numeravimas.</span><span class="sxs-lookup"><span data-stu-id="28ad9-122">Select the Auto numbering check box.</span></span>
6. <span data-ttu-id="28ad9-123">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-123">Click Save.</span></span>
7. <span data-ttu-id="28ad9-124">Eikite į Organizacijos administravimas > Numeracijos > SF numeravimo nustatymas.</span><span class="sxs-lookup"><span data-stu-id="28ad9-124">Go to Organization administration > Number sequences > Invoice numbering setup.</span></span>
8. <span data-ttu-id="28ad9-125">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-125">Click Edit.</span></span>
9. <span data-ttu-id="28ad9-126">Lauke Numeravimas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-126">In the Numbering field, type a value.</span></span>
10. <span data-ttu-id="28ad9-127">Lauke Modulis pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="28ad9-127">In the Module field, select an option.</span></span>
11. <span data-ttu-id="28ad9-128">Lauke Numeracijos kodas įveskite arba pasirinkite vertę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-128">In the Number sequence code field, enter or select a value.</span></span>
    * <span data-ttu-id="28ad9-129">Čia pasirinkta numeracija turi būti naudojama automatiniam važtaraščio numeravimui.</span><span class="sxs-lookup"><span data-stu-id="28ad9-129">The number sequence selected here should be used for packing slip auto-numbering.</span></span>  
12. <span data-ttu-id="28ad9-130">Lauke Sąskaitos kodas pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="28ad9-130">In the Account code field, select an option.</span></span>
13. <span data-ttu-id="28ad9-131">Pažymėkite žymės langelį Tęsti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-131">Select the Continue check box.</span></span>
14. <span data-ttu-id="28ad9-132">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-132">Click Save.</span></span>

## <a name="generate-packing-slip"></a><span data-ttu-id="28ad9-133">Generuoti važtaraštį</span><span class="sxs-lookup"><span data-stu-id="28ad9-133">Generate packing slip</span></span>

## <a name="specify-transportation-details"></a><span data-ttu-id="28ad9-134">Nurodyti transportavimo informaciją</span><span class="sxs-lookup"><span data-stu-id="28ad9-134">Specify transportation details</span></span>
1. <span data-ttu-id="28ad9-135">Eikite į Ilgalaikis turtas > Užklausos ir ataskaitos > Važtaraščiai.</span><span class="sxs-lookup"><span data-stu-id="28ad9-135">Go to Fixed assets > Inquiries and reports > Packing slips.</span></span>
2. <span data-ttu-id="28ad9-136">Veiksmų srityje spustelėkite Bendra.</span><span class="sxs-lookup"><span data-stu-id="28ad9-136">On the Action Pane, click General.</span></span>
3. <span data-ttu-id="28ad9-137">Spustelėkite Transportavimo informacija.</span><span class="sxs-lookup"><span data-stu-id="28ad9-137">Click Transportation details.</span></span>
4. <span data-ttu-id="28ad9-138">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-138">Click Edit.</span></span>
5. <span data-ttu-id="28ad9-139">Lauke Spausdinti transportavimo informaciją pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="28ad9-139">Select Yes in the Print transportation details field.</span></span>
    * <span data-ttu-id="28ad9-140">Jei pasirinkta, transportavimo informacija, kurią galite nurodyti šioje formoje, bus spausdinama važtaraštyje.</span><span class="sxs-lookup"><span data-stu-id="28ad9-140">If selected, transportation details that you can specify on this form will be printed on the Packing slip.</span></span>  
6. <span data-ttu-id="28ad9-141">Lauke Išduotos prekės įveskite arba pasirinkite vertę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-141">In the Goods issued by field, enter or select a value.</span></span>
7. <span data-ttu-id="28ad9-142">Lauke Paketas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-142">In the Package field, type a value.</span></span>
8. <span data-ttu-id="28ad9-143">Lauke Vežėjo tipas pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="28ad9-143">In the Carrier type field, select an option.</span></span>
9. <span data-ttu-id="28ad9-144">Lauke Vežėjas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-144">In the Carrier field, enter or select a value.</span></span>
10. <span data-ttu-id="28ad9-145">Lauke Modelis įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-145">In the Model field, enter or select a value.</span></span>
11. <span data-ttu-id="28ad9-146">Lauke Registracijos numeris įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-146">In the Registration number field, type a value.</span></span>
12. <span data-ttu-id="28ad9-147">Lauke Priekabos registracijos numeris įveskite vertę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-147">In the Trailer registration number field, type a value.</span></span>
13. <span data-ttu-id="28ad9-148">Lauke Vairuotojas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-148">In the Driver field, enter or select a value.</span></span>
14. <span data-ttu-id="28ad9-149">Lauke Vairuotojo vardas ir pavardė įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-149">In the Driver name field, type a value.</span></span>
15. <span data-ttu-id="28ad9-150">Lauke Pakrovimo data ir laikas įveskite datą ir laiką.</span><span class="sxs-lookup"><span data-stu-id="28ad9-150">In the Loading date and time field, enter a date and time.</span></span>
16. <span data-ttu-id="28ad9-151">Lauke Pakrovimo adresas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-151">In the Loading address field, enter or select a value.</span></span>
17. <span data-ttu-id="28ad9-152">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-152">Click Save.</span></span>
    * <span data-ttu-id="28ad9-153">Baigę turto iškrovimo procesą taip pat galite užpildyti važtaraščio iškrovimo informaciją.</span><span class="sxs-lookup"><span data-stu-id="28ad9-153">After the asset unloading process is completed, yo can also fill in unloading information for the packing slip.</span></span>  
18. <span data-ttu-id="28ad9-154">Lauke Iškrovimo data ir laikas įveskite datą ir laiką.</span><span class="sxs-lookup"><span data-stu-id="28ad9-154">In the Unloading date and time field, enter a date and time.</span></span>
19. <span data-ttu-id="28ad9-155">Lauke Iškrovimo adresas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="28ad9-155">In the Unloading address field, enter or select a value.</span></span>
20. <span data-ttu-id="28ad9-156">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="28ad9-156">Click Save.</span></span>
21. <span data-ttu-id="28ad9-157">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="28ad9-157">Close the page.</span></span>

## <a name="verify-the-packing-slip-report"></a><span data-ttu-id="28ad9-158">Patikrinti važtaraščio ataskaitą</span><span class="sxs-lookup"><span data-stu-id="28ad9-158">Verify the Packing slip report</span></span>
1. <span data-ttu-id="28ad9-159">Veiksmų srityje spustelėkite Bendra.</span><span class="sxs-lookup"><span data-stu-id="28ad9-159">On the Action Pane, click General.</span></span>
2. <span data-ttu-id="28ad9-160">Spustelėkite Ilgalaikio turto važtaraštis.</span><span class="sxs-lookup"><span data-stu-id="28ad9-160">Click Fixed asset packing slip.</span></span>
3. <span data-ttu-id="28ad9-161">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="28ad9-161">Click OK.</span></span>
    * <span data-ttu-id="28ad9-162">Sugeneravus ataskaitą bus spausdinama visa transportavimo informacija.</span><span class="sxs-lookup"><span data-stu-id="28ad9-162">After the report is generated, all transportation details will be printed.</span></span>  

