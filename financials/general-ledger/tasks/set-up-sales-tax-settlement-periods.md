--- 
title: Nustatyti PVM sudengimo laikotarpius
description: "PVM sudengimo laikotarpiuose pateikiama informacija apie laikotarpių intervalus, už kuriuos reikia pranešti apie PVM ir jį sumokėti."
author: twheeloc
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
ms.author: vstehman
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 4d65dee3bd059966458cb9603807de85b704fc49
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-sales-tax-settlement-periods"></a><span data-ttu-id="17a3d-103">Nustatyti PVM sudengimo laikotarpius</span><span class="sxs-lookup"><span data-stu-id="17a3d-103">Set up sales tax settlement periods</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="17a3d-104">PVM sudengimo laikotarpiuose pateikiama informacija apie laikotarpių intervalus, už kuriuos reikia pranešti apie PVM ir jį sumokėti.</span><span class="sxs-lookup"><span data-stu-id="17a3d-104">Sales tax settlement periods contain information about the period intervals for which sales tax needs to be reported and paid.</span></span> <span data-ttu-id="17a3d-105">Galima vykdyti konkrečios datos intervalo sudengimo laikotarpio procesą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-105">A settlement process can be run for a settlement period for a specific date interval.</span></span> <span data-ttu-id="17a3d-106">Bus sudengti visi mokesčių kodai, susieti su sudengimo laikotarpiu.</span><span class="sxs-lookup"><span data-stu-id="17a3d-106">All tax codes associated with the settlement period will be settled.</span></span> <span data-ttu-id="17a3d-107">Atsižvelgiant į susijusios PVM institucijos sąranką, mokestiniai įsipareigojimai registruojami arba tiekėjui, arba DK sąskaitoje.</span><span class="sxs-lookup"><span data-stu-id="17a3d-107">Depending on the set up of the related Sales tax authority, the tax liability is posted either to a vendor or a General ledger account.</span></span>



<span data-ttu-id="17a3d-108">Šioje užduotyje naudojama demonstracinė įmonė USMF.</span><span class="sxs-lookup"><span data-stu-id="17a3d-108">This task uses the USMF demo company.</span></span>



1. <span data-ttu-id="17a3d-109">Pasirinkite Mokestis > Netiesioginiai mokesčiai > PVM > PVM sudengimo laikotarpiai.</span><span class="sxs-lookup"><span data-stu-id="17a3d-109">Go to Tax > Indirect taxes > Sales tax > Sales tax settlement periods.</span></span>
2. <span data-ttu-id="17a3d-110">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="17a3d-110">Click New.</span></span>
3. <span data-ttu-id="17a3d-111">Lauke Sudengimo laikotarpis surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="17a3d-111">In the Settlement period field, type a value.</span></span>
4. <span data-ttu-id="17a3d-112">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="17a3d-112">In the Description field, type a value.</span></span>
5. <span data-ttu-id="17a3d-113">Lauke Institucija pasirinkite PVM instituciją, kuri gauna ataskaitas ir mokėjimus, sukurtus už sudengimo laikotarpį.</span><span class="sxs-lookup"><span data-stu-id="17a3d-113">In the Authority field, select the sales tax authority that receives the reports and the payments that are created for the settlement period.</span></span>
6. <span data-ttu-id="17a3d-114">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-114">In the list, find and select the desired record.</span></span>
7. <span data-ttu-id="17a3d-115">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="17a3d-115">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="17a3d-116">Lauke Mokėjimo sąlygos spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-116">In the Terms of payment field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="17a3d-117">Susijusią PVM instituciją galima nustatyti kaip tiekėją ir, sudengiant PVM, bus sukurta atidaryta tiekėjo SF.</span><span class="sxs-lookup"><span data-stu-id="17a3d-117">The related Sales tax authority can be set up as a vendor and the Sales tax settlement will create an open vendor invoice.</span></span> <span data-ttu-id="17a3d-118">Mokėjimo sąlygos apibrėžia atidarytos tiekėjo SF terminą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-118">The Terms of payment defines the Due date for the open vendor invoice.</span></span>  
9. <span data-ttu-id="17a3d-119">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-119">In the list, find and select the desired record.</span></span>
10. <span data-ttu-id="17a3d-120">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="17a3d-120">In the list, click the link in the selected row.</span></span>
11. <span data-ttu-id="17a3d-121">Pasirinkite sudengimo laikotarpių intervalų tipą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-121">Select a type for the settlement period intervals.</span></span>
12. <span data-ttu-id="17a3d-122">Įveskite laikotarpio intervalo vienetų skaičių vienam laikotarpiui.</span><span class="sxs-lookup"><span data-stu-id="17a3d-122">Enter the number of Period interval units per period.</span></span> <span data-ttu-id="17a3d-123">Pavyzdžiui, ketvirtį sudaro 3 mėnesiai.</span><span class="sxs-lookup"><span data-stu-id="17a3d-123">For example, a quarter has 3 months.</span></span>
13. <span data-ttu-id="17a3d-124">Pažymėkite arba atžymėkite žymės langelį Sudengiant PVM naudoti paketinį apdorojimą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-124">Select or clear the Use batch processing for sales tax settlement check box.</span></span>
    * <span data-ttu-id="17a3d-125">Sudengimo laikotarpio procesą galima apdoroti kaip paketinę užduotį fone.</span><span class="sxs-lookup"><span data-stu-id="17a3d-125">The settlement process for the settlement period can be processed as batch job in the background.</span></span> <span data-ttu-id="17a3d-126">Tai rekomenduojama atlikti su daug mokesčių operacijų, patenkančių į laikotarpio intervalą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-126">This is recommended for a large number of tax transactions within a period interval.</span></span>  
14. <span data-ttu-id="17a3d-127">Išplėskite skirtuką Laikotarpio intervalai.</span><span class="sxs-lookup"><span data-stu-id="17a3d-127">Expand the Period intervals tab.</span></span>
15. <span data-ttu-id="17a3d-128">Spustelėkite Pridėti.</span><span class="sxs-lookup"><span data-stu-id="17a3d-128">Click Add.</span></span>
16. <span data-ttu-id="17a3d-129">Sąraše pažymėkite pasirinktą eilutę.</span><span class="sxs-lookup"><span data-stu-id="17a3d-129">In the list, mark the selected row.</span></span>
17. <span data-ttu-id="17a3d-130">Lauke Pradžios data įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-130">In the From date field, enter a date.</span></span>
18. <span data-ttu-id="17a3d-131">Lauke Pabaigos data įveskite datą.</span><span class="sxs-lookup"><span data-stu-id="17a3d-131">In the To date field, enter a date.</span></span>
19. <span data-ttu-id="17a3d-132">Spustelėkite Naujas laikotarpio intervalas.</span><span class="sxs-lookup"><span data-stu-id="17a3d-132">Click New period interval.</span></span>
    * <span data-ttu-id="17a3d-133">Įvedus pirmąjį laikotarpio intervalą, galima automatiškai kurti naujus laikotarpius.</span><span class="sxs-lookup"><span data-stu-id="17a3d-133">Once the first period interval has been entered, new periods can be created automatically.</span></span> <span data-ttu-id="17a3d-134">Jei reikia, galite grįžti ir pridėti naujų laikotarpių intervalų.</span><span class="sxs-lookup"><span data-stu-id="17a3d-134">You can come back and add new period intervals as required.</span></span>  
20. <span data-ttu-id="17a3d-135">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="17a3d-135">Close the page.</span></span>

