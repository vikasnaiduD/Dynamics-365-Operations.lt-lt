--- 
title: "Kurti uždarą klausimą"
description: "Uždari klausimai leidžia suteikti respondentui pasirinkimo variantų."
author: kherr75
manager: AnnBe
ms.date: 06/10/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Operations
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 59f1af68e4b1198894a7cdab291021de9f3cf8a9
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="create-a-closed-ended-question"></a><span data-ttu-id="eda68-103">Kurti uždarą klausimą</span><span class="sxs-lookup"><span data-stu-id="eda68-103">Create a closed ended question</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="eda68-104">Uždari klausimai leidžia suteikti respondentui pasirinkimo variantų.</span><span class="sxs-lookup"><span data-stu-id="eda68-104">Closed-ended questions allow you to provide options for the respondent to choose from.</span></span> <span data-ttu-id="eda68-105">Pirmiausia, turite sukurti atsakymų grupę su atsakymais, tada sukurkite klausimą, kuris naudos atsakymų grupę.</span><span class="sxs-lookup"><span data-stu-id="eda68-105">First, you need to create the Answer group with the answers, then create the question that will use the answer group.</span></span> <span data-ttu-id="eda68-106">Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.</span><span class="sxs-lookup"><span data-stu-id="eda68-106">The demo data company used to create this procedure is USMF.</span></span>


## <a name="create-an-answer-group"></a><span data-ttu-id="eda68-107">Kurti atsakymų grupę</span><span class="sxs-lookup"><span data-stu-id="eda68-107">Create an answer group</span></span>
1. <span data-ttu-id="eda68-108">Eikite į Klausimynas > Kūrimas > Atsakymų grupės.</span><span class="sxs-lookup"><span data-stu-id="eda68-108">Go to Questionnaire > Design > Answer groups.</span></span>
2. <span data-ttu-id="eda68-109">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="eda68-109">Click New.</span></span>
3. <span data-ttu-id="eda68-110">Lauke „Atsakymų grupė“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-110">In the Answer group field, type a value.</span></span>
4. <span data-ttu-id="eda68-111">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-111">In the Description field, type a value.</span></span>
    * <span data-ttu-id="eda68-112">Naudokite funkciją „Atsitiktinė tvarka“, kad atsakymai būtų pateikiami atsitiktinai vis kitokia tvarka kiekvieną kartą, kai klausimui naudojama atsakymų grupė.</span><span class="sxs-lookup"><span data-stu-id="eda68-112">Use the Randomize functionality to randomly place the answers in a different order each time the answer group is used for a question.</span></span>  
5. <span data-ttu-id="eda68-113">Spustelėkite „Atsakyti“.</span><span class="sxs-lookup"><span data-stu-id="eda68-113">Click Answer.</span></span>
6. <span data-ttu-id="eda68-114">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="eda68-114">Click New.</span></span>
    * <span data-ttu-id="eda68-115">Atsakymų rodymo tvarką valdo sekos numeris, nebent atsakymų grupui taikoma „Atsitiktinė tvarka“.</span><span class="sxs-lookup"><span data-stu-id="eda68-115">Sequence number controls the order in which the answers are displayed, unless Randomize is selected for the Answer group.</span></span>  
    * <span data-ttu-id="eda68-116">Klausimynas gali būti vertinamas atsakymams skiriant taškus.</span><span class="sxs-lookup"><span data-stu-id="eda68-116">Points can be awarded to answers for use in scoring the questionnaire.</span></span>  
7. <span data-ttu-id="eda68-117">Lauke „Taškai“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="eda68-117">In the Points field, enter a number.</span></span>
    * <span data-ttu-id="eda68-118">Galima pažymėti teisingą atsakymą parodant, kad pasirinktas atsakymas yra teisingas.</span><span class="sxs-lookup"><span data-stu-id="eda68-118">The correct answer can be marked to indicate that the selected answer is the correct one.</span></span> <span data-ttu-id="eda68-119">Tai gali būti naudojama vertinant klausimyną.</span><span class="sxs-lookup"><span data-stu-id="eda68-119">This can be used for scoring the questionnaire.</span></span>  
8. <span data-ttu-id="eda68-120">Lauke „Atsakymas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-120">In the Answer field, type a value.</span></span>
    * <span data-ttu-id="eda68-121">Toliau kurkite atsakymų pasirinkimo parinktis atsakymų grupei.</span><span class="sxs-lookup"><span data-stu-id="eda68-121">Continue to create answer selection options for the answer group.</span></span>  
9. <span data-ttu-id="eda68-122">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="eda68-122">Click New.</span></span>
10. <span data-ttu-id="eda68-123">Lauke „Taškai“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="eda68-123">In the Points field, enter a number.</span></span>
11. <span data-ttu-id="eda68-124">Lauke „Atsakymas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-124">In the Answer field, type a value.</span></span>
12. <span data-ttu-id="eda68-125">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="eda68-125">Click New.</span></span>
13. <span data-ttu-id="eda68-126">Lauke „Taškai“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="eda68-126">In the Points field, enter a number.</span></span>
14. <span data-ttu-id="eda68-127">Lauke „Atsakymas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-127">In the Answer field, type a value.</span></span>
15. <span data-ttu-id="eda68-128">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="eda68-128">Click New.</span></span>
16. <span data-ttu-id="eda68-129">Lauke „Taškai“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="eda68-129">In the Points field, enter a number.</span></span>
17. <span data-ttu-id="eda68-130">Lauke „Atsakymas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-130">In the Answer field, type a value.</span></span>
18. <span data-ttu-id="eda68-131">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="eda68-131">Click New.</span></span>
19. <span data-ttu-id="eda68-132">Lauke „Taškai“ įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="eda68-132">In the Points field, enter a number.</span></span>
20. <span data-ttu-id="eda68-133">Lauke „Atsakymas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-133">In the Answer field, type a value.</span></span>
21. <span data-ttu-id="eda68-134">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="eda68-134">Close the page.</span></span>
22. <span data-ttu-id="eda68-135">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="eda68-135">Close the page.</span></span>

## <a name="create-the-question"></a><span data-ttu-id="eda68-136">Kurti klausimą</span><span class="sxs-lookup"><span data-stu-id="eda68-136">Create the question</span></span>
1. <span data-ttu-id="eda68-137">Pasirinkite Klausimynas > Kūrimas > Klausimai.</span><span class="sxs-lookup"><span data-stu-id="eda68-137">Go to Questionnaire > Design > Questions.</span></span>
2. <span data-ttu-id="eda68-138">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="eda68-138">Click New.</span></span>
3. <span data-ttu-id="eda68-139">Naudokite lauką „Tipas“, kad sugrupuotumėte susijusius klausimus.</span><span class="sxs-lookup"><span data-stu-id="eda68-139">Use the Type field to group related questions together.</span></span>
    * <span data-ttu-id="eda68-140">Galite naudoti įvesties tipo žymės langelį, alternatyvų mygtuką arba pasirinktinio įvedimo lauką uždariems klausimams.</span><span class="sxs-lookup"><span data-stu-id="eda68-140">You can use input types of Check box, Alternative button, or Combo box for closed-ended questions.</span></span>  
4. <span data-ttu-id="eda68-141">Lauke „Įvesties tipas“ pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="eda68-141">In the Input type field, select an option.</span></span>
5. <span data-ttu-id="eda68-142">Lauke Atsakymų grupė įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-142">In the Answer group field, enter or select a value.</span></span>
6. <span data-ttu-id="eda68-143">Lauke „Tekstas“ įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="eda68-143">In the Text field, type a value.</span></span>

