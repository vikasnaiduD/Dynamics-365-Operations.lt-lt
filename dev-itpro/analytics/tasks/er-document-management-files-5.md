--- 
title: "Formato modifikavimas ir vykdymas, kad dokumentų valdymo failai galėtų būti naudojami formato išvestyse elektroninėse ataskaitose (ER)"
description: "Toliau nurodytuose veiksmuose paaiškinta, kaip vartotojas, kuriam priskirtas sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmuo, gali konfigūruoti elektroninių ataskaitų (ER) formatą, norėdamas dokumentų valdymo failus (priedus) naudoti ER išvestyje."
author: NickSelin
manager: AnnBe
ms.date: 10/31/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 58e79f4d969e8bf0c7f150fd307f9f48334d6405
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="modify-and-run-format-to-use-document-management-files-in-format-outputs-for-electronic-reporting-er"></a><span data-ttu-id="b49e4-103">Formato modifikavimas ir vykdymas, kad dokumentų valdymo failai galėtų būti naudojami formato išvestyse elektroninėse ataskaitose (ER)</span><span class="sxs-lookup"><span data-stu-id="b49e4-103">Modify and run format to use Document Management files in format outputs for electronic reporting (ER)</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="b49e4-104">Toliau nurodytuose veiksmuose paaiškinta, kaip vartotojas, kuriam priskirtas sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmuo, gali konfigūruoti elektroninių ataskaitų (ER) formatą, norėdamas dokumentų valdymo failus (priedus) naudoti ER išvestyje.</span><span class="sxs-lookup"><span data-stu-id="b49e4-104">The following steps explain how a user assigned to the system administrator or electronic reporting developer role can configure an Electronic reporting (ER) format to use Document Management files (attachments) in ER output.</span></span> <span data-ttu-id="b49e4-105">Šiuos veiksmus galima atlikti DEMF įmonėje.</span><span class="sxs-lookup"><span data-stu-id="b49e4-105">These steps can be performed in the DEMF company.</span></span>

<span data-ttu-id="b49e4-106">Norėdami atlikti šiuos veiksmus, pirmiausia turite atlikti veiksmus, nurodytus procedūroje „ER: dokumentų valdymo failų naudojimas formato išvestyse (4 dalis): formato paleidimas“.</span><span class="sxs-lookup"><span data-stu-id="b49e4-106">To complete these steps, you must first complete the steps in the “ER Use Document Management files in format outputs (Part 4): Run format” procedure.</span></span>

<span data-ttu-id="b49e4-107">Ši procedūra yra skirta funkcijai, įtrauktai į „Dynamics 365 for Operations“ 1611 versiją.</span><span class="sxs-lookup"><span data-stu-id="b49e4-107">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>


## <a name="modify-the-format-to-populate-attachments-into-generating-messages-in-binary-format"></a><span data-ttu-id="b49e4-108">Keiskite formatą, jei norite priedus įvesti į generuojamus pranešimus dvejetainiu formatu</span><span class="sxs-lookup"><span data-stu-id="b49e4-108">Modify the format to populate attachments into generating messages in binary format</span></span>
1. <span data-ttu-id="b49e4-109">Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="b49e4-109">Go to Organization administration > Electronic reporting > Configurations.</span></span>
2. <span data-ttu-id="b49e4-110">Medyje išplėskite Kliento SF modelis.</span><span class="sxs-lookup"><span data-stu-id="b49e4-110">In the tree, expand 'Customer invoice model'.</span></span>
3. <span data-ttu-id="b49e4-111">Medyje išplėskite dalį Kliento SF modelis / kliento SF modelis (pasirinktinis).</span><span class="sxs-lookup"><span data-stu-id="b49e4-111">In the tree, expand 'Customer invoice model\Customer invoice model (custom)'.</span></span>
4. <span data-ttu-id="b49e4-112">Medyje pasirinkite Kliento SF modelis / kliento SF modelis (pasirinktinis) / elektroninės SF pranešimo pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="b49e4-112">In the tree, select 'Customer invoice model\Customer invoice model (custom)\Electronic invoice sample message'.</span></span>
5. <span data-ttu-id="b49e4-113">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="b49e4-113">Click Designer.</span></span>
    * <span data-ttu-id="b49e4-114">SF pranešimas bus automatiškai įvedamas generuojamoje išvestyje kaip XML failas naudojant UNICODE kodavimą.</span><span class="sxs-lookup"><span data-stu-id="b49e4-114">You will populate the invoice message in the generating output as an XML file using UNICODE encoding.</span></span>  
6. <span data-ttu-id="b49e4-115">Spustelėdami Įtraukti šakninį elementą atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="b49e4-115">Click Add root to open the drop dialog.</span></span>
7. <span data-ttu-id="b49e4-116">Medyje pasirinkite „Bendra \ Failas“.</span><span class="sxs-lookup"><span data-stu-id="b49e4-116">In the tree, select 'Common\File'.</span></span>
8. <span data-ttu-id="b49e4-117">Lauke Pavadinimas įveskite XML pranešimas.</span><span class="sxs-lookup"><span data-stu-id="b49e4-117">In the Name field, type 'Xml message'.</span></span>
    * <span data-ttu-id="b49e4-118">XML pranešimas</span><span class="sxs-lookup"><span data-stu-id="b49e4-118">Xml message</span></span>  
9. <span data-ttu-id="b49e4-119">Lauke „Kodavimas“ įveskite „UTF-8“.</span><span class="sxs-lookup"><span data-stu-id="b49e4-119">In the Encoding field, type 'UTF-8'.</span></span>
    * <span data-ttu-id="b49e4-120">UTF-8</span><span class="sxs-lookup"><span data-stu-id="b49e4-120">UTF-8</span></span>  
10. <span data-ttu-id="b49e4-121">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="b49e4-121">Click OK.</span></span>
    * <span data-ttu-id="b49e4-122">Sukonfigūruokite generuojamą išvestį kaip suglaudintą failą.</span><span class="sxs-lookup"><span data-stu-id="b49e4-122">Configure the generating output as a zipped file.</span></span>  
11. <span data-ttu-id="b49e4-123">Spustelėdami Įtraukti šakninį elementą atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="b49e4-123">Click Add root to open the drop dialog.</span></span>
12. <span data-ttu-id="b49e4-124">Medyje pasirinkite Bendra / aplankas.</span><span class="sxs-lookup"><span data-stu-id="b49e4-124">In the tree, select 'Common\Folder'.</span></span>
13. <span data-ttu-id="b49e4-125">Lauke Pavadinimas įveskite ZIP išvestis.</span><span class="sxs-lookup"><span data-stu-id="b49e4-125">In the Name field, type 'Zip output'.</span></span>
    * <span data-ttu-id="b49e4-126">ZIP išvestis</span><span class="sxs-lookup"><span data-stu-id="b49e4-126">Zip output</span></span>  
14. <span data-ttu-id="b49e4-127">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="b49e4-127">Click OK.</span></span>
15. <span data-ttu-id="b49e4-128">Medyje pasirinkite ZIP išvestis.</span><span class="sxs-lookup"><span data-stu-id="b49e4-128">In the tree, select 'Zip output'.</span></span>
    * <span data-ttu-id="b49e4-129">Pridėkite priedų prie generuojamo suglaudinto failo kaip failus su pradiniais pavadinimais ir plėtiniais.</span><span class="sxs-lookup"><span data-stu-id="b49e4-129">Add attachments to the generating zipped file as files with original names and extensions.</span></span>  
16. <span data-ttu-id="b49e4-130">Spustelėdami Įtraukti atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="b49e4-130">Click Add to open the drop dialog.</span></span>
17. <span data-ttu-id="b49e4-131">Medyje pasirinkite „Bendra \ Failas“.</span><span class="sxs-lookup"><span data-stu-id="b49e4-131">In the tree, select 'Common\File'.</span></span>
18. <span data-ttu-id="b49e4-132">Lauke Pavadinimas įveskite Pridėtas failas.</span><span class="sxs-lookup"><span data-stu-id="b49e4-132">In the Name field, type 'Attached file'.</span></span>
    * <span data-ttu-id="b49e4-133">Pridėtas failas</span><span class="sxs-lookup"><span data-stu-id="b49e4-133">Attached file</span></span>  
19. <span data-ttu-id="b49e4-134">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="b49e4-134">Click OK.</span></span>
20. <span data-ttu-id="b49e4-135">Medyje pasirinkite ZIP išvestis / pridėtas failas.</span><span class="sxs-lookup"><span data-stu-id="b49e4-135">In the tree, select 'Zip output\Attached file'.</span></span>
21. <span data-ttu-id="b49e4-136">Spustelėdami Įtraukti atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="b49e4-136">Click Add to open the drop dialog.</span></span>
22. <span data-ttu-id="b49e4-137">Medyje pasirinkite Text\Base64.</span><span class="sxs-lookup"><span data-stu-id="b49e4-137">In the tree, select 'Text\Base64'.</span></span>
23. <span data-ttu-id="b49e4-138">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="b49e4-138">Click OK.</span></span>

## <a name="map-new-format-elements-to-data-model"></a><span data-ttu-id="b49e4-139">Susiekite naujo formato elementus su duomenų modeliu</span><span class="sxs-lookup"><span data-stu-id="b49e4-139">Map new format elements to data model</span></span>
1. <span data-ttu-id="b49e4-140">Spustelėkite skirtuką „Susiejimas“.</span><span class="sxs-lookup"><span data-stu-id="b49e4-140">Click the Mapping tab.</span></span>
2. <span data-ttu-id="b49e4-141">Medyje išplėskite „modelis‟.</span><span class="sxs-lookup"><span data-stu-id="b49e4-141">In the tree, expand 'model'.</span></span>
3. <span data-ttu-id="b49e4-142">Medyje išplėskite model\Invoice attachments.</span><span class="sxs-lookup"><span data-stu-id="b49e4-142">In the tree, expand 'model\Invoice attachments'.</span></span>
4. <span data-ttu-id="b49e4-143">Medyje pasirinkite ZIP išvestis / pridėtas failas / Base64.</span><span class="sxs-lookup"><span data-stu-id="b49e4-143">In the tree, select 'Zip output\Attached file\Base64'.</span></span>
5. <span data-ttu-id="b49e4-144">Medyje pasirinkite model\Invoice attachments\File content.</span><span class="sxs-lookup"><span data-stu-id="b49e4-144">In the tree, select 'model\Invoice attachments\File content'.</span></span>
6. <span data-ttu-id="b49e4-145">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="b49e4-145">Click Bind.</span></span>
7. <span data-ttu-id="b49e4-146">Medyje pasirinkite ZIP išvestis / pridėtas failas.</span><span class="sxs-lookup"><span data-stu-id="b49e4-146">In the tree, select 'Zip output\Attached file'.</span></span>
8. <span data-ttu-id="b49e4-147">Spustelėkite Redaguoti failo vardą.</span><span class="sxs-lookup"><span data-stu-id="b49e4-147">Click Edit filename.</span></span>
9. <span data-ttu-id="b49e4-148">Medyje išplėskite „modelis‟.</span><span class="sxs-lookup"><span data-stu-id="b49e4-148">In the tree, expand 'model'.</span></span>
10. <span data-ttu-id="b49e4-149">Medyje išplėskite model\Invoice attachments.</span><span class="sxs-lookup"><span data-stu-id="b49e4-149">In the tree, expand 'model\Invoice attachments'.</span></span>
11. <span data-ttu-id="b49e4-150">Medyje pasirinkite model\Invoice attachments\File name.</span><span class="sxs-lookup"><span data-stu-id="b49e4-150">In the tree, select 'model\Invoice attachments\File name'.</span></span>
12. <span data-ttu-id="b49e4-151">Spustelėkite „Įtraukti duomenų šaltinį“.</span><span class="sxs-lookup"><span data-stu-id="b49e4-151">Click Add data source.</span></span>
13. <span data-ttu-id="b49e4-152">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="b49e4-152">Click Save.</span></span>
14. <span data-ttu-id="b49e4-153">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="b49e4-153">Close the page.</span></span>
15. <span data-ttu-id="b49e4-154">Medyje pasirinkite model\Invoice attachments.</span><span class="sxs-lookup"><span data-stu-id="b49e4-154">In the tree, select 'model\Invoice attachments'.</span></span>
16. <span data-ttu-id="b49e4-155">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="b49e4-155">Click Bind.</span></span>
17. <span data-ttu-id="b49e4-156">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="b49e4-156">Click Save.</span></span>
18. <span data-ttu-id="b49e4-157">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="b49e4-157">Close the page.</span></span>

## <a name="run-the-designed-report-for-the-selected-invoice"></a><span data-ttu-id="b49e4-158">Paleiskite sukurtą pasirinktos SF ataskaitą</span><span class="sxs-lookup"><span data-stu-id="b49e4-158">Run the designed report for the selected invoice</span></span>
1. <span data-ttu-id="b49e4-159">Spustelėkite Vykdyti.</span><span class="sxs-lookup"><span data-stu-id="b49e4-159">Click Run.</span></span>
2. <span data-ttu-id="b49e4-160">Išplėskite dalį Įtrauktini įrašai ().</span><span class="sxs-lookup"><span data-stu-id="b49e4-160">Expand the Records to include () section.</span></span>
3. <span data-ttu-id="b49e4-161">Spustelėkite Filtras.</span><span class="sxs-lookup"><span data-stu-id="b49e4-161">Click Filter.</span></span>
4. <span data-ttu-id="b49e4-162">Pasirinkite kliento SF žurnalo eilutę ir lauką Pardavimo užsakymas.</span><span class="sxs-lookup"><span data-stu-id="b49e4-162">Select the row of the Customer invoice journal and the Sales order field.</span></span>
5. <span data-ttu-id="b49e4-163">Lauko Kriterijai kriterijų lauke Pardavimo užsakymas įveskite užsakymo numerį 000148.</span><span class="sxs-lookup"><span data-stu-id="b49e4-163">In the Criteria field, In the criteria “Sales order” field, type the order number 000148.</span></span>
    * <span data-ttu-id="b49e4-164">000148</span><span class="sxs-lookup"><span data-stu-id="b49e4-164">000148</span></span>  
6. <span data-ttu-id="b49e4-165">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="b49e4-165">Click OK.</span></span>
7. <span data-ttu-id="b49e4-166">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="b49e4-166">Click OK.</span></span>
    * <span data-ttu-id="b49e4-167">Peržiūrėkite sugeneruotą išvestį.</span><span class="sxs-lookup"><span data-stu-id="b49e4-167">Review the generated output.</span></span> <span data-ttu-id="b49e4-168">Atkreipkite dėmesį, kad be SF pranešimo XML formatu sukuriamas vienas failas kiekvienam priedui.</span><span class="sxs-lookup"><span data-stu-id="b49e4-168">Note,that in addition to the invoice message in XML format, a single file has been created for each attachment.</span></span> <span data-ttu-id="b49e4-169">Priedų failai yra užpildomi įvedant suglaudintos išvesties duomenis dvejetainiu formatu.</span><span class="sxs-lookup"><span data-stu-id="b49e4-169">The attachment files are populated with the zipped output in binary format.</span></span>  

