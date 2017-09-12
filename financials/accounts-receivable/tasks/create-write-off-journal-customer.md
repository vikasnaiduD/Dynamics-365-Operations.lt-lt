--- 
title: "Kurti kliento nurašymo žurnalą"
description: "Šis užduočių vadovas jums parodys, kaip nustatyti nurašymų parametrus ir tada nurašyti operacijas puslapyje Rinkiniai, puslapyje Atidarytos klientų SF ir puslapyje Klientas."
author: ShivamPandey-msft
manager: AnnBe
ms.date: 11/14/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 19a816f04283ce4f200de7396617313e45e057db
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="create-a-write-off-journal-for-a-customer"></a><span data-ttu-id="759ae-103">Kurti kliento nurašymo žurnalą</span><span class="sxs-lookup"><span data-stu-id="759ae-103">Create a write-off journal for a customer</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="759ae-104">Šis užduočių vadovas jums parodys, kaip nustatyti nurašymų parametrus ir tada nurašyti operacijas puslapyje Rinkiniai, puslapyje Atidarytos klientų SF ir puslapyje Klientas.</span><span class="sxs-lookup"><span data-stu-id="759ae-104">This task guide will show you how to set up the parameters for write-offs and then write off transactions from the Collections page, the Open customer invoices page, and the Customer page.</span></span> <span data-ttu-id="759ae-105">Šioje užduotyje naudojama demonstracinė įmonė USMF.</span><span class="sxs-lookup"><span data-stu-id="759ae-105">This task uses the USMF demo company.</span></span>


## <a name="set-up-the-write-off-parameters"></a><span data-ttu-id="759ae-106">Nustatyti nurašymo parametrus</span><span class="sxs-lookup"><span data-stu-id="759ae-106">Set up the write off parameters</span></span>
1. <span data-ttu-id="759ae-107">Pasirinkite Kreditas ir rinkiniai > Sąranka > Gautinų sumų parametrai.</span><span class="sxs-lookup"><span data-stu-id="759ae-107">Go to Credit and collections > Setup > Accounts receivable parameters.</span></span>
2. <span data-ttu-id="759ae-108">Spustelėkite skirtuką Rinkiniai.</span><span class="sxs-lookup"><span data-stu-id="759ae-108">Click the Collections tab.</span></span>
3. <span data-ttu-id="759ae-109">Išplėskite arba sutraukite dalį Nurašymas.</span><span class="sxs-lookup"><span data-stu-id="759ae-109">Expand or collapse the Write-off section.</span></span>
    * <span data-ttu-id="759ae-110">Nurašymo žurnalas yra bendrasis žurnalas, kuriame bus laikomos jūsų sukurtos nurašymo operacijos.</span><span class="sxs-lookup"><span data-stu-id="759ae-110">The Write-off journal is the general journal that will hold the write-off transactions that you create.</span></span>  
    * <span data-ttu-id="759ae-111">Prie kiekvieno nurašymo galite pridėti priežasties kodą.</span><span class="sxs-lookup"><span data-stu-id="759ae-111">You can attach a reason code to every write-off.</span></span> <span data-ttu-id="759ae-112">Nurašydami šios numatytosios nuostatos galite nepaisyti.</span><span class="sxs-lookup"><span data-stu-id="759ae-112">You can override this default at the time of the write-off.</span></span>  
    * <span data-ttu-id="759ae-113">Šią parinktį nustatykite į Taip, jei norite atskirti PVM nuo pradinės nurašymo operacijos.</span><span class="sxs-lookup"><span data-stu-id="759ae-113">Set this to Yes if you want to separate the sales tax from the original transaction in the write-off.</span></span>  
4. <span data-ttu-id="759ae-114">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-114">Close the page.</span></span>
5. <span data-ttu-id="759ae-115">Pasirinkite Kreditas ir rinkiniai > Sąranka > Klientų registravimo šablonai.</span><span class="sxs-lookup"><span data-stu-id="759ae-115">Go to Credit and collections > Setup > Customer posting profiles.</span></span>
    * <span data-ttu-id="759ae-116">Nurašymo sąskaita bus naudojama kaip išlaidų sąskaita arba rezervo koregavimas bendrajame žurnale</span><span class="sxs-lookup"><span data-stu-id="759ae-116">The write-off account will be used as the expense account or reserve adjustment in the general journal</span></span>   
6. <span data-ttu-id="759ae-117">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-117">Close the page.</span></span>

## <a name="write-off-a-customer-balance-from-the-aged-balances-page"></a><span data-ttu-id="759ae-118">Nurašyti kliento balansą pagal terminus suskirstytų balansų puslapyje</span><span class="sxs-lookup"><span data-stu-id="759ae-118">Write off a customer balance from the aged balances page</span></span>
1. <span data-ttu-id="759ae-119">Pasirinkite Kreditas ir rinkiniai > Rinkiniai > Pagal terminus suskirstyti balansai.</span><span class="sxs-lookup"><span data-stu-id="759ae-119">Go to Credit and collections > Collections > Aged balances.</span></span>
2. <span data-ttu-id="759ae-120">Pažymėkite kliento eilutę, kurią norite nurašyti.</span><span class="sxs-lookup"><span data-stu-id="759ae-120">Mark the row for the customer that you want to write off.</span></span> <span data-ttu-id="759ae-121">Pavyzdžiui, pažymėkite eilutę su Birch Company.</span><span class="sxs-lookup"><span data-stu-id="759ae-121">For example, mark the line with Birch Company on it.</span></span>
3. <span data-ttu-id="759ae-122">Veiksmų srityje spustelėkite Rinkti.</span><span class="sxs-lookup"><span data-stu-id="759ae-122">On the Action Pane, click Collect.</span></span>
4. <span data-ttu-id="759ae-123">Spustelėkite Nurašyti.</span><span class="sxs-lookup"><span data-stu-id="759ae-123">Click Write off.</span></span>
5. <span data-ttu-id="759ae-124">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="759ae-124">Click OK.</span></span>
6. <span data-ttu-id="759ae-125">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-125">Close the page.</span></span>
7. <span data-ttu-id="759ae-126">Pasirinkite Didžioji knyga > Žurnalų įrašai > Bendrieji žurnalai.</span><span class="sxs-lookup"><span data-stu-id="759ae-126">Go to General ledger > Journal entries > General journals.</span></span>
8. <span data-ttu-id="759ae-127">Pasirinkite žurnalo, kuriame yra jūsų nurašymas, paketo numerį.</span><span class="sxs-lookup"><span data-stu-id="759ae-127">Select the journal batch number for the journal that contains your write-off.</span></span>
    * <span data-ttu-id="759ae-128">Atšaukti kliento balansui sukuriama viena eilutė.</span><span class="sxs-lookup"><span data-stu-id="759ae-128">One line is created to reverse the customer balance.</span></span> <span data-ttu-id="759ae-129">Viena ar kelios eilutės sukuriamos registruoti nurašymui nurašymo sąskaitoje.</span><span class="sxs-lookup"><span data-stu-id="759ae-129">One or more lines are created to post the write-off to the write-off account.</span></span>  
9. <span data-ttu-id="759ae-130">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-130">Close the page.</span></span>
10. <span data-ttu-id="759ae-131">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-131">Close the page.</span></span>

## <a name="write-off-transactions-from-the-collections-form"></a><span data-ttu-id="759ae-132">Nurašykite operacijas rinkinių formoje.</span><span class="sxs-lookup"><span data-stu-id="759ae-132">Write off transactions from the collections form.</span></span>
1. <span data-ttu-id="759ae-133">Pasirinkite Kreditas ir rinkiniai > Rinkiniai > Pagal terminus suskirstyti balansai.</span><span class="sxs-lookup"><span data-stu-id="759ae-133">Go to Credit and collections > Collections > Aged balances.</span></span>
2. <span data-ttu-id="759ae-134">Pasirinkite kliento su operacijomis, kurias norite nurašyti, pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="759ae-134">Select the name of the customer that has the transactions that you want to write off.</span></span> <span data-ttu-id="759ae-135">Pavyzdžiui, pasirinkite Cave Wholesales (US-004).</span><span class="sxs-lookup"><span data-stu-id="759ae-135">For example, select Cave Wholesales (US-004).</span></span>
3. <span data-ttu-id="759ae-136">Pažymėkite pirmosios operacijos eilutę.</span><span class="sxs-lookup"><span data-stu-id="759ae-136">Mark the row for the first transaction.</span></span>
4. <span data-ttu-id="759ae-137">Pažymėkite antrosios operacijos eilutę.</span><span class="sxs-lookup"><span data-stu-id="759ae-137">Mark the row for the second transaction.</span></span>
5. <span data-ttu-id="759ae-138">Spustelėkite Nurašyti.</span><span class="sxs-lookup"><span data-stu-id="759ae-138">Click Write off.</span></span>
6. <span data-ttu-id="759ae-139">Lauke Priežasties komentaras surinkite „Blogos skolos‟.</span><span class="sxs-lookup"><span data-stu-id="759ae-139">In the Reason comment field, type 'Bad debts'.</span></span>
7. <span data-ttu-id="759ae-140">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="759ae-140">Click OK.</span></span>
8. <span data-ttu-id="759ae-141">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-141">Close the page.</span></span>
9. <span data-ttu-id="759ae-142">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-142">Close the page.</span></span>
10. <span data-ttu-id="759ae-143">Pasirinkite Didžioji knyga > Žurnalų įrašai > Bendrieji žurnalai.</span><span class="sxs-lookup"><span data-stu-id="759ae-143">Go to General ledger > Journal entries > General journals.</span></span>
11. <span data-ttu-id="759ae-144">Pasirinkite žurnalo, kuriame yra jūsų nurašymas, paketo numerį.</span><span class="sxs-lookup"><span data-stu-id="759ae-144">Select the journal batch number for the journal that contains your write-off.</span></span>
    * <span data-ttu-id="759ae-145">Atšaukti kliento balansui sukuriama viena eilutė.</span><span class="sxs-lookup"><span data-stu-id="759ae-145">One line is created to reverse the customer balance.</span></span> <span data-ttu-id="759ae-146">Viena ar kelios eilutės sukuriamos registruoti nurašymui nurašymo sąskaitoje.</span><span class="sxs-lookup"><span data-stu-id="759ae-146">One or more lines are created to post the write-off to the write-off account.</span></span>  
12. <span data-ttu-id="759ae-147">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-147">Close the page.</span></span>
13. <span data-ttu-id="759ae-148">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-148">Close the page.</span></span>

## <a name="write-off-an-invoice-from-the-open-customers-invoices-page"></a><span data-ttu-id="759ae-149">Nurašyti SF puslapyje Atidarytos klientų SF</span><span class="sxs-lookup"><span data-stu-id="759ae-149">Write off an invoice from the Open customers invoices page</span></span>
1. <span data-ttu-id="759ae-150">Pasirinkite Gautinos sumos > Sąskaitos faktūros > Atidarytos klientų SF.</span><span class="sxs-lookup"><span data-stu-id="759ae-150">Go to Accounts receivable > Invoices > Open customer invoices.</span></span>
2. <span data-ttu-id="759ae-151">Pažymėkite SF eilutę.</span><span class="sxs-lookup"><span data-stu-id="759ae-151">Mark the line for an invoice.</span></span> <span data-ttu-id="759ae-152">Pvz., pažymėkite eilutę, skirtą CIV-000667.</span><span class="sxs-lookup"><span data-stu-id="759ae-152">For example, mark the line for CIV-000667.</span></span>
3. <span data-ttu-id="759ae-153">Veiksmų srityje spustelėkite Sąskaita faktūra.</span><span class="sxs-lookup"><span data-stu-id="759ae-153">On the Action Pane, click Invoice.</span></span>
4. <span data-ttu-id="759ae-154">Spustelėkite Nurašyti.</span><span class="sxs-lookup"><span data-stu-id="759ae-154">Click Write off.</span></span>
5. <span data-ttu-id="759ae-155">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="759ae-155">Click OK.</span></span>
6. <span data-ttu-id="759ae-156">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-156">Close the page.</span></span>

## <a name="write-off-a-customer-balance-from-the-customer-page"></a><span data-ttu-id="759ae-157">Nurašyti kliento balansą kliento puslapyje</span><span class="sxs-lookup"><span data-stu-id="759ae-157">Write off a customer balance from the customer page</span></span>
1. <span data-ttu-id="759ae-158">Pasirinkite Gautinos sumos > Klientai > Visi klientai.</span><span class="sxs-lookup"><span data-stu-id="759ae-158">Go to Accounts receivable > Customers > All customers.</span></span>
2. <span data-ttu-id="759ae-159">Pasirinkti kliento sąskaitą.</span><span class="sxs-lookup"><span data-stu-id="759ae-159">Select a customer account.</span></span> <span data-ttu-id="759ae-160">Pavyzdžiui, pasirinkite US-001 (Contoso Retail San Diego).</span><span class="sxs-lookup"><span data-stu-id="759ae-160">For example, select US-001 (Contoso Retail San Diego).</span></span>
3. <span data-ttu-id="759ae-161">Veiksmų srityje spustelėkite Rinkti.</span><span class="sxs-lookup"><span data-stu-id="759ae-161">On the Action Pane, click Collect.</span></span>
4. <span data-ttu-id="759ae-162">Spustelėkite Nurašyti.</span><span class="sxs-lookup"><span data-stu-id="759ae-162">Click Write off.</span></span>
5. <span data-ttu-id="759ae-163">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="759ae-163">Click OK.</span></span>
6. <span data-ttu-id="759ae-164">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="759ae-164">Close the page.</span></span>

