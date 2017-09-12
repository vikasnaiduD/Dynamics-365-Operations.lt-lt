--- 
title: "Formato kūrimas, kad norint elektroninėse ataskaitose (ER) dinamiškai įtraukti stulpelius į „Excel“ ataskaitas būtų naudojami horizontaliai išplečiami diapazonai"
description: "Toliau nurodytuose veiksmuose paaiškinta, kaip vartotojas, kuriam priskirtas sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmuo, gali konfigūruoti elektroninių ataskaitų (ER) formatą, norėdamas ataskaitas generuoti kaip OPENXML darbalapių („Excel“) failus, kuriuose būtinus stulpelius galima dinamiškai kurti kaip horizontaliai išplečiamus diapazonus."
author: NickSelin
manager: AnnBe
ms.date: 10/28/2016
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
ms.openlocfilehash: fdba6a68cd98b0ccbc4072f5c1124088ed9d814b
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="design-a-format-to-use-horizontally-expandable-ranges-to-dynamically-add-columns-in-excel-reports-for-electronic-reporting-er"></a><span data-ttu-id="fc037-103">Formato kūrimas, kad norint elektroninėse ataskaitose (ER) dinamiškai įtraukti stulpelius į „Excel“ ataskaitas būtų naudojami horizontaliai išplečiami diapazonai</span><span class="sxs-lookup"><span data-stu-id="fc037-103">Design a format to use horizontally-expandable ranges to dynamically add columns in Excel reports for electronic reporting (ER)</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="fc037-104">Toliau nurodytuose veiksmuose paaiškinta, kaip vartotojas, kuriam priskirtas sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmuo, gali konfigūruoti elektroninių ataskaitų (ER) formatą, norėdamas ataskaitas generuoti kaip OPENXML darbalapių („Excel“) failus, kuriuose būtinus stulpelius galima dinamiškai kurti kaip horizontaliai išplečiamus diapazonus.</span><span class="sxs-lookup"><span data-stu-id="fc037-104">The following steps explain how a user assigned to the system administrator or electronic reporting developer role can configure an Electronic reporting (ER) format to generate reports as OPENXML worksheets (Excel) files in which the required columns can be created dynamically as horizontally expandable ranges.</span></span> <span data-ttu-id="fc037-105">Šiuos veiksmus galima atlikti bet kurioje įmonėje.</span><span class="sxs-lookup"><span data-stu-id="fc037-105">These steps can be performed in any company.</span></span>

<span data-ttu-id="fc037-106">Norėdami atlikti šiuos veiksmus, pirmiausia turite baigti šiuos tris užduočių vadovus:</span><span class="sxs-lookup"><span data-stu-id="fc037-106">To complete these steps, you must first complete these three task guides:</span></span> 

<span data-ttu-id="fc037-107">„ER sukurti konfigūracijų teikėją ir jį pažymėti kaip aktyvų“</span><span class="sxs-lookup"><span data-stu-id="fc037-107">“ER Create a configuration provider and mark it as active”</span></span>

<span data-ttu-id="fc037-108">„ER naudoti finansines dimensijas kaip duomenų šaltinį (1 dalis: duomenų modelio kūrimas)“</span><span class="sxs-lookup"><span data-stu-id="fc037-108">“ER Use financial dimensions as a data source (Part 1: Design data model)”</span></span>

<span data-ttu-id="fc037-109">„ER naudoti finansines dimensijas kaip duomenų šaltinį (2 dalis: modelio susiejimas)“</span><span class="sxs-lookup"><span data-stu-id="fc037-109">“ER Use financial dimensions as a data source (Part 2: Model mapping)”</span></span>

<span data-ttu-id="fc037-110">Taip pat turite atsisiųsti ir įrašyti vietinę šablono kopiją su ataskaitos pavyzdžiu, esančią čia: http://msdynamics.blob.core.windows.net/media/2016/09/SampleFinDimWsReport.xlsx</span><span class="sxs-lookup"><span data-stu-id="fc037-110">You must also download and save a local copy of the template with a sample report found here: http://msdynamics.blob.core.windows.net/media/2016/09/SampleFinDimWsReport.xlsx</span></span>

<span data-ttu-id="fc037-111">Ši procedūra yra skirta funkcijai, įtrauktai į „Dynamics 365 for Operations“ 1611 versiją.</span><span class="sxs-lookup"><span data-stu-id="fc037-111">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>


## <a name="create-a-new-report-configuration"></a><span data-ttu-id="fc037-112">Naujos ataskaitos konfigūracijos kūrimas</span><span class="sxs-lookup"><span data-stu-id="fc037-112">Create a new report configuration</span></span>
1. <span data-ttu-id="fc037-113">Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="fc037-113">Go to Organization administration > Electronic reporting > Configurations.</span></span>
2. <span data-ttu-id="fc037-114">Medyje pasirinkite Finansinių dimensijų modelio pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="fc037-114">In the tree, select 'Financial dimensions sample model'.</span></span>
3. <span data-ttu-id="fc037-115">Spustelėdami Kurti konfigūraciją, atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="fc037-115">Click Create configuration to open the drop dialog.</span></span>
4. <span data-ttu-id="fc037-116">Lauke Naujas įveskite Formatas, pagrįstas duomenų modeliu Finansinių dimensijų modelio pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="fc037-116">In the New field, enter 'Format based on data model Financial dimensions sample model'.</span></span>
    * <span data-ttu-id="fc037-117">Naudokite iš anksto sukurtą modelį kaip naujos ataskaitos duomenų šaltinį.</span><span class="sxs-lookup"><span data-stu-id="fc037-117">Use the model created in advance as the data source for your new report.</span></span>  
5. <span data-ttu-id="fc037-118">Lauke Pavadinimas įveskite Ataskaitos su horizontaliai išplečiamais diapazonais pavyzdys.</span><span class="sxs-lookup"><span data-stu-id="fc037-118">In the Name field, type 'Sample report with horizontally expandable ranges'.</span></span>
    * <span data-ttu-id="fc037-119">Ataskaitos su horizontaliai išplečiamais diapazonais pavyzdys</span><span class="sxs-lookup"><span data-stu-id="fc037-119">Sample report with horizontally expandable ranges</span></span>  
6. <span data-ttu-id="fc037-120">Lauke Aprašas įveskite „Excel“ išvesties su dinamiškai įtraukiamais stulpeliais kūrimas.</span><span class="sxs-lookup"><span data-stu-id="fc037-120">In the Description field, type 'To make Excel output with dynamically adding columns'.</span></span>
    * <span data-ttu-id="fc037-121">„Excel“ išvesties su dinamiškai įtraukiamais stulpeliais kūrimas</span><span class="sxs-lookup"><span data-stu-id="fc037-121">To make Excel output with dynamically adding columns</span></span>  
7. <span data-ttu-id="fc037-122">Lauke Duomenų modelio aprašas pasirinkite Įrašas.</span><span class="sxs-lookup"><span data-stu-id="fc037-122">In the Data model definition field, select Entry.</span></span>
8. <span data-ttu-id="fc037-123">Spustelėkite Sukurti konfigūraciją.</span><span class="sxs-lookup"><span data-stu-id="fc037-123">Click Create configuration.</span></span>

## <a name="design-the-report-format"></a><span data-ttu-id="fc037-124">Ataskaitos formato kūrimas</span><span class="sxs-lookup"><span data-stu-id="fc037-124">Design the report format</span></span>
1. <span data-ttu-id="fc037-125">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="fc037-125">Click Designer.</span></span>
2. <span data-ttu-id="fc037-126">Įjunkite perjungimo mygtuką Rodyti išsamią informaciją.</span><span class="sxs-lookup"><span data-stu-id="fc037-126">Turn on the ‘Show details’ toggle button.</span></span>
3. <span data-ttu-id="fc037-127">Veiksmų srityje spustelėkite Importuoti.</span><span class="sxs-lookup"><span data-stu-id="fc037-127">On the Action Pane, click Import.</span></span>
4. <span data-ttu-id="fc037-128">Spustelėkite Importuoti iš „Excel‟.</span><span class="sxs-lookup"><span data-stu-id="fc037-128">Click Import from Excel.</span></span>
5. <span data-ttu-id="fc037-129">Spustelėkite Priedai.</span><span class="sxs-lookup"><span data-stu-id="fc037-129">Click Attachments.</span></span>
    * <span data-ttu-id="fc037-130">Importuokite ataskaitos šabloną.</span><span class="sxs-lookup"><span data-stu-id="fc037-130">Import the report’s template.</span></span> <span data-ttu-id="fc037-131">Naudokite „Excel“ failą, kurį šiuo tikslu atsisiuntėte.</span><span class="sxs-lookup"><span data-stu-id="fc037-131">Use Excel file that you downloaded for that.</span></span>  
6. <span data-ttu-id="fc037-132">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="fc037-132">Click New.</span></span>
7. <span data-ttu-id="fc037-133">Spustelėkite Failas.</span><span class="sxs-lookup"><span data-stu-id="fc037-133">Click File.</span></span>
8. <span data-ttu-id="fc037-134">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="fc037-134">Close the page.</span></span>
9. <span data-ttu-id="fc037-135">Lauke Šablonas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="fc037-135">In the Template field, enter or select a value.</span></span>
    * <span data-ttu-id="fc037-136">Pasirinkite atsisiųstą šabloną.</span><span class="sxs-lookup"><span data-stu-id="fc037-136">Select the downloaded template.</span></span>  
10. <span data-ttu-id="fc037-137">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="fc037-137">Click OK.</span></span>
    * <span data-ttu-id="fc037-138">Įtraukite naują diapazoną, norėdami dinamiškai kurti „Excel“ išvestį su tiek finansinių dimensijų stulpelių, kiek pasirinkote (vartotojo dialogo formoje).</span><span class="sxs-lookup"><span data-stu-id="fc037-138">Add a new range to dynamically create Excel output with as many columns as you selected (in the user dialog form) for financial dimensions.</span></span> <span data-ttu-id="fc037-139">Kiekvienas kiekvieno stulpelio langelis nurodys vienos finansinės dimensijos pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="fc037-139">Each cell for every column will represent a single financial dimension’s name.</span></span>  
11. <span data-ttu-id="fc037-140">Spustelėdami Įtraukti atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="fc037-140">Click Add to open the drop dialog.</span></span>
12. <span data-ttu-id="fc037-141">Medyje pasirinkite Excel\Range.</span><span class="sxs-lookup"><span data-stu-id="fc037-141">In the tree, select 'Excel\Range'.</span></span>
13. <span data-ttu-id="fc037-142">Lauke „Excel“ diapazonas įveskite DimNames.</span><span class="sxs-lookup"><span data-stu-id="fc037-142">In the Excel range field, type 'DimNames'.</span></span>
    * <span data-ttu-id="fc037-143">DimNames</span><span class="sxs-lookup"><span data-stu-id="fc037-143">DimNames</span></span>  
14. <span data-ttu-id="fc037-144">Lauke Dubliavimo kryptis pasirinkite Horizontali.</span><span class="sxs-lookup"><span data-stu-id="fc037-144">In the Replication direction field, select 'Horizontal'.</span></span>
15. <span data-ttu-id="fc037-145">Spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="fc037-145">Click OK.</span></span>
16. <span data-ttu-id="fc037-146">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal.</span><span class="sxs-lookup"><span data-stu-id="fc037-146">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal'.</span></span>
17. <span data-ttu-id="fc037-147">Spustelėkite Perkelti aukštyn.</span><span class="sxs-lookup"><span data-stu-id="fc037-147">Click Move up.</span></span>
18. <span data-ttu-id="fc037-148">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Cell<DimNames>.</span><span class="sxs-lookup"><span data-stu-id="fc037-148">In the tree, select 'Excel = "SampleFinDimWsReport"\Cell<DimNames>'.</span></span>
19. <span data-ttu-id="fc037-149">Spustelėkite Iškirpti.</span><span class="sxs-lookup"><span data-stu-id="fc037-149">Click Cut.</span></span>
20. <span data-ttu-id="fc037-150">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal.</span><span class="sxs-lookup"><span data-stu-id="fc037-150">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal'.</span></span>
21. <span data-ttu-id="fc037-151">Spustelėkite Įklijuoti.</span><span class="sxs-lookup"><span data-stu-id="fc037-151">Click Paste.</span></span>
22. <span data-ttu-id="fc037-152">Medyje išplėskite Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal.</span><span class="sxs-lookup"><span data-stu-id="fc037-152">In the tree, expand 'Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal'.</span></span>
23. <span data-ttu-id="fc037-153">Medyje išplėskite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical.</span><span class="sxs-lookup"><span data-stu-id="fc037-153">In the tree, expand 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical'.</span></span>
24. <span data-ttu-id="fc037-154">Medyje išplėskite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical.</span><span class="sxs-lookup"><span data-stu-id="fc037-154">In the tree, expand 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical'.</span></span>
25. <span data-ttu-id="fc037-155">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical.</span><span class="sxs-lookup"><span data-stu-id="fc037-155">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical'.</span></span>
    * <span data-ttu-id="fc037-156">Įtraukite naują diapazoną, norėdami dinamiškai kurti „Excel“ išvestį su tiek finansinių dimensijų stulpelių, kiek pasirinkote (vartotojo dialogo formoje).</span><span class="sxs-lookup"><span data-stu-id="fc037-156">Add a new range to dynamically create Excel output with as many columns as you selected (in the user dialog form) for financial dimensions.</span></span> <span data-ttu-id="fc037-157">Kiekvienas kiekvieno stulpelio langelis nurodys vienos finansinės dimensijos reikšmę, skirtą kiekvienai ataskaitų operacijai.</span><span class="sxs-lookup"><span data-stu-id="fc037-157">Each cell for every column will represent a single financial dimension’s value for each reporting transaction.</span></span>  
26. <span data-ttu-id="fc037-158">Spustelėkite Įtraukti diapazoną.</span><span class="sxs-lookup"><span data-stu-id="fc037-158">Click Add Range.</span></span>
27. <span data-ttu-id="fc037-159">Lauke „Excel“ diapazonas įveskite DimValues.</span><span class="sxs-lookup"><span data-stu-id="fc037-159">In the Excel range field, type 'DimValues'.</span></span>
    * <span data-ttu-id="fc037-160">DimValues</span><span class="sxs-lookup"><span data-stu-id="fc037-160">DimValues</span></span>  
28. <span data-ttu-id="fc037-161">Lauke Dubliavimo kryptis pasirinkite Horizontali.</span><span class="sxs-lookup"><span data-stu-id="fc037-161">In the Replication direction field, select 'Horizontal'.</span></span>
29. <span data-ttu-id="fc037-162">Spustelėkite Gerai.</span><span class="sxs-lookup"><span data-stu-id="fc037-162">Click OK.</span></span>
30. <span data-ttu-id="fc037-163">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<DimValues>.</span><span class="sxs-lookup"><span data-stu-id="fc037-163">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<DimValues>'.</span></span>
31. <span data-ttu-id="fc037-164">Spustelėkite Iškirpti.</span><span class="sxs-lookup"><span data-stu-id="fc037-164">Click Cut.</span></span>
32. <span data-ttu-id="fc037-165">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal.</span><span class="sxs-lookup"><span data-stu-id="fc037-165">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal'.</span></span>
33. <span data-ttu-id="fc037-166">Spustelėkite Įklijuoti.</span><span class="sxs-lookup"><span data-stu-id="fc037-166">Click Paste.</span></span>
34. <span data-ttu-id="fc037-167">Medyje išplėskite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal.</span><span class="sxs-lookup"><span data-stu-id="fc037-167">In the tree, expand 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal'.</span></span>

## <a name="map-format-elements-to-data-sources"></a><span data-ttu-id="fc037-168">Formato elementų susiejimas su duomenų šaltiniais</span><span class="sxs-lookup"><span data-stu-id="fc037-168">Map format elements to data sources</span></span>
1. <span data-ttu-id="fc037-169">Spustelėkite skirtuką „Susiejimas“.</span><span class="sxs-lookup"><span data-stu-id="fc037-169">Click the Mapping tab.</span></span>
2. <span data-ttu-id="fc037-170">Medyje išplėskite dalį model: Data model Financial dimensions sample model.</span><span class="sxs-lookup"><span data-stu-id="fc037-170">In the tree, expand 'model: Data model Financial dimensions sample model'.</span></span>
3. <span data-ttu-id="fc037-171">Medyje išplėskite dalį model: Data model Financial dimensions sample model\Journal: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-171">In the tree, expand 'model: Data model Financial dimensions sample model\Journal: Record list'.</span></span>
4. <span data-ttu-id="fc037-172">Medyje išplėskite dalį model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-172">In the tree, expand 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list'.</span></span>
5. <span data-ttu-id="fc037-173">Medyje išplėskite dalį model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Dimensions data: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-173">In the tree, expand 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Dimensions data: Record list'.</span></span>
6. <span data-ttu-id="fc037-174">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal\Cell<DimValues>.</span><span class="sxs-lookup"><span data-stu-id="fc037-174">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal\Cell<DimValues>'.</span></span>
7. <span data-ttu-id="fc037-175">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Dimensions data: Record list\Code: String.</span><span class="sxs-lookup"><span data-stu-id="fc037-175">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Dimensions data: Record list\Code: String'.</span></span>
8. <span data-ttu-id="fc037-176">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-176">Click Bind.</span></span>
9. <span data-ttu-id="fc037-177">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal.</span><span class="sxs-lookup"><span data-stu-id="fc037-177">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Range<DimValues>: Horizontal'.</span></span>
10. <span data-ttu-id="fc037-178">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Dimensions data: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-178">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Dimensions data: Record list'.</span></span>
11. <span data-ttu-id="fc037-179">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-179">Click Bind.</span></span>
12. <span data-ttu-id="fc037-180">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<Credit>.</span><span class="sxs-lookup"><span data-stu-id="fc037-180">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<Credit>'.</span></span>
13. <span data-ttu-id="fc037-181">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Credit: Real.</span><span class="sxs-lookup"><span data-stu-id="fc037-181">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Credit: Real'.</span></span>
14. <span data-ttu-id="fc037-182">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-182">Click Bind.</span></span>
15. <span data-ttu-id="fc037-183">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<Debit>.</span><span class="sxs-lookup"><span data-stu-id="fc037-183">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<Debit>'.</span></span>
16. <span data-ttu-id="fc037-184">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Debit: Real.</span><span class="sxs-lookup"><span data-stu-id="fc037-184">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Debit: Real'.</span></span>
17. <span data-ttu-id="fc037-185">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-185">Click Bind.</span></span>
18. <span data-ttu-id="fc037-186">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<Currency>.</span><span class="sxs-lookup"><span data-stu-id="fc037-186">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<Currency>'.</span></span>
19. <span data-ttu-id="fc037-187">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Currency: String.</span><span class="sxs-lookup"><span data-stu-id="fc037-187">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Currency: String'.</span></span>
20. <span data-ttu-id="fc037-188">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-188">Click Bind.</span></span>
21. <span data-ttu-id="fc037-189">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<TransDate>.</span><span class="sxs-lookup"><span data-stu-id="fc037-189">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<TransDate>'.</span></span>
22. <span data-ttu-id="fc037-190">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Date: Date.</span><span class="sxs-lookup"><span data-stu-id="fc037-190">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Date: Date'.</span></span>
23. <span data-ttu-id="fc037-191">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-191">Click Bind.</span></span>
24. <span data-ttu-id="fc037-192">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<TransVoucher>.</span><span class="sxs-lookup"><span data-stu-id="fc037-192">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<TransVoucher>'.</span></span>
25. <span data-ttu-id="fc037-193">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Voucher: String.</span><span class="sxs-lookup"><span data-stu-id="fc037-193">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list\Voucher: String'.</span></span>
26. <span data-ttu-id="fc037-194">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-194">Click Bind.</span></span>
27. <span data-ttu-id="fc037-195">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<TransBatch>.</span><span class="sxs-lookup"><span data-stu-id="fc037-195">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical\Cell<TransBatch>'.</span></span>
28. <span data-ttu-id="fc037-196">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Batch: String.</span><span class="sxs-lookup"><span data-stu-id="fc037-196">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Batch: String'.</span></span>
29. <span data-ttu-id="fc037-197">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-197">Click Bind.</span></span>
30. <span data-ttu-id="fc037-198">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical.</span><span class="sxs-lookup"><span data-stu-id="fc037-198">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Range<TransactionLine>: Vertical'.</span></span>
31. <span data-ttu-id="fc037-199">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-199">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Transaction: Record list'.</span></span>
32. <span data-ttu-id="fc037-200">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-200">Click Bind.</span></span>
33. <span data-ttu-id="fc037-201">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Cell<Batch>.</span><span class="sxs-lookup"><span data-stu-id="fc037-201">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical\Cell<Batch>'.</span></span>
34. <span data-ttu-id="fc037-202">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list\Batch: String.</span><span class="sxs-lookup"><span data-stu-id="fc037-202">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list\Batch: String'.</span></span>
35. <span data-ttu-id="fc037-203">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-203">Click Bind.</span></span>
36. <span data-ttu-id="fc037-204">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical.</span><span class="sxs-lookup"><span data-stu-id="fc037-204">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<JournalLine>: Vertical'.</span></span>
37. <span data-ttu-id="fc037-205">Medyje pasirinkite model: Data model Financial dimensions sample model\Journal: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-205">In the tree, select 'model: Data model Financial dimensions sample model\Journal: Record list'.</span></span>
38. <span data-ttu-id="fc037-206">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-206">Click Bind.</span></span>
39. <span data-ttu-id="fc037-207">Medyje išplėskite dalį model: Data model Financial dimensions sample model\Dimensions setting: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-207">In the tree, expand 'model: Data model Financial dimensions sample model\Dimensions setting: Record list'.</span></span>
40. <span data-ttu-id="fc037-208">Medyje pasirinkite dalį model: Data model Financial dimensions sample model\Dimensions setting: Record list\Code: String.</span><span class="sxs-lookup"><span data-stu-id="fc037-208">In the tree, select 'model: Data model Financial dimensions sample model\Dimensions setting: Record list\Code: String'.</span></span>
41. <span data-ttu-id="fc037-209">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal\Cell<DimNames>'.</span><span class="sxs-lookup"><span data-stu-id="fc037-209">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal\Cell<DimNames>'.</span></span>
42. <span data-ttu-id="fc037-210">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-210">Click Bind.</span></span>
43. <span data-ttu-id="fc037-211">Medyje pasirinkite dalį model: Data model Financial dimensions sample model\Dimensions setting: Record list.</span><span class="sxs-lookup"><span data-stu-id="fc037-211">In the tree, select 'model: Data model Financial dimensions sample model\Dimensions setting: Record list'.</span></span>
44. <span data-ttu-id="fc037-212">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal.</span><span class="sxs-lookup"><span data-stu-id="fc037-212">In the tree, select 'Excel = "SampleFinDimWsReport"\Range<DimNames>: Horizontal'.</span></span>
45. <span data-ttu-id="fc037-213">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-213">Click Bind.</span></span>
46. <span data-ttu-id="fc037-214">Medyje pasirinkite Excel = "SampleFinDimWsReport"\Cell<CompanyName>.</span><span class="sxs-lookup"><span data-stu-id="fc037-214">In the tree, select 'Excel = "SampleFinDimWsReport"\Cell<CompanyName>'.</span></span>
47. <span data-ttu-id="fc037-215">Medyje pasirinkite model: Data model Financial dimensions sample model\Company: String.</span><span class="sxs-lookup"><span data-stu-id="fc037-215">In the tree, select 'model: Data model Financial dimensions sample model\Company: String'.</span></span>
48. <span data-ttu-id="fc037-216">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="fc037-216">Click Bind.</span></span>
49. <span data-ttu-id="fc037-217">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="fc037-217">Click Save.</span></span>
50. <span data-ttu-id="fc037-218">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="fc037-218">Close the page.</span></span>

