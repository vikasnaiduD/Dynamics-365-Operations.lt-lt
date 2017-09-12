--- 
title: "Formato modifikavimas iš naujo pritaikant „Microsoft Excel‟ šabloną elektroninėse ataskaitose (ER)"
description: "Norėdami užbaigti veiksmus šioje procedūroje, pirmiausia turite užbaigti procedūrą „ER – kurkite konfigūraciją ataskaitoms generuoti OPENXML formatu“."
author: NickSelin
manager: AnnBe
ms.date: 06/19/2017
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
ms.openlocfilehash: ae1de653354d891e99fb41fa4b10e6910f458cf4
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="modify-a-format-by-reapplying-a-microsoft-excel-template-for-electronic-reporting-er"></a><span data-ttu-id="0869e-103">Formato modifikavimas iš naujo pritaikant „Microsoft Excel‟ šabloną elektroninėse ataskaitose (ER)</span><span class="sxs-lookup"><span data-stu-id="0869e-103">Modify a format by reapplying a Microsoft Excel template for electronic reporting (ER)</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="0869e-104">Norėdami užbaigti veiksmus šioje procedūroje, pirmiausia turite užbaigti procedūrą „ER – kurkite konfigūraciją ataskaitoms generuoti OPENXML formatu“.</span><span class="sxs-lookup"><span data-stu-id="0869e-104">To complete the steps in this procedure, you must first complete the procedure, ER - Design a configuration for generating reports in OPENXML format.</span></span>

<span data-ttu-id="0869e-105">Šia procedūra paaiškinama, kaip keisti elektroninių ataskaitų teikimo (ER) formato konfigūraciją, iš naujo taikant „Microsoft Excel“ šabloną, kuris buvo pakeistas.</span><span class="sxs-lookup"><span data-stu-id="0869e-105">This procedure explains how to modify an Electronic reporting (ER) format configuration by reapplying a Microsoft Excel template that has been modified.</span></span> <span data-ttu-id="0869e-106">Šios procedūros metu importuosite modifikuotą „Excel“ šabloną į ER formato konfigūracijas, sukurtas pavyzdinei įmonei „Litware, Inc.“, ir tada generuokite elektroninius dokumentus.</span><span class="sxs-lookup"><span data-stu-id="0869e-106">In this procedure, you will import a modified Excel template into ER format configurations that have been created for the sample company, Litware, Inc., and then generate electronic documents.</span></span> <span data-ttu-id="0869e-107">Ši procedūra skirta vartotojams, kuriems priskirtas sistemos administratoriaus arba elektroninių ataskaitų teikimo programuotojo vaidmuo.</span><span class="sxs-lookup"><span data-stu-id="0869e-107">This procedure is intended for users who have the system administrator or electronic reporting developer role.</span></span> <span data-ttu-id="0869e-108">Šiuos veiksmus galima atlikti naudojant GBSI duomenų rinkinį.</span><span class="sxs-lookup"><span data-stu-id="0869e-108">These steps can be completed by using the GBSI dataset.</span></span> <span data-ttu-id="0869e-109">Prieš pradėdami atsisiųskite ir įrašykite failą SampleVendPaymWsReport2.xlsx, kuris nurodytas žinyno temoje „Keiskite elektroninių ataskaitų pateikimo formatą, iš naujo taikydami „Excel“ šabloną“ (https://docs.microsoft.com/en-us/dynamics365/unified-operations/dev-itpro/analytics/modify-electronic-reporting-format-reapply-excel-template/).</span><span class="sxs-lookup"><span data-stu-id="0869e-109">Before you begin, download and save the file, SampleVendPaymWsReport2.xlsx, which is listed in the Help topic, Modify Electronic reporting format by reapplying an Excel template (https://docs.microsoft.com/en-us/dynamics365/unified-operations/dev-itpro/analytics/modify-electronic-reporting-format-reapply-excel-template/).</span></span>

1. <span data-ttu-id="0869e-110">Pasirinkite Organizacijos administravimas > Darbo sritys > Elektroninės ataskaitos.</span><span class="sxs-lookup"><span data-stu-id="0869e-110">Go to Organization administration > Workspaces > Electronic reporting.</span></span>
    * <span data-ttu-id="0869e-111">Įsitikinkite, kad pavyzdinės įmonės „Litware, Inc.” konfigūracijos teikėjas yra prieinamas ir pažymėtas kaip aktyvus.</span><span class="sxs-lookup"><span data-stu-id="0869e-111">Make sure that the configuration provider for the sample company, Litware, Inc., is available and marked as Active.</span></span> <span data-ttu-id="0869e-112">Jei nematote šio konfigūracijos teikėjo, atlikite procedūros „Kurkite konfigūracijos teikėją ir pažymėkite kaip aktyvų” veiksmus.</span><span class="sxs-lookup"><span data-stu-id="0869e-112">If you don’t see this configuration provider, complete the steps in the procedure, Create a configuration provider and mark it as active.</span></span>  

## <a name="select-the-er-format"></a><span data-ttu-id="0869e-113">Pasirinkite ER formatą</span><span class="sxs-lookup"><span data-stu-id="0869e-113">Select the ER format</span></span>
1. <span data-ttu-id="0869e-114">Spustelėkite Ataskaitų konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="0869e-114">Click Reporting configurations.</span></span>
2. <span data-ttu-id="0869e-115">Medyje išplėskite „Mokėjimo modelis‟.</span><span class="sxs-lookup"><span data-stu-id="0869e-115">In the tree, expand 'Payment model'.</span></span>
3. <span data-ttu-id="0869e-116">Medyje pasirinkite Mokėjimo modelis\Darbalapio ataskaitos pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="0869e-116">In the tree, select 'Payment model\Sample worksheet report'.</span></span>
4. <span data-ttu-id="0869e-117">Spustelėkite Priedai.</span><span class="sxs-lookup"><span data-stu-id="0869e-117">Click Attachments.</span></span>
    * <span data-ttu-id="0869e-118">Atkreipkite dėmesį, kad SampleVendPaymWsReport.xlsx „Excel“ failas šiuo metu naudojamas kaip šablonas mokėjimo žurnalo apdorojimui.</span><span class="sxs-lookup"><span data-stu-id="0869e-118">Note that the SampleVendPaymWsReport.xlsx Excel file is currently used as a template for payment journal processing.</span></span>   
5. <span data-ttu-id="0869e-119">Spustelėkite Atidaryti.</span><span class="sxs-lookup"><span data-stu-id="0869e-119">Click Open.</span></span>
    * <span data-ttu-id="0869e-120">Spustelėkite Atidaryti, kad ištirtumėte „Excel“ šablono išdėstymą.</span><span class="sxs-lookup"><span data-stu-id="0869e-120">Click Open to explore the layout of the Excel template.</span></span>  
    * <span data-ttu-id="0869e-121">Peržiūrėkite šabloną.</span><span class="sxs-lookup"><span data-stu-id="0869e-121">Review the template.</span></span> <span data-ttu-id="0869e-122">Žinokite, kad į ją dabar įeina šie kiekvienos mokėjimo eilutės duomenys: tiekėjo sąskaitos numeris, tiekėjo pavadinimas, bankas, kodas, sąskaitos numeris, debetas, kreditas ir valiuta.</span><span class="sxs-lookup"><span data-stu-id="0869e-122">Note that it currently includes the following details for each payment line: vendor account number, vendor name, bank, routing number, account number, debit, credit, and currency.</span></span> <span data-ttu-id="0869e-123">Šiam pavyzdžiui mes norime pratęsti šį sąrašą, pridėdami informacijos apie mokėjimo datą.</span><span class="sxs-lookup"><span data-stu-id="0869e-123">For this example, we want to extend this list by adding details about the payment date.</span></span>   
6. <span data-ttu-id="0869e-124">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="0869e-124">Close the page.</span></span>

## <a name="reapply-a-new-excel-template-to-er-format"></a><span data-ttu-id="0869e-125">Iš naujo taikykite naują „Excel“ šabloną į ER formatui</span><span class="sxs-lookup"><span data-stu-id="0869e-125">Reapply a new Excel template to ER format</span></span>
1. <span data-ttu-id="0869e-126">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="0869e-126">Click Designer.</span></span>
    * <span data-ttu-id="0869e-127">Atidarykite pasirinkto ER formato juodraščio versiją redagavimui.</span><span class="sxs-lookup"><span data-stu-id="0869e-127">Open the draft version of the selected ER format for editing.</span></span>  
2. <span data-ttu-id="0869e-128">Veiksmų srityje spustelėkite Importuoti.</span><span class="sxs-lookup"><span data-stu-id="0869e-128">On the Action Pane, click Import.</span></span>
3. <span data-ttu-id="0869e-129">Spustelėkite Naujinti iš „Excel‟.</span><span class="sxs-lookup"><span data-stu-id="0869e-129">Click Update from Excel.</span></span>
    * <span data-ttu-id="0869e-130">Spustelėkite „Atnaujinti šabloną“ ir pasirinkite failą, SampleVendPaymWsReport2.xlsx.</span><span class="sxs-lookup"><span data-stu-id="0869e-130">Click ‘Update template’, and then select the file, SampleVendPaymWsReport2.xlsx.</span></span>  
    * <span data-ttu-id="0869e-131">Spustelėkite Atnaujinti šabloną ir naršykite, kad gautumėte anksčiau atsisiųstą SampleVendPaymWsReport2.xlsx failą.</span><span class="sxs-lookup"><span data-stu-id="0869e-131">Click Update template and browse to get the downloaded earlier SampleVendPaymWsReport2.xlsx file.</span></span>  
4. <span data-ttu-id="0869e-132">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="0869e-132">Click OK.</span></span>
    * <span data-ttu-id="0869e-133">Pritaikytas SampleVendPaymWsReport2.xlsx šablonas.</span><span class="sxs-lookup"><span data-stu-id="0869e-133">The SampleVendPaymWsReport2.xlsx template is applied.</span></span> <span data-ttu-id="0869e-134">ER formato struktūra sinchronizuojama su šablono, kurio elementai pridėti prie ER formato, turiniu.</span><span class="sxs-lookup"><span data-stu-id="0869e-134">The structure of the ER format is synchronized with the content of the template, whose elements are added to the ER format.</span></span> <span data-ttu-id="0869e-135">Bet kokie ER formate esantys elementai, kurie neįtraukiami į šabloną, pašalinami iš formato apibrėžties.</span><span class="sxs-lookup"><span data-stu-id="0869e-135">Any existing elements in the ER format that aren’t included in the template are removed from the format definition.</span></span>  
5. <span data-ttu-id="0869e-136">Medyje pasirinkite „Excel“.</span><span class="sxs-lookup"><span data-stu-id="0869e-136">In the tree, select 'Excel'.</span></span>
    * <span data-ttu-id="0869e-137">Atkreipkite dėmesį, kad šablono lauke dabar yra nuoroda į naują šabloną.</span><span class="sxs-lookup"><span data-stu-id="0869e-137">Note that the Template field now contains a reference to the new template.</span></span>   
6. <span data-ttu-id="0869e-138">Spustelėkite Priedai.</span><span class="sxs-lookup"><span data-stu-id="0869e-138">Click Attachments.</span></span>
7. <span data-ttu-id="0869e-139">Spustelėkite Atidaryti.</span><span class="sxs-lookup"><span data-stu-id="0869e-139">Click Open.</span></span>
    * <span data-ttu-id="0869e-140">Spustelėkite Atidaryti, kad ištirtumėte pakeisto „Excel“ šablono išdėstymą.</span><span class="sxs-lookup"><span data-stu-id="0869e-140">Click Open to explore the layout of the modified Excel template.</span></span>  
    * <span data-ttu-id="0869e-141">Peržiūrėkite šabloną.</span><span class="sxs-lookup"><span data-stu-id="0869e-141">Review the template.</span></span> <span data-ttu-id="0869e-142">Atkreipkite dėmesį, kad jame dabar yra eilutė mokėjimo datai.</span><span class="sxs-lookup"><span data-stu-id="0869e-142">Note that it now contains a line for the payment date.</span></span>   
8. <span data-ttu-id="0869e-143">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="0869e-143">Close the page.</span></span>
9. <span data-ttu-id="0869e-144">Medyje išplėskite „Excel“.</span><span class="sxs-lookup"><span data-stu-id="0869e-144">In the tree, expand 'Excel'.</span></span>
10. <span data-ttu-id="0869e-145">Medyje išplėskite „Excel \ PaymLines”.</span><span class="sxs-lookup"><span data-stu-id="0869e-145">In the tree, expand 'Excel\PaymLines'.</span></span>
11. <span data-ttu-id="0869e-146">Medyje pasirinkite „Excel\PaymLines\PaymDate“.</span><span class="sxs-lookup"><span data-stu-id="0869e-146">In the tree, select 'Excel\PaymLines\PaymDate'.</span></span>
    * <span data-ttu-id="0869e-147">Atkreipkite dėmesį, kad ER formate dabar yra dar vienas elementas.</span><span class="sxs-lookup"><span data-stu-id="0869e-147">Note that the ER format now contains one more item.</span></span> <span data-ttu-id="0869e-148">Langelis PaymDate pridėtas prie „Excel“ šablono.</span><span class="sxs-lookup"><span data-stu-id="0869e-148">A cell, PaymDate, has been added to the Excel template.</span></span>  
12. <span data-ttu-id="0869e-149">Spustelėkite skirtuką „Susiejimas“.</span><span class="sxs-lookup"><span data-stu-id="0869e-149">Click the Mapping tab.</span></span>
13. <span data-ttu-id="0869e-150">Medyje išplėskite „modelis‟.</span><span class="sxs-lookup"><span data-stu-id="0869e-150">In the tree, expand 'model'.</span></span>
14. <span data-ttu-id="0869e-151">Medyje išplėskite „modelis \ Mokėjimai‟.</span><span class="sxs-lookup"><span data-stu-id="0869e-151">In the tree, expand 'model\Payments'.</span></span>
15. <span data-ttu-id="0869e-152">Medyje pasirinkite „modelis \ Mokėjimai \ Operacijos data (TransactionDate)“.</span><span class="sxs-lookup"><span data-stu-id="0869e-152">In the tree, select 'model\Payments\Transaction date(TransactionDate)'.</span></span>
16. <span data-ttu-id="0869e-153">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="0869e-153">Click Bind.</span></span>
    * <span data-ttu-id="0869e-154">Nurodykite, kokie duomenys pridedami prie naujo langelio veikiant.</span><span class="sxs-lookup"><span data-stu-id="0869e-154">Specify what data is added to the new cell at runtime.</span></span>  
17. <span data-ttu-id="0869e-155">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="0869e-155">Click Save.</span></span>
18. <span data-ttu-id="0869e-156">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="0869e-156">Close the page.</span></span>

## <a name="enable-the-modified-draft-version-of-the-er-format-for-use-in-payment-journal-processing"></a><span data-ttu-id="0869e-157">Įgalinkite pakeistą ER formato juodraščio versiją naudoti mokėjimų žurnalo apdorojimui</span><span class="sxs-lookup"><span data-stu-id="0869e-157">Enable the modified draft version of the ER format for use in payment journal processing</span></span>
1. <span data-ttu-id="0869e-158">Veiksmų srityje spustelėkite Konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="0869e-158">On the Action Pane, click Configurations.</span></span>
2. <span data-ttu-id="0869e-159">Spustelėkite Vartotojo parametrai.</span><span class="sxs-lookup"><span data-stu-id="0869e-159">Click User parameters.</span></span>
3. <span data-ttu-id="0869e-160">Lauke Paleisti parametrus pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="0869e-160">Select Yes in the Run settings field.</span></span>
4. <span data-ttu-id="0869e-161">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="0869e-161">Click OK.</span></span>
5. <span data-ttu-id="0869e-162">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="0869e-162">Click Edit.</span></span>
6. <span data-ttu-id="0869e-163">Lauke Paleisti juodraštį pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="0869e-163">Select Yes in the Run Draft field.</span></span>

## <a name="use-the-modified-draft-version-of-the-er-format-for-payment-journal-processing"></a><span data-ttu-id="0869e-164">Naudokite pakeistą ER formato juodraščio versiją naudoti mokėjimų žurnalo apdorojimui</span><span class="sxs-lookup"><span data-stu-id="0869e-164">Use the modified draft version of the ER format for payment journal processing</span></span>
    * <span data-ttu-id="0869e-165">Peržiūrėkite sukurtą darbalapį, įskaitant naują mokėjimo eilučių informaciją – mokėjimo data.</span><span class="sxs-lookup"><span data-stu-id="0869e-165">Review the created worksheet, including new detail of payment lines – payment date.</span></span>  

