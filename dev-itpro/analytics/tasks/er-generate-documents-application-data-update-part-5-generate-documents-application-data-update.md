--- 
title: "Dokumentų generavimas elektroninėse ataskaitose (ER) su atnaujintais prašymų duomenimis"
description: "Norėdami atlikti šios procedūros veiksmus, turite pirma užbaigti procedūrą „ER generuoti dokumentus su programos duomenų atnaujinimu (4 dalis – modifikuoti formatą)“."
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
ms.openlocfilehash: 332cfcbdb6ccbb78d30a421adde33a12360df94b
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="generate-documents-with-application-data-update-for-electronic-reporting-er"></a><span data-ttu-id="923bd-103">Dokumentų generavimas elektroninėse ataskaitose (ER) su atnaujintais prašymų duomenimis</span><span class="sxs-lookup"><span data-stu-id="923bd-103">Generate documents with application data update for electronic reporting (ER)</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="923bd-104">Norėdami atlikti šios procedūros veiksmus, turite pirma užbaigti procedūrą „ER generuoti dokumentus su programos duomenų atnaujinimu (4 dalis: modifikuoti formatą)“.</span><span class="sxs-lookup"><span data-stu-id="923bd-104">To complete the steps in this procedure, you must first complete the procedure, “ER Generate documents with application data update (Part 4: Modify format)”.</span></span>



<span data-ttu-id="923bd-105">Veiksmai šioje procedūroje paaiškina, kaip kurti elektroninių ataskaitų (ER) konfigūraciją, norint generuoti elektroninį dokumentą ir atnaujinti programos duomenis.</span><span class="sxs-lookup"><span data-stu-id="923bd-105">The steps in this procedure explain how to design Electronic reporting (ER) configurations to generate an electronic document and update application data.</span></span> <span data-ttu-id="923bd-106">Šioje procedūroje vykdote ER formato konfigūraciją, kad sugeneruotumėte Intrastat ataskaitą ir atnaujintumėte programos duomenis ataskaitų proceso archyvavimo informacijai.</span><span class="sxs-lookup"><span data-stu-id="923bd-106">In this procedure, you execute the ER format configuration to generate the Intrastat report and update application data for archiving details of the reporting process.</span></span>



<span data-ttu-id="923bd-107">Ši procedūra sukurta vartotojams, kuriems priskirtas sistemos administratoriaus arba elektroninių ataskaitų teikimo programuotojo vaidmuo.</span><span class="sxs-lookup"><span data-stu-id="923bd-107">This procedure is created for users with the assigned role of system administrator or electronic reporting developer.</span></span> <span data-ttu-id="923bd-108">Šiuos veiksmus galima atlikti naudojant DEMF duomenų rinkinį.</span><span class="sxs-lookup"><span data-stu-id="923bd-108">These steps can be completed using the DEMF dataset.</span></span> <span data-ttu-id="923bd-109">Prieš pradėdami įsitikinkite, kad šalies kontekstas DEMF įmonei yra BEL (Belgija).</span><span class="sxs-lookup"><span data-stu-id="923bd-109">Before you begin, make sure that the country context for the DEMF company is BEL (Belgium).</span></span>


## <a name="set-up-foreign-trade-parameters"></a><span data-ttu-id="923bd-110">Nustatyti užsienio prekybos parametrus</span><span class="sxs-lookup"><span data-stu-id="923bd-110">Set up foreign trade parameters</span></span>
1. <span data-ttu-id="923bd-111">Eikite į Mokestis > Nustatymas > Užsienio prekyba > Užsienio prekybos parametrai.</span><span class="sxs-lookup"><span data-stu-id="923bd-111">Go to Tax > Setup > Foreign trade > Foreign trade parameters.</span></span>
2. <span data-ttu-id="923bd-112">Spustelėkite skirtuką Numeracijos.</span><span class="sxs-lookup"><span data-stu-id="923bd-112">Click the Number sequences tab.</span></span>
    * <span data-ttu-id="923bd-113">Archyvuojami Intrastat ataskaitų kūrimo proceso informaciją, turime nustatyti kiekvieno archyvo, kurį sukūrėme, įrašus.</span><span class="sxs-lookup"><span data-stu-id="923bd-113">Archiving details of Intrastat reporting process, we need to identify records of each archive we created.</span></span> <span data-ttu-id="923bd-114">Tam reikia konfigūruoti specialią numerių seką.</span><span class="sxs-lookup"><span data-stu-id="923bd-114">A special number sequence must be configured for that.</span></span>  
3. <span data-ttu-id="923bd-115">Pasirinkite „Intrastat archyvo ID“ nuorodą.</span><span class="sxs-lookup"><span data-stu-id="923bd-115">Select the ‘Intrastat archive ID’ reference.</span></span>
4. <span data-ttu-id="923bd-116">Lauke Numeracijos kodas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="923bd-116">In the Number sequence code field, type a value.</span></span>
    * <span data-ttu-id="923bd-117">Lauke „Numerių sekos kodas“ įveskite arba pasirinkite vertę „Fore_2“.</span><span class="sxs-lookup"><span data-stu-id="923bd-117">In the ‘Number sequence code’ field, enter or select the value ‘Fore_2’.</span></span>  
5. <span data-ttu-id="923bd-118">ResolveChanges Numerio sekos kodas.</span><span class="sxs-lookup"><span data-stu-id="923bd-118">ResolveChanges the Number sequence code.</span></span>
6. <span data-ttu-id="923bd-119">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="923bd-119">Click Save.</span></span>
7. <span data-ttu-id="923bd-120">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="923bd-120">Close the page.</span></span>

## <a name="run-modified-er-format"></a><span data-ttu-id="923bd-121">Paleiskite pakeistą ER formatą</span><span class="sxs-lookup"><span data-stu-id="923bd-121">Run modified ER format</span></span>
1. <span data-ttu-id="923bd-122">Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="923bd-122">Go to Organization administration > Electronic reporting > Configurations.</span></span>
2. <span data-ttu-id="923bd-123">Medyje išplėskite „Intrastat (model)“.</span><span class="sxs-lookup"><span data-stu-id="923bd-123">In the tree, expand 'Intrastat (model)'.</span></span>
3. <span data-ttu-id="923bd-124">Medyje pasirinkite „Intrastat (model)\Intrastat (format)“.</span><span class="sxs-lookup"><span data-stu-id="923bd-124">In the tree, select 'Intrastat (model)\Intrastat (format)'.</span></span>
4. <span data-ttu-id="923bd-125">Spustelėkite Vykdyti.</span><span class="sxs-lookup"><span data-stu-id="923bd-125">Click Run.</span></span>
5. <span data-ttu-id="923bd-126">Lauke Įveskite failo pavadinimą įveskite „intrastat2.xml“.</span><span class="sxs-lookup"><span data-stu-id="923bd-126">In the Enter file name field, type 'intrastat2.xml'.</span></span>
    * <span data-ttu-id="923bd-127">intrastat2.xml</span><span class="sxs-lookup"><span data-stu-id="923bd-127">intrastat2.xml</span></span>  
6. <span data-ttu-id="923bd-128">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="923bd-128">Click OK.</span></span>

## <a name="review-er-format-executions-results"></a><span data-ttu-id="923bd-129">Peržiūrėkite ER formato vykdymo rezultatus</span><span class="sxs-lookup"><span data-stu-id="923bd-129">Review ER format execution’s results</span></span>
    * <span data-ttu-id="923bd-130">Peržiūrėkite sugeneruotą XML failą.</span><span class="sxs-lookup"><span data-stu-id="923bd-130">Review the generated XML file.</span></span>  
1. <span data-ttu-id="923bd-131">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="923bd-131">Close the page.</span></span>
2. <span data-ttu-id="923bd-132">Pasirinkite Mokesčiai > Deklaracijos > Užsienio prekyba > Intrastat.</span><span class="sxs-lookup"><span data-stu-id="923bd-132">Go to Tax > Declarations > Foreign trade > Intrastat.</span></span>
    * <span data-ttu-id="923bd-133">Atidarykite šią formą, kurioje yra Intrastat operacijos, kurios buvo įtrauktos sugeneruotą elektroninį dokumentą.</span><span class="sxs-lookup"><span data-stu-id="923bd-133">Open this form containing Intrastat transactions that have been included to the generated electronic document.</span></span>  
3. <span data-ttu-id="923bd-134">Spustelėkite Intrastat archyvas.</span><span class="sxs-lookup"><span data-stu-id="923bd-134">Click Intrastat archive.</span></span>
    * <span data-ttu-id="923bd-135">Kadangi įvykdyto ER formate dabar yra programos duomenų atnaujinimo parametrai, informacija apie užpildytą Intrastat ataskaitą suarchyvuota.</span><span class="sxs-lookup"><span data-stu-id="923bd-135">Since the executed ER format contains now settings for application data update, the details of the completed Intrastat reporting have been archived.</span></span> <span data-ttu-id="923bd-136">Šioje formoje galite pamatyti sukurto archyvo antraštės įrašą.</span><span class="sxs-lookup"><span data-stu-id="923bd-136">In this form, you can see the header record of the created archive.</span></span>  
4. <span data-ttu-id="923bd-137">Spustelėkite Informacija.</span><span class="sxs-lookup"><span data-stu-id="923bd-137">Click Details.</span></span>
    * <span data-ttu-id="923bd-138">Šioje formoje galite pamatyti sukurto archyvo išsamią informaciją.</span><span class="sxs-lookup"><span data-stu-id="923bd-138">In this form, you can see the details for the created archive.</span></span>  
5. <span data-ttu-id="923bd-139">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="923bd-139">Close the page.</span></span>
6. <span data-ttu-id="923bd-140">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="923bd-140">Close the page.</span></span>
7. <span data-ttu-id="923bd-141">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="923bd-141">Close the page.</span></span>

