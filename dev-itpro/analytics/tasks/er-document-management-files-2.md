--- 
title: "Duomenų modelio išplėtimas, kad dokumentų valdymo failai galėtų būti naudojami formato išvestyse elektroninėse ataskaitose (ER)"
description: "Toliau nurodytuose veiksmuose paaiškinta, kaip vartotojas, kuriam priskirtas sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmuo, gali konfigūruoti elektroninių ataskaitų (ER) formatą, norėdamas dokumentų valdymo failus (priedus) naudoti ER išvestyje."
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
ms.openlocfilehash: 1a5325dc3a97b9e205b41fe8dae18f43e430daeb
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="extend-data-model-to-use-document-management-files-in-format-outputs-for-electronic-reporting-er"></a><span data-ttu-id="08367-103">Duomenų modelio išplėtimas, kad dokumentų valdymo failai galėtų būti naudojami formato išvestyse elektroninėse ataskaitose (ER)</span><span class="sxs-lookup"><span data-stu-id="08367-103">Extend data model to use Document Management files in format outputs for electronic reporting (ER)</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="08367-104">Toliau nurodytuose veiksmuose paaiškinta, kaip vartotojas, kuriam priskirtas sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmuo, gali konfigūruoti elektroninių ataskaitų (ER) formatą, norėdamas dokumentų valdymo failus (priedus) naudoti ER išvestyje.</span><span class="sxs-lookup"><span data-stu-id="08367-104">The following steps explain how a user assigned to the System Administrator or Electronic Reporting Developer role can configure an Electronic reporting (ER) format to use Document Management files (attachments) in ER output.</span></span> <span data-ttu-id="08367-105">Šiuos veiksmus galima atlikti bet kurioje įmonėje.</span><span class="sxs-lookup"><span data-stu-id="08367-105">These steps can be performed in any company.</span></span>

<span data-ttu-id="08367-106">Norėdami atlikti šiuos veiksmus, pirmiausia turite atlikti veiksmus, nurodytus užduočių vedlyje „ER: dokumentų valdymo failų naudojimas formato išvestyse (1 dalis: duomenų modelio ruošimas)“.</span><span class="sxs-lookup"><span data-stu-id="08367-106">To complete these steps, you must first complete the steps in the “ER Use Document Management files in format outputs (Part 1: Prepare data model)” task guide.</span></span>

<span data-ttu-id="08367-107">Ši procedūra yra skirta funkcijai, įtrauktai į „Dynamics 365 for Operations“ 1611 versiją.</span><span class="sxs-lookup"><span data-stu-id="08367-107">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>


## <a name="extend-data-model-to-present-the-document-management-files-in-it"></a><span data-ttu-id="08367-108">Duomenų modelio išplėtimas, kad jame būtų pateikti dokumentų valdymo failai</span><span class="sxs-lookup"><span data-stu-id="08367-108">Extend data model to present the Document Management files in it</span></span>
1. <span data-ttu-id="08367-109">Pasirinkite Organizacijos administravimas > Darbo sritys > Elektroninės ataskaitos.</span><span class="sxs-lookup"><span data-stu-id="08367-109">Go to Organization administration > Workspaces > Electronic reporting.</span></span>
2. <span data-ttu-id="08367-110">Spustelėkite Ataskaitų konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="08367-110">Click Reporting configurations.</span></span>
3. <span data-ttu-id="08367-111">Medyje išplėskite Kliento SF modelis.</span><span class="sxs-lookup"><span data-stu-id="08367-111">In the tree, expand 'Customer invoice model'.</span></span>
4. <span data-ttu-id="08367-112">Medyje pasirinkite dalį Customer invoice model\Customer invoice model (custom).</span><span class="sxs-lookup"><span data-stu-id="08367-112">In the tree, select 'Customer invoice model\Customer invoice model (custom)'.</span></span>
5. <span data-ttu-id="08367-113">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="08367-113">Click Designer.</span></span>
6. <span data-ttu-id="08367-114">Medyje pasirinkite Customer invoice(InvoiceCustomer).</span><span class="sxs-lookup"><span data-stu-id="08367-114">In the tree, select 'Customer invoice(InvoiceCustomer)'.</span></span>
    * <span data-ttu-id="08367-115">Išplėsime šį duomenų modelį, kad jame būtų rodomi visi failai, pridėti prie pardavimo užsakymo, kuris yra susijęs su elektroniniu būdu apdorojama SF.</span><span class="sxs-lookup"><span data-stu-id="08367-115">We will extend this data model to expose in it any files that have been attached to a sales order that is related to an electronically processing invoice.</span></span>  
7. <span data-ttu-id="08367-116">Spustelėdami Naujas atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="08367-116">Click New to open the drop dialog.</span></span>
8. <span data-ttu-id="08367-117">Lauke Pavadinimas, įveskite SF priedai.</span><span class="sxs-lookup"><span data-stu-id="08367-117">In the Name field, type 'Invoice attachments'.</span></span>
    * <span data-ttu-id="08367-118">SF priedai</span><span class="sxs-lookup"><span data-stu-id="08367-118">Invoice attachments</span></span>  
9. <span data-ttu-id="08367-119">Lauke „Prekės tipas“ pasirinkite „Įrašų sąrašas“.</span><span class="sxs-lookup"><span data-stu-id="08367-119">In the Item type field, select 'Record list'.</span></span>
10. <span data-ttu-id="08367-120">Spustelėkite Pridėti.</span><span class="sxs-lookup"><span data-stu-id="08367-120">Click Add.</span></span>
11. <span data-ttu-id="08367-121">Spustelėdami Naujas atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="08367-121">Click New to open the drop dialog.</span></span>
12. <span data-ttu-id="08367-122">Lauke Pavadinimas įveskite Failo turinys.</span><span class="sxs-lookup"><span data-stu-id="08367-122">In the Name field, type 'File content'.</span></span>
    * <span data-ttu-id="08367-123">Failo turinys</span><span class="sxs-lookup"><span data-stu-id="08367-123">File content</span></span>  
13. <span data-ttu-id="08367-124">Lauke Prekės tipas pasirinkite Konteineris.</span><span class="sxs-lookup"><span data-stu-id="08367-124">In the Item type field, select 'Container'.</span></span>
14. <span data-ttu-id="08367-125">Spustelėkite Pridėti.</span><span class="sxs-lookup"><span data-stu-id="08367-125">Click Add.</span></span>
15. <span data-ttu-id="08367-126">Spustelėdami Naujas atidarykite išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="08367-126">Click New to open the drop dialog.</span></span>
16. <span data-ttu-id="08367-127">Lauke Pavadinimas įveskite Failo vardas.</span><span class="sxs-lookup"><span data-stu-id="08367-127">In the Name field, type 'File name'.</span></span>
    * <span data-ttu-id="08367-128">Failo vardas</span><span class="sxs-lookup"><span data-stu-id="08367-128">File name</span></span>  
17. <span data-ttu-id="08367-129">Lauke „Prekės tipas“ pasirinkite „Eilutė“.</span><span class="sxs-lookup"><span data-stu-id="08367-129">In the Item type field, select 'String'.</span></span>
18. <span data-ttu-id="08367-130">Spustelėkite Pridėti.</span><span class="sxs-lookup"><span data-stu-id="08367-130">Click Add.</span></span>

## <a name="map-new-data-model-elements-to-dynamics-365-for-finance-and-operations-enterprise-edition-data-sources"></a><span data-ttu-id="08367-131">Naujų duomenų modelio elementų susiejimas su „Dynamics 365 for Finance and Operations“, „Enterprise“ leidimo duomenų šaltiniais</span><span class="sxs-lookup"><span data-stu-id="08367-131">Map new data model elements to Dynamics 365 for Finance and Operations, Enterprise edition data sources</span></span>
1. <span data-ttu-id="08367-132">Spustelėkite „Susieti modelį su duomenų šaltiniu“.</span><span class="sxs-lookup"><span data-stu-id="08367-132">Click Map model to datasource.</span></span>
2. <span data-ttu-id="08367-133">Naudokite spartųjį filtrą, kad atfiltruotumėte lauką Aprašas pagal reikšmę InvoiceCustomer.</span><span class="sxs-lookup"><span data-stu-id="08367-133">Use the Quick Filter to filter on the Definition field with a value of 'InvoiceCustomer'.</span></span>
    * <span data-ttu-id="08367-134">InvoiceCustomer</span><span class="sxs-lookup"><span data-stu-id="08367-134">InvoiceCustomer</span></span>  
    * <span data-ttu-id="08367-135">Susiesime naujo modelio elementus su tinkamais duomenų šaltiniais.</span><span class="sxs-lookup"><span data-stu-id="08367-135">We will map new model elements to appropriate data sources.</span></span>  
3. <span data-ttu-id="08367-136">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="08367-136">Click Designer.</span></span>
4. <span data-ttu-id="08367-137">Medyje pasirinkite SF priedai.</span><span class="sxs-lookup"><span data-stu-id="08367-137">In the tree, select 'Invoice attachments'.</span></span>
5. <span data-ttu-id="08367-138">Medyje išplėskite SF priedai.</span><span class="sxs-lookup"><span data-stu-id="08367-138">In the tree, expand 'Invoice attachments'.</span></span>
6. <span data-ttu-id="08367-139">Medyje pasirinkite Invoice attachments\File name.</span><span class="sxs-lookup"><span data-stu-id="08367-139">In the tree, select 'Invoice attachments\File name'.</span></span>
7. <span data-ttu-id="08367-140">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="08367-140">Click Edit.</span></span>
8. <span data-ttu-id="08367-141">Lauke Formulė įveskite CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'originalFileName()'.</span><span class="sxs-lookup"><span data-stu-id="08367-141">In the Formula field, enter 'CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'originalFileName()''.</span></span>
    * <span data-ttu-id="08367-142">CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'originalFileName()'</span><span class="sxs-lookup"><span data-stu-id="08367-142">CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'originalFileName()'</span></span>  
9. <span data-ttu-id="08367-143">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="08367-143">Click Save.</span></span>
10. <span data-ttu-id="08367-144">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="08367-144">Close the page.</span></span>
11. <span data-ttu-id="08367-145">Medyje pasirinkite Invoice attachments\File content.</span><span class="sxs-lookup"><span data-stu-id="08367-145">In the tree, select 'Invoice attachments\File content'.</span></span>
12. <span data-ttu-id="08367-146">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="08367-146">Click Edit.</span></span>
13. <span data-ttu-id="08367-147">Lauke Formulė įveskite CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'getFileContentAsContainer()'.</span><span class="sxs-lookup"><span data-stu-id="08367-147">In the Formula field, enter 'CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'getFileContentAsContainer()''.</span></span>
    * <span data-ttu-id="08367-148">CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'getFileContentAsContainer()'</span><span class="sxs-lookup"><span data-stu-id="08367-148">CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.'getFileContentAsContainer()'</span></span>  
14. <span data-ttu-id="08367-149">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="08367-149">Click Save.</span></span>
15. <span data-ttu-id="08367-150">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="08367-150">Close the page.</span></span>
16. <span data-ttu-id="08367-151">Medyje pasirinkite SF priedai.</span><span class="sxs-lookup"><span data-stu-id="08367-151">In the tree, select 'Invoice attachments'.</span></span>
17. <span data-ttu-id="08367-152">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="08367-152">Click Edit.</span></span>
18. <span data-ttu-id="08367-153">Lauke Formulė įveskite CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'.</span><span class="sxs-lookup"><span data-stu-id="08367-153">In the Formula field, enter 'CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents''.</span></span>
    * <span data-ttu-id="08367-154">CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'</span><span class="sxs-lookup"><span data-stu-id="08367-154">CustInvoiceJour.'>Relations'.SalesTable.'<Relations'.'<Documents'</span></span>  
19. <span data-ttu-id="08367-155">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="08367-155">Click Save.</span></span>
20. <span data-ttu-id="08367-156">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="08367-156">Close the page.</span></span>
21. <span data-ttu-id="08367-157">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="08367-157">Click Save.</span></span>
22. <span data-ttu-id="08367-158">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="08367-158">Close the page.</span></span>
23. <span data-ttu-id="08367-159">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="08367-159">Close the page.</span></span>
24. <span data-ttu-id="08367-160">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="08367-160">Close the page.</span></span>
25. <span data-ttu-id="08367-161">Spustelėkite keisti būseną.</span><span class="sxs-lookup"><span data-stu-id="08367-161">Click Change status.</span></span>
26. <span data-ttu-id="08367-162">Spustelėkite Baigti.</span><span class="sxs-lookup"><span data-stu-id="08367-162">Click Complete.</span></span>
27. <span data-ttu-id="08367-163">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="08367-163">Click OK.</span></span>

