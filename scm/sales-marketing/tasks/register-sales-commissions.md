--- 
title: Registruoti pardavimo komisinius
description: "Ši procedūra nurodo, kaip apskaičiuojami ir registruojami pardavimo komisiniai."
author: omulvad
manager: AnnBe
ms.date: 11/10/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: omulvad
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: f195f9e466eab3cf87afea2b5d430d0ea25c5a83
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="register-sales-commissions"></a><span data-ttu-id="1618e-103">Registruoti pardavimo komisinius</span><span class="sxs-lookup"><span data-stu-id="1618e-103">Register sales commissions</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="1618e-104">Ši procedūra nurodo, kaip apskaičiuojami ir registruojami pardavimo komisiniai.</span><span class="sxs-lookup"><span data-stu-id="1618e-104">This procedure shows you how sales commissions are calculated and registered.</span></span> <span data-ttu-id="1618e-105">Šią procedūrą galite vykdyti demonstracinėje duomenų įmonėje USMF arba su savo duomenimis.</span><span class="sxs-lookup"><span data-stu-id="1618e-105">You can run this procedure in demo data company USMF or on your own data.</span></span> <span data-ttu-id="1618e-106">Prieš paleisdami šį vadovą, paleiskite vadovą pavadinimu „Pardavimo komisinių taisyklių nustatymas“, kad įsitikintumėte, jog turite visus reikalingus komisinių skaičiavimo nustatymus.</span><span class="sxs-lookup"><span data-stu-id="1618e-106">Before starting this guide, run the guide called "Set up sales commission rules" to make sure that you have all the necessary commission calculation setup.</span></span>

<span data-ttu-id="1618e-107">Atkreipkite dėmesį į savo pasirinktus komisinių proceso kliento ir prekės numerius ir naudokite juos, kai šiame vadove jūsų bus paprašyta sukurti pardavimo užsakymą.</span><span class="sxs-lookup"><span data-stu-id="1618e-107">Take note of the customer and item numbers that you have chosen for the commission process and use them when asked to create a sales order in this guide.</span></span>


## <a name="invoice-a-sales-order-that-qualifies-a-salesperson-for-a-commission"></a><span data-ttu-id="1618e-108">Pardavimo užsakymo, suteikiančio pardavėjui teisę gauti komisinius, sąskaitos faktūros išrašymas</span><span class="sxs-lookup"><span data-stu-id="1618e-108">Invoice a sales order that qualifies a salesperson for a commission</span></span>
1. <span data-ttu-id="1618e-109">Eikite į Pardavimas ir rinkodara > Pardavimo užsakymai > Visi pardavimo užsakymai.</span><span class="sxs-lookup"><span data-stu-id="1618e-109">Go to Sales and marketing > Sales orders > All sales orders.</span></span>
2. <span data-ttu-id="1618e-110">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="1618e-110">Click New.</span></span>
3. <span data-ttu-id="1618e-111">Lauke Kliento sąskaita spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="1618e-111">In the Customer account field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="1618e-112">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="1618e-112">In the list, find and select the desired record.</span></span>
5. <span data-ttu-id="1618e-113">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="1618e-113">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="1618e-114">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="1618e-114">Click OK.</span></span>
7. <span data-ttu-id="1618e-115">Veiksmų srityje spustelėkite Parinktys.</span><span class="sxs-lookup"><span data-stu-id="1618e-115">On the Action Pane, click Options.</span></span>
8. <span data-ttu-id="1618e-116">Spustelėkite Keisti rodinį.</span><span class="sxs-lookup"><span data-stu-id="1618e-116">Click Change view.</span></span>
9. <span data-ttu-id="1618e-117">Spustelėkite antraštės rodinį.</span><span class="sxs-lookup"><span data-stu-id="1618e-117">Click Header view.</span></span>
10. <span data-ttu-id="1618e-118">Išplėskite skyrių Nustatymas.</span><span class="sxs-lookup"><span data-stu-id="1618e-118">Expand the Setup section.</span></span>
    * <span data-ttu-id="1618e-119">Lauko Pardavimo grupė reikšmė nurodo grupę, kuriai priskirtas vienas ar keli pardavimo atstovai.</span><span class="sxs-lookup"><span data-stu-id="1618e-119">The value in the Sales group field represents a group with one or more sales representatives assigned to it.</span></span> <span data-ttu-id="1618e-120">Grupėje esantys žmonės išrašius užsakymo sąskaitą faktūrą gaus komisinius pagal iš anksto nustatytus tarifus ir paskirstymą.</span><span class="sxs-lookup"><span data-stu-id="1618e-120">The people in the group are the ones who will receive commissions when the order is invoiced, as per predefined rates and distribution.</span></span>   <span data-ttu-id="1618e-121">Reikšmė kopijuojama iš dalies Kliento kortelė, tačiau, jei norite, galite ją pakeisti.</span><span class="sxs-lookup"><span data-stu-id="1618e-121">The value is copied from the Customer card, but you can change it if you wish.</span></span>  <span data-ttu-id="1618e-122">Pardavimo grupė taip pat nukopijuojama į pardavimo užsakymo eilutę.</span><span class="sxs-lookup"><span data-stu-id="1618e-122">The Sales group is also copied to the sales order line.</span></span> <span data-ttu-id="1618e-123">Galite ją pakeisti, kad ji skirtųsi nuo antraštėje ir (arba) tarp eilučių nurodytos grupės.</span><span class="sxs-lookup"><span data-stu-id="1618e-123">You can change it so that it can differ from the one in the header and/or between lines.</span></span>  
    * <span data-ttu-id="1618e-124">Lauko Komisinių grupė reikšmė nurodo grupę, kurią sukūrėte vienam ar keliems klientams norėdami sekti komisinius.</span><span class="sxs-lookup"><span data-stu-id="1618e-124">The value in the Commission group field represents a group that you have created for one or more customers with the purpose of tracking commissions.</span></span>   <span data-ttu-id="1618e-125">Reikšmė kopijuojama iš dalies Kliento kortelė, tačiau, jei norite, galite ją pakeisti.</span><span class="sxs-lookup"><span data-stu-id="1618e-125">The value is copied from the Customer card, but you can change it if you wish.</span></span>   
11. <span data-ttu-id="1618e-126">Veiksmų srityje spustelėkite Parinktys.</span><span class="sxs-lookup"><span data-stu-id="1618e-126">On the Action Pane, click Options.</span></span>
12. <span data-ttu-id="1618e-127">Spustelėkite Keisti rodinį.</span><span class="sxs-lookup"><span data-stu-id="1618e-127">Click Change view.</span></span>
13. <span data-ttu-id="1618e-128">Spustelėkite Eilutės rodinys.</span><span class="sxs-lookup"><span data-stu-id="1618e-128">Click Line view.</span></span>
14. <span data-ttu-id="1618e-129">Lauke Prekės numeris spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="1618e-129">In the Item number field, click the drop-down button to open the lookup.</span></span>
15. <span data-ttu-id="1618e-130">Sąraše pasirinkite nustatytą komisinių prekę.</span><span class="sxs-lookup"><span data-stu-id="1618e-130">In the list, select the item you have set up for commissions.</span></span> 
16. <span data-ttu-id="1618e-131">Lauke Kiekis įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="1618e-131">In the Quantity field, enter a number.</span></span>
    * <span data-ttu-id="1618e-132">Atkreipkite dėmesį į eilutės dalį Grynoji suma.</span><span class="sxs-lookup"><span data-stu-id="1618e-132">Take note of the line's Net amount.</span></span> <span data-ttu-id="1618e-133">Joje nurodomos pardavimo įplaukos, kurios, šiuo atveju, yra komisinių skaičiavimo pagrindas.</span><span class="sxs-lookup"><span data-stu-id="1618e-133">It represents the sales revenue, which in this example is the basis for commission calculation.</span></span>  
17. <span data-ttu-id="1618e-134">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="1618e-134">Click Save.</span></span>
18. <span data-ttu-id="1618e-135">Veiksmų srityje spustelėkite Sąskaita faktūra.</span><span class="sxs-lookup"><span data-stu-id="1618e-135">On the Action Pane, click Invoice.</span></span>
19. <span data-ttu-id="1618e-136">Spustelėkite Sąskaita faktūra.</span><span class="sxs-lookup"><span data-stu-id="1618e-136">Click Invoice.</span></span>
20. <span data-ttu-id="1618e-137">Išplėskite skyrių Parametrai.</span><span class="sxs-lookup"><span data-stu-id="1618e-137">Expand the Parameters section.</span></span>
21. <span data-ttu-id="1618e-138">Lauke Kiekis pasirinkite Visi.</span><span class="sxs-lookup"><span data-stu-id="1618e-138">In the Quantity field, select 'All'.</span></span>
22. <span data-ttu-id="1618e-139">Lauke Registravimas pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="1618e-139">Select Yes in the Posting field.</span></span>
23. <span data-ttu-id="1618e-140">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="1618e-140">Click OK.</span></span>
24. <span data-ttu-id="1618e-141">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="1618e-141">Click OK.</span></span>
    * <span data-ttu-id="1618e-142">Operacijos registravimas gali užtrukti apie minutę.</span><span class="sxs-lookup"><span data-stu-id="1618e-142">It may take a minute or so to post the transaction.</span></span> <span data-ttu-id="1618e-143">Palaukite, kol apdorojimas baigsis ir neuždarykite puslapio.</span><span class="sxs-lookup"><span data-stu-id="1618e-143">Allow the processing to complete and don’t close the page.</span></span>  

## <a name="review-the-registered-sales-commissions"></a><span data-ttu-id="1618e-144">Registruotų pardavimo komisinių peržiūra</span><span class="sxs-lookup"><span data-stu-id="1618e-144">Review the registered sales commissions</span></span>
1. <span data-ttu-id="1618e-145">Veiksmų srityje spustelėkite Sąskaita faktūra.</span><span class="sxs-lookup"><span data-stu-id="1618e-145">On the Action Pane, click Invoice.</span></span>
2. <span data-ttu-id="1618e-146">Spustelėkite Sąskaita faktūra.</span><span class="sxs-lookup"><span data-stu-id="1618e-146">Click Invoice.</span></span>
3. <span data-ttu-id="1618e-147">Veiksmų srityje spustelėkite Sąskaita faktūra.</span><span class="sxs-lookup"><span data-stu-id="1618e-147">On the Action Pane, click Invoice.</span></span>
4. <span data-ttu-id="1618e-148">Spustelėkite Komisinių operacijos.</span><span class="sxs-lookup"><span data-stu-id="1618e-148">Click Commission transactions.</span></span>
    * <span data-ttu-id="1618e-149">Skirtuke Peržiūra rodomos eilutės, kuriose nurodomos su sąskaitą faktūrą turinčiu pardavimo užsakymu susietiems pardavimo atstovams mokėtinos komisinių sumos.</span><span class="sxs-lookup"><span data-stu-id="1618e-149">The Overview tab displays lines representing the commission amounts payable to sales representatives who are associated with the invoiced sales order.</span></span> <span data-ttu-id="1618e-150">Peržiūrėkime išsamią informaciją.</span><span class="sxs-lookup"><span data-stu-id="1618e-150">Let's review the details.</span></span>     
    * <span data-ttu-id="1618e-151">Jei nustatydami komisinių pardavimo grupę naudojote vadovą „Pardavimo komisinių taisyklių nustatymas“, pardavimo komisinius gali gauti du pardavėjai ir komisiniai padalinami jiems po lygiai.</span><span class="sxs-lookup"><span data-stu-id="1618e-151">If you used the "Set up sales commission rules" guide to set up the Commission sales group, there are two sales people to receive a sales commissions, and the commission is split equally between them.</span></span>  
    * <span data-ttu-id="1618e-152">Šiame pavyzdyje komisinių suma apskaičiuojama kaip pardavimo įplaukų procentinė dalis (užsakymo eilutės grynoji suma).</span><span class="sxs-lookup"><span data-stu-id="1618e-152">In this example, the total amount of the commission is calculated as a percentage of the sales revenue (the net amount of order line).</span></span>   
5. <span data-ttu-id="1618e-153">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="1618e-153">Close the page.</span></span>
6. <span data-ttu-id="1618e-154">Spustelėkite Kvitas.</span><span class="sxs-lookup"><span data-stu-id="1618e-154">Click Voucher.</span></span>
    * <span data-ttu-id="1618e-155">Galite peržiūrėti komisinių sumų, kurios užregistruotos iš anksto numatytų komisinių išlaidų ir mokėtinų komisinių sąskaitose, kvitų operacijas.</span><span class="sxs-lookup"><span data-stu-id="1618e-155">You can review the voucher transactions for the commission amounts that have been posted to the predefined commission expense and commission payable accounts.</span></span>  

