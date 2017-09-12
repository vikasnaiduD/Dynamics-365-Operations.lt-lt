--- 
title: "Išjungti gamybos eigos versiją"
description: "Kai aktyvi gamybos eigos versija nebereikalinga, galite jį išjungti."
author: cvocph
manager: AnnBe
ms.date: 10/07/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: yuyus
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: conradv
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 8db4b2857e9a7c99ee6fa4ef397f7ed99335faba
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="deactivate-a-production-flow-version"></a><span data-ttu-id="9f0c8-103">Išjungti gamybos eigos versiją</span><span class="sxs-lookup"><span data-stu-id="9f0c8-103">Deactivate a production flow version</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="9f0c8-104">Kai aktyvi gamybos eigos versija nebereikalinga, galite jį išjungti.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-104">When an active production flow version is no longer needed, it can be deactivated.</span></span> <span data-ttu-id="9f0c8-105">Turėtumėte šią parinktį naudoti tik jei visos „kanban“ taisyklės ir veiklos yra baigtos ir nebus vėl suaktyvintos.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-105">You should only use this option if all kanban rules and activities have ended and will not be activated again.</span></span> <span data-ttu-id="9f0c8-106">Atkreipkite dėmesį, kad visų su šia gamybos versija susijusių „kanban“ taisyklių galiojimo data bus atnaujinta į dabartinę datą ir laiką.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-106">Note that the expiry date of all kanban rules related to this production flow version will be updated with the current date and time.</span></span> 

<span data-ttu-id="9f0c8-107">Norėdami keisti aktyvią gamybos eigos versiją, galite nustatyti aktyvios versijos galiojimo datą ir sukurti naują versiją.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-107">To modify an active production flow version, consider setting an expiry date for the active version and create a new version.</span></span> <span data-ttu-id="9f0c8-108">Tokiu būdu galėsite tęsti gamybos operacijas, tuo pat metu ruošdami naują versiją ir susijusias „kanban“ taisykles.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-108">This will allow you to continue your production operations while preparing the new version and related kanban rules.</span></span> 

<span data-ttu-id="9f0c8-109">Norėdami, kad baigtų galioti aktyvi gamybos eigos versija, turite nustatyti galiojimo datą.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-109">To expire an active production flow version, you need to set an expiry date.</span></span> <span data-ttu-id="9f0c8-110">Šia prasme išjungimas yra daugiau išimtis negu taisyklė.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-110">In that sense, deactivation is more like an exception than a rule.</span></span> 

<span data-ttu-id="9f0c8-111">Šiai procedūrai atlikti reikalinga gamybos eiga, kurios versiją galima išjungti.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-111">For this procedure you need a production flow with a version that can be deactivated.</span></span> <span data-ttu-id="9f0c8-112">Nebandykite to atlikti gamybos aplinkoje, nebent esate 100 % tikri, kad versija yra visiškai pasenusi.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-112">Do not try this in a production environment unless you are 100% positive that the version is fully obsolete.</span></span>


## <a name="deactivate-a-production-flow-version"></a><span data-ttu-id="9f0c8-113">Išjungti gamybos eigos versiją</span><span class="sxs-lookup"><span data-stu-id="9f0c8-113">Deactivate a production flow version</span></span>
1. <span data-ttu-id="9f0c8-114">Pasirinkite Gamybos kontrolė > Nustatymai > „Lean“ gamybos eiga > Gamybos eigos.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-114">Go to Production control > Setup > Lean production flow > Production flows.</span></span>
2. <span data-ttu-id="9f0c8-115">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-115">In the list, find and select the desired record.</span></span>
3. <span data-ttu-id="9f0c8-116">Sąraše spustelėkite saitą pasirinktoje eilutėje.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-116">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="9f0c8-117">Sąraše raskite ir pasirinkite norimą įrašą.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-117">In the list, find and select the desired record.</span></span>
5. <span data-ttu-id="9f0c8-118">Spustelėkite Išjungti.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-118">Click Deactivate.</span></span>
    * <span data-ttu-id="9f0c8-119">Tęskite tik jei esate 100 % tikri, kad ši gamybos eigos versija yra pasenusi.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-119">Do not proceed if you are not 100% positive that this production flow version is obsolete.</span></span> <span data-ttu-id="9f0c8-120">Spustelėjus Gerai nustos galioti visos aktyvios „kanban“ taisyklės ir nedelsiant bus sustabdytos visos šios gamybos eigos versijos gamybos ir papildymo veiklos.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-120">Clicking Ok will expire all active kanban rules and put an immediate stop to all production and replenishment activities of this production flow version.</span></span>  
6. <span data-ttu-id="9f0c8-121">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="9f0c8-121">Click OK.</span></span>

