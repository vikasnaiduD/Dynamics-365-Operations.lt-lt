---
title: "Duomenų importavimas iš „Excel“ duomenų objekto šablonų naudojant kelis darbalapius"
description: "Šioje temoje aprašoma, kaip naudojant „Excel“ duomenų objekto šablonus importuoti duomenis į „Microsoft Dynamics 365 for Finance and Operations, Enterprise Edition“."
author: Sunil-Garg
manager: AnnBe
ms.date: 01/01/2018
ms.topic: article
ms.prod: 
ms.service: dynamics-ax-platform
ms.technology: 
audience: Application user
ms.reviewer: margoc
ms.search.scope: Operations
ms.custom: 
ms.assetid: 
ms.search.region: Global
ms.author: sunilg
ms.search.validFrom: 2018-01-01
ms.dyn365.ops.version: Platform update 13
ms.translationtype: HT
ms.sourcegitcommit: 0ca19ab9ed7a52328c5dd5252c418bb9343bdc2b
ms.openlocfilehash: 84b9e9128d7ea6cdf9949549f4ab7a1c6c01691b
ms.contentlocale: lt-lt
ms.lasthandoff: 12/14/2017

---

# <a name="excel-templates-with-multiple-worksheets"></a><span data-ttu-id="92d02-103">„Excel“ šablonai su keliais darbalapiais</span><span class="sxs-lookup"><span data-stu-id="92d02-103">Excel templates with multiple worksheets</span></span>

<span data-ttu-id="92d02-104">„Microsoft Dynamics 365 for Finance and Operations, Enterprise Edition“ duomenų valdymas palaiko „Microsoft Excel“ pagrįstus šablonus, skirtus duomenų objektams.</span><span class="sxs-lookup"><span data-stu-id="92d02-104">Data management in Microsoft Dynamics 365 for Finance and Operations, Enterprise edition supports Microsoft Excel-based templates for data entities.</span></span> <span data-ttu-id="92d02-105">Šiuose šablonuose gali būti vienas ar daugiau darbalapių.</span><span class="sxs-lookup"><span data-stu-id="92d02-105">These templates can contain one or more worksheets.</span></span> <span data-ttu-id="92d02-106">Šablonai su keliais darbalapiais dažnai naudojami, kai patogu tvarkyti duomenis viename faile ir importuoti juos į kelis duomenų objektus.</span><span class="sxs-lookup"><span data-stu-id="92d02-106">Templates with multiple worksheets are often used when it is convenient to manage data in a single file and import it to multiple data entities.</span></span> <span data-ttu-id="92d02-107">Pavyzdys: vietos ir sandėliai.</span><span class="sxs-lookup"><span data-stu-id="92d02-107">An example would be sites and warehouses.</span></span>

## <a name="upload-a-file-once-and-map-it-to-all-entities"></a><span data-ttu-id="92d02-108">Failo įkėlimas vieną kartą ir susiejimas su visais objektais</span><span class="sxs-lookup"><span data-stu-id="92d02-108">Upload a file once and map it to all entities</span></span>
<span data-ttu-id="92d02-109">Apžvelkime pavyzdį: turime vieną „Excel“ failą ir darbalapius pavadinimais **Vietos** ir **Sandėliai**.</span><span class="sxs-lookup"><span data-stu-id="92d02-109">Let’s take an example where there is one Excel file with worksheets called **Sites** and **Warehouses**.</span></span> <span data-ttu-id="92d02-110">Norėdami nustatyti duomenų importavimo projektą, įtraukite pirmą duomenų objektą, **Vietos**, tada nusiųskite failą.</span><span class="sxs-lookup"><span data-stu-id="92d02-110">To set up the data import project, you would add the first data entity, **Sites** and then upload the file.</span></span> <span data-ttu-id="92d02-111">Kaip šio objekto naudotiną darbalapį galėsite pasirinkti darbalapį **Vietos**.</span><span class="sxs-lookup"><span data-stu-id="92d02-111">You will be able to select **Sites** as the worksheet to be used for this entity.</span></span>

<span data-ttu-id="92d02-112">Jei įtrauksite antrą objektą **Sandėliai** neuždarę formos **Įtraukti failą**, darbalapių peržvalgoje galėsite pasirinkti darbalapį **Sandėliai** ir jums nereikės dar kartą nusiųsti failo.</span><span class="sxs-lookup"><span data-stu-id="92d02-112">If you add the second entity **Warehouses** without leaving the **Add file** form, the worksheet lookup will let you select the **Warehouses** worksheet without having to upload the file again.</span></span> <span data-ttu-id="92d02-113">Naują failą nusiųsti reikėtų tik jei darbalapio **Sandėliai** duomenys buvo į kitame faile.</span><span class="sxs-lookup"><span data-stu-id="92d02-113">The only reason to upload a new file would be if the **Warehouses** data was in a different file.</span></span>

![Keli darbalapiai](./media/AddFileMultipleWorkSheets.png) 

## <a name="fix-worksheet-to-entity-mapping"></a><span data-ttu-id="92d02-115">Darbalapio susiejimo su objektu nustatymas</span><span class="sxs-lookup"><span data-stu-id="92d02-115">Fix worksheet to entity mapping</span></span>

<span data-ttu-id="92d02-116">Darbalapio susiejimą su duomenų objektu importavimo užduotyje galima nustatyti naudojant tinklelį.</span><span class="sxs-lookup"><span data-stu-id="92d02-116">The mapping of the worksheet to a data entity in the import job can be fixed from the grid.</span></span> <span data-ttu-id="92d02-117">Tinklelio stulpelyje **Darbalapis** rodomi susieto failo darbalapiai.</span><span class="sxs-lookup"><span data-stu-id="92d02-117">The **Worksheet** column in the grid shows the worksheets from the file that was mapped.</span></span> <span data-ttu-id="92d02-118">Išplečiamajame meniu galite pasirinkti kitą darbalapį.</span><span class="sxs-lookup"><span data-stu-id="92d02-118">You can choose a different worksheet from the drop-down menu.</span></span> <span data-ttu-id="92d02-119">Jei pasirinktas darbalapis jau susietas su objektu duomenų projekte, sistema paprašys patvirtinti pakeitimą.</span><span class="sxs-lookup"><span data-stu-id="92d02-119">If the chosen worksheet is already mapped to an entity in the data project, the system asks you to confirm the change.</span></span> <span data-ttu-id="92d02-120">Rekomenduojame nustatyti visus susiejimus tinklelyje.</span><span class="sxs-lookup"><span data-stu-id="92d02-120">We recommend that you fix all mappings in the grid.</span></span>

![Darbalapio susiejimo naujinimas](./media/UpdateMappings.png)

## <a name="re-map-to-a-new-file"></a><span data-ttu-id="92d02-122">Pakartotinis susiejimas su nauju failu</span><span class="sxs-lookup"><span data-stu-id="92d02-122">Re-map to a new file</span></span>

<span data-ttu-id="92d02-123">Tais atvejais, kai duomenų projekte reikia nusiųsti esamų objektų to pačio failo naują versiją arba visiškai naują failą, turite naudoti formą **Įtraukti failą** ir vėl įtraukti objektus, kaip juos įtrauktumėte pirmą kartą.</span><span class="sxs-lookup"><span data-stu-id="92d02-123">In cases where a new version of the same file or a completely new file must be uploaded for existing entities in a data project, you must use the **Add file** experience, and add the entities again as if they were being added for the first time.</span></span> <span data-ttu-id="92d02-124">Prieš tęsiant sistema patvirtins, kad norite perrašyti esamus objektus duomenų projekte.</span><span class="sxs-lookup"><span data-stu-id="92d02-124">The system will confirm that you want to overwrite the existing entities in the data project before proceeding.</span></span> <span data-ttu-id="92d02-125">Objektų, kurie dar kartą neįtraukiami (arba neperrašomi), susiejimai (iš kito ankstesnio failo) išliks.</span><span class="sxs-lookup"><span data-stu-id="92d02-125">Entities that are not added again (or overwritten) will continue to hold the previous mappings from the previous file.</span></span>

## <a name="upload-a-file-using-run-project"></a><span data-ttu-id="92d02-126">Failo nusiuntimas naudojant parinktį Vykdyti projektą</span><span class="sxs-lookup"><span data-stu-id="92d02-126">Upload a file using Run project</span></span>

<span data-ttu-id="92d02-127">Galite įkelti „Excel“ failą naudodami parinktį **Vykdyti projektą**, norėdami vykdyti importavimo projektą.</span><span class="sxs-lookup"><span data-stu-id="92d02-127">You can upload an Excel file while using the **Run project** option to execute an import project.</span></span> <span data-ttu-id="92d02-128">Turite būti atsargūs ir nusiųsti tik failus, kuriuose yra darbalapiai, atitinkantys duomenų projekto duomenų objektų esamus susiejimus.</span><span class="sxs-lookup"><span data-stu-id="92d02-128">You must be careful to upload only files that have the same worksheets as the existing mappings on the data entities in the data project.</span></span> <span data-ttu-id="92d02-129">Jei naujai nusiųstame faile darbalapių nerasta, sistema rodo klaidą ir importavimas sustabdomas.</span><span class="sxs-lookup"><span data-stu-id="92d02-129">If a worksheet is not found in the newly uploaded file, the system displays an error and will stop the import.</span></span> <span data-ttu-id="92d02-130">Jei objekto susiejimą su darbalapiu reikia keisti, pirmiausia reikia atnaujinti duomenų projekto susiejimus pačiame duomenų objekte, kad būtų galima naudoti failą formoje **Vykdyti projektą**.</span><span class="sxs-lookup"><span data-stu-id="92d02-130">If the mapping to the worksheet must be changed for an entity, then the mappings in the data project must be first updated from within the data project before using the file in the **Run project** experience.</span></span>

