--- 
title: "Nustatyti akredityvo banko priemones ir registravimo šablonus"
description: "Ši procedūra padeda sukurti banko priemonę ir užregistruoti šabloną, reikalingą norint apdoroti akredityvus."
author: kweekley
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
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: a5c68feeb163e09f183c49afea24d2f9e5999594
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-bank-facilities-and-posting-profiles-for-letter-of-credit"></a><span data-ttu-id="c2fa3-103">Nustatyti akredityvo banko priemones ir registravimo šablonus</span><span class="sxs-lookup"><span data-stu-id="c2fa3-103">Set up bank facilities and posting profiles for letter of credit</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="c2fa3-104">Ši procedūra padeda sukurti banko priemonę ir užregistruoti šabloną, reikalingą norint apdoroti akredityvus.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-104">This procedure walks through creating a Bank facility and posting profile required to process Letters of credit.</span></span> 

<span data-ttu-id="c2fa3-105">Šioje užduotyje naudojama demonstracinė įmonė „USMF‟.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-105">This tasks uses the demo company 'USMF'.</span></span>






## <a name="general-ledger-parameter"></a><span data-ttu-id="c2fa3-106">Didžiosios knygos parametras</span><span class="sxs-lookup"><span data-stu-id="c2fa3-106">General ledger parameter</span></span>
1. <span data-ttu-id="c2fa3-107">Pasirinkite Grynųjų pinigų ir banko valdymas > Nustatymas > Grynųjų pinigų ir banko valdymo parametrai.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-107">Go to Cash and bank management > Setup > Cash and bank management parameters.</span></span>
2. <span data-ttu-id="c2fa3-108">Išplėskite skyrių Banko dokumentas.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-108">Expand the Bank document section.</span></span>
3. <span data-ttu-id="c2fa3-109">Pasirinkite parinktį Įjungti importo akredityvą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-109">Select the Enable import letter of credit option.</span></span>
4. <span data-ttu-id="c2fa3-110">Pasirinkite parinktį Įjungti eksporto akredityvą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-110">Select the Enable export letter of credit option.</span></span>
5. <span data-ttu-id="c2fa3-111">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-111">Click Save.</span></span>
6. <span data-ttu-id="c2fa3-112">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-112">Close the page.</span></span>

## <a name="create-bank-facility"></a><span data-ttu-id="c2fa3-113">Banko priemonės kūrimas</span><span class="sxs-lookup"><span data-stu-id="c2fa3-113">Create Bank facility</span></span>
1. <span data-ttu-id="c2fa3-114">Pasirinkite Grynųjų pinigų ir banko valdymas > Nustatymai > Banko priemonės.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-114">Go to Cash and bank management > Setup > Bank facilities.</span></span>
2. <span data-ttu-id="c2fa3-115">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-115">Click New.</span></span>
3. <span data-ttu-id="c2fa3-116">Lauke Priemonių grupė įveskite banko priemonių grupės pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-116">In the Facility group field, enter the bank facility group name.</span></span>
4. <span data-ttu-id="c2fa3-117">Lauke Aprašas įveskite banko priemonių grupės aprašymą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-117">In the Description field, enter the bank facility group description.</span></span>
5. <span data-ttu-id="c2fa3-118">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-118">Click Save.</span></span>
6. <span data-ttu-id="c2fa3-119">Spustelėkite skirtuką Paslaugų tipai.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-119">Click the Facility types tab.</span></span>
7. <span data-ttu-id="c2fa3-120">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-120">Click New.</span></span>
8. <span data-ttu-id="c2fa3-121">Lauke Paslaugų tipai įveskite unikalų kodą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-121">In the Facility type field, enter a unique code.</span></span>
9. <span data-ttu-id="c2fa3-122">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-122">In the Description field, type a value.</span></span>
10. <span data-ttu-id="c2fa3-123">Lauke Priemonių grupė spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-123">In the Facility group field, click the drop-down button to open the lookup.</span></span>
11. <span data-ttu-id="c2fa3-124">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-124">In the list, find and select the desired record.</span></span>
12. <span data-ttu-id="c2fa3-125">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-125">In the list, click the link in the selected row.</span></span>
13. <span data-ttu-id="c2fa3-126">Lauke Priemonės pobūdis pasirinkite banko priemonės pobūdį.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-126">In the Facility nature field, select the nature of the bank facility.</span></span>
14. <span data-ttu-id="c2fa3-127">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-127">Click Save.</span></span>
15. <span data-ttu-id="c2fa3-128">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-128">Close the page.</span></span>

## <a name="bank-posting-profile"></a><span data-ttu-id="c2fa3-129">Banko registravimo šablonas</span><span class="sxs-lookup"><span data-stu-id="c2fa3-129">Bank posting profile</span></span>
1. <span data-ttu-id="c2fa3-130">Pasirinkite Grynųjų pinigų ir banko valdymas > Nustatymai > Banko dokumentų registravimo šablonas.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-130">Go to Cash and bank management > Setup > Bank documents posting profile.</span></span>
2. <span data-ttu-id="c2fa3-131">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-131">Click New.</span></span>
3. <span data-ttu-id="c2fa3-132">Lauke Sąskaitos / grupės numeris spustelėkite išplečiamąjį mygtuką, kad atidarytumėte peržvalgą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-132">In the Account/Group number field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="c2fa3-133">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-133">In the list, find and select the desired record.</span></span>
5. <span data-ttu-id="c2fa3-134">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-134">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="c2fa3-135">Pasirinkite pagrindinę atsiskaitymo sąskaitą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-135">Select the main account for settlement.</span></span>
    * <span data-ttu-id="c2fa3-136">Ši sąskaita naudojama skaičiuojant grynųjų pinigų srautų prognozę.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-136">This account is used when calculating cash flow forecast.</span></span>  
7. <span data-ttu-id="c2fa3-137">Lauke Išlaidų sąskaita pasirinkite išlaidų operacijų sąskaitą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-137">In the Charges account field, select the account for expense transactions.</span></span>
8. <span data-ttu-id="c2fa3-138">Lauke Maržos sąskaita pasirinkite maržos operacijų sąskaitą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-138">In the Margin account field, select the account for margin transactions.</span></span>
    * <span data-ttu-id="c2fa3-139">Ši sąskaita debetuojama registruojant atidarymo maržą ir kredituojama registruojant mokėjimą.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-139">This account is debited when the opening margin is posted and credited when the payment is posted.</span></span>  
9. <span data-ttu-id="c2fa3-140">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="c2fa3-140">Click Save.</span></span>

