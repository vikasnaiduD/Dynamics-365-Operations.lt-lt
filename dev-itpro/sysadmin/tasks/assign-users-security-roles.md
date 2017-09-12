--- 
title: "Vartotojų priskyrimas saugos vaidmenims"
description: "Norėdami pasiekti „Microsoft Dynamics 365 for Finance and Operations“, „Enterprise“ leidimą, vartotojams turi būti priskirti saugos vaidmenys."
author: maertenm
manager: AnnBe
ms.date: 06/07/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: sericks
ms.search.scope: Operations
ms.search.region: Global
ms.author: maertenm
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 551048af26f46d334c562d1968963aed262a5e03
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="assign-users-to-security-roles"></a><span data-ttu-id="301d1-103">Vartotojų priskyrimas saugos vaidmenims</span><span class="sxs-lookup"><span data-stu-id="301d1-103">Assign users to security roles</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="301d1-104">Norėdami pasiekti „Microsoft Dynamics 365 for Finance and Operations“, „Enterprise“ leidimą, vartotojams turi būti priskirti saugos vaidmenys.</span><span class="sxs-lookup"><span data-stu-id="301d1-104">To access Microsoft Dynamics 365 for Finance and Operations, Enterprise edition, users must be assigned to security roles.</span></span> <span data-ttu-id="301d1-105">Šia procedūra paaiškinama, kaip sistemos administratoriai gali automatiškai pagal verslo duomenis priskirti vartotojus.</span><span class="sxs-lookup"><span data-stu-id="301d1-105">This procedure explains how system administrators can assign users to roles automatically, based on business data.</span></span> <span data-ttu-id="301d1-106">Kuriant šią procedūrą naudojama demonstracinių duomenų įmonė yra USMF.</span><span class="sxs-lookup"><span data-stu-id="301d1-106">The demo data company used to create this procedure is USMF.</span></span>


## <a name="automatically-assign-users-to-roles"></a><span data-ttu-id="301d1-107">Automatinis vartotojų priskyrimas vaidmenims</span><span class="sxs-lookup"><span data-stu-id="301d1-107">Automatically assign users to roles</span></span>
1. <span data-ttu-id="301d1-108">Eikite į Sistemos administravimas > Sauga > Priskirti vartotojus vaidmenims.</span><span class="sxs-lookup"><span data-stu-id="301d1-108">Go to System administration > Security > Assign users to roles.</span></span>
2. <span data-ttu-id="301d1-109">Medyje pasirinkite Apskaitos prižiūrėtojas.</span><span class="sxs-lookup"><span data-stu-id="301d1-109">In the tree, select 'Accounting supervisor'.</span></span>
    * <span data-ttu-id="301d1-110">Pasirinkite vaidmenį, kurio taisyklę norite sukonfigūruoti.</span><span class="sxs-lookup"><span data-stu-id="301d1-110">Select the role that you want to configure the rule for.</span></span> <span data-ttu-id="301d1-111">Šiame pavyzdyje pasirinkite Apskaitos prižiūrėtojas.</span><span class="sxs-lookup"><span data-stu-id="301d1-111">In this example, select Accounting supervisor.</span></span>  
3. <span data-ttu-id="301d1-112">Spustelėkite Įtraukti taisyklę, kad atidarytumėte išplečiamąjį dialogo langą.</span><span class="sxs-lookup"><span data-stu-id="301d1-112">Click Add rule to open the drop dialog.</span></span>
4. <span data-ttu-id="301d1-113">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="301d1-113">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="301d1-114">Pasirinkite su šia taisykle naudotiną užklausą.</span><span class="sxs-lookup"><span data-stu-id="301d1-114">Select the query to use for this rule.</span></span>  
5. <span data-ttu-id="301d1-115">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="301d1-115">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="301d1-116">Spustelėkite Redaguoti užklausą.</span><span class="sxs-lookup"><span data-stu-id="301d1-116">Click Edit query.</span></span>
    * <span data-ttu-id="301d1-117">Pagal poreikį užklausą redaguokite.</span><span class="sxs-lookup"><span data-stu-id="301d1-117">Edit the query, as needed.</span></span>  
7. <span data-ttu-id="301d1-118">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="301d1-118">Click OK.</span></span>

## <a name="exclude-users-from-automatic-role-assignment"></a><span data-ttu-id="301d1-119">Vartotojų šalinimas iš automatinio vaidmenų priskyrimo</span><span class="sxs-lookup"><span data-stu-id="301d1-119">Exclude users from automatic role assignment</span></span>
1. <span data-ttu-id="301d1-120">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="301d1-120">Close the page.</span></span>
2. <span data-ttu-id="301d1-121">Eikite į Sistemos administravimas > Sauga > Priskirti vartotojus vaidmenims.</span><span class="sxs-lookup"><span data-stu-id="301d1-121">Go to System administration > Security > Assign users to roles.</span></span>
3. <span data-ttu-id="301d1-122">Medyje pasirinkite Apskaitos prižiūrėtojas.</span><span class="sxs-lookup"><span data-stu-id="301d1-122">In the tree, select 'Accounting supervisor'.</span></span>
    * <span data-ttu-id="301d1-123">Pasirinkite vaidmenį.</span><span class="sxs-lookup"><span data-stu-id="301d1-123">Select a role.</span></span> <span data-ttu-id="301d1-124">Šiam pavyzdžiui pasirinkite Apskaitos prižiūrėtojas.</span><span class="sxs-lookup"><span data-stu-id="301d1-124">For this example, select Accounting supervisor.</span></span>  
4. <span data-ttu-id="301d1-125">Spustelėkite Rankiniu būdu priskirti / pašalinti vartotojus.</span><span class="sxs-lookup"><span data-stu-id="301d1-125">Click Manually assign / exclude users.</span></span>
5. <span data-ttu-id="301d1-126">Sąraše pažymėkite pasirinktą eilutę.</span><span class="sxs-lookup"><span data-stu-id="301d1-126">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="301d1-127">Pasirinkite vartotoją.</span><span class="sxs-lookup"><span data-stu-id="301d1-127">Select a user.</span></span>  
6. <span data-ttu-id="301d1-128">Spustelėkite Pašalinti iš vaidmens.</span><span class="sxs-lookup"><span data-stu-id="301d1-128">Click Exclude from role.</span></span>
    * <span data-ttu-id="301d1-129">Spustelėkite Pašalinti iš vaidmens, kad pasirinktus vartotojus pašalintumėte iš vaidmens.</span><span class="sxs-lookup"><span data-stu-id="301d1-129">Click Exclude from role to exclude the selected users from the role.</span></span> <span data-ttu-id="301d1-130">Norėdami pašalinti pašalinimus, pasirinkite vartotojus, kurių pašalinimus norite pašalinti ir spustelėkite Grąžinti būseną.</span><span class="sxs-lookup"><span data-stu-id="301d1-130">To remove exclusions, select the users that you want to remove exclusions for, and then click Reset status.</span></span> <span data-ttu-id="301d1-131">Kai pašalinate pašalinimą grąžindami vartotojo būseną, vartotojo vaidmuo vėl priskiriamas automatiškai.</span><span class="sxs-lookup"><span data-stu-id="301d1-131">When you remove an exclusion by resetting the user’s status, the user’s role is again assigned automatically.</span></span> <span data-ttu-id="301d1-132">Tačiau, grąžinus būseną, vartotojas ne iš kato priskiriamas vaidmeniui ar iš vaidmens pašalinamas.</span><span class="sxs-lookup"><span data-stu-id="301d1-132">However, the user is not immediately assigned to the role or excluded from the role when you reset the status.</span></span> <span data-ttu-id="301d1-133">Vartotojas vaidmeniui priskiriamas arba iš vaidmens pašalinamas kitą kartą vykdant automatinio vaidmenų priskyrimo taisykles.</span><span class="sxs-lookup"><span data-stu-id="301d1-133">Instead, the user is either assigned to the role or removed from the role the next time that the rules for automatic role assignment are run.</span></span>  

