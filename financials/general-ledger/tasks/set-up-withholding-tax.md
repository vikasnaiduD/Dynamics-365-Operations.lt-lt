--- 
title: "Nustatyti išskaitomą mokestį"
description: "Išskaitomas mokestis yra tiekėjams taikomas mokestis, kurį taikant nesukuriama PVM operacijų."
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
ms.openlocfilehash: dc4c0745235052cb4145bc7083fef1a88c8bb5c9
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-withholding-tax"></a><span data-ttu-id="9d914-103">Nustatyti išskaitomą mokestį</span><span class="sxs-lookup"><span data-stu-id="9d914-103">Set up withholding tax</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="9d914-104">Išskaitomas mokestis yra tiekėjams taikomas mokestis, kurį taikant nesukuriama PVM operacijų.</span><span class="sxs-lookup"><span data-stu-id="9d914-104">Withholding tax is a tax on vendors that does not create sales tax transactions.</span></span> <span data-ttu-id="9d914-105">Tiekėjas įsipareigoja sumokėti jo mokėjimams priskiriamą išskaitomą mokestį.</span><span class="sxs-lookup"><span data-stu-id="9d914-105">Withholding tax that is calculated on vendor payments is a liability.</span></span> <span data-ttu-id="9d914-106">Todėl išskaitomą mokestį galima registruoti tik balanso arba įsipareigojimų sąskaitose.</span><span class="sxs-lookup"><span data-stu-id="9d914-106">Therefore, only balance sheet accounts or liability accounts are valid accounts for posting withholding tax.</span></span> <span data-ttu-id="9d914-107">Šis užduočių vadovas parodo, kaip nustatyti išskaitomą mokestį.</span><span class="sxs-lookup"><span data-stu-id="9d914-107">This task guide demonstrates how to set up withholding tax.</span></span>

1. <span data-ttu-id="9d914-108">Pasirinkite Mokestis > Netiesioginiai mokesčiai > Išskaitomas mokestis > Išskaitomo mokesčio kodai.</span><span class="sxs-lookup"><span data-stu-id="9d914-108">Go to Tax > Indirect taxes > Withholding tax > Withholding tax codes.</span></span>
2. <span data-ttu-id="9d914-109">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="9d914-109">Click New.</span></span>
3. <span data-ttu-id="9d914-110">Lauke Išskaitomo mokesčio kodas surinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="9d914-110">In the Withholding tax code field, type a value.</span></span>
4. <span data-ttu-id="9d914-111">Lauke Išskaitomo mokesčio pavadinimas įveskite išskaitomo mokesčio kodo pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="9d914-111">In the Withholding tax name field, enter the name of the withholding tax code.</span></span>
5. <span data-ttu-id="9d914-112">Lauke Pagrindinė sąskaita pasirinkite pagrindinę sąskaitą, kurioje registruoti išskaitomo mokesčio įsipareigojimus.</span><span class="sxs-lookup"><span data-stu-id="9d914-112">In the Main account field, select the main account for posting the withholding tax liability.</span></span>
6. <span data-ttu-id="9d914-113">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="9d914-113">Click Save.</span></span>
7. <span data-ttu-id="9d914-114">Spustelėkite Reikšmės.</span><span class="sxs-lookup"><span data-stu-id="9d914-114">Click Values.</span></span>
8. <span data-ttu-id="9d914-115">Sąraše pažymėkite pasirinktą eilutę.</span><span class="sxs-lookup"><span data-stu-id="9d914-115">In the list, mark the selected row.</span></span>
9. <span data-ttu-id="9d914-116">Lauke Reikšmė įveskite procentinę dalį, naudojamą skaičiuoti išskaitomam mokesčiui.</span><span class="sxs-lookup"><span data-stu-id="9d914-116">In the Value field, enter a percentage used for the calculation of the withholding tax.</span></span>
10. <span data-ttu-id="9d914-117">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="9d914-117">Click Save.</span></span>
11. <span data-ttu-id="9d914-118">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="9d914-118">Close the page.</span></span>
12. <span data-ttu-id="9d914-119">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="9d914-119">Click Save.</span></span>
13. <span data-ttu-id="9d914-120">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="9d914-120">Close the page.</span></span>
14. <span data-ttu-id="9d914-121">Pasirinkite Mokestis > Netiesioginiai mokesčiai > Išskaitomas mokestis > Išskaitomo mokesčio grupės.</span><span class="sxs-lookup"><span data-stu-id="9d914-121">Go to Tax > Indirect taxes > Withholding tax > Withholding tax groups.</span></span>
15. <span data-ttu-id="9d914-122">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="9d914-122">Click New.</span></span>
16. <span data-ttu-id="9d914-123">Lauke Išskaitomo mokesčio grupė įveskite išskaitomo mokesčio grupės identifikatorių.</span><span class="sxs-lookup"><span data-stu-id="9d914-123">In the Withholding tax group field, enter the identifier of the withholding tax group.</span></span>
17. <span data-ttu-id="9d914-124">Lauke Aprašas įveskite išskaitomo mokesčio grupės pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="9d914-124">In the Description field, enter the name of the withholding tax group.</span></span>
18. <span data-ttu-id="9d914-125">Sąraše pažymėkite pasirinktą eilutę.</span><span class="sxs-lookup"><span data-stu-id="9d914-125">In the list, mark the selected row.</span></span>
19. <span data-ttu-id="9d914-126">Lauke Išskaitomo mokesčio kodas pasirinkite išskaitomo mokesčio kodą.</span><span class="sxs-lookup"><span data-stu-id="9d914-126">In the Withholding tax code field, select the withholding tax code.</span></span>
20. <span data-ttu-id="9d914-127">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="9d914-127">In the list, click the link in the selected row.</span></span>
21. <span data-ttu-id="9d914-128">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="9d914-128">Click Save.</span></span>

