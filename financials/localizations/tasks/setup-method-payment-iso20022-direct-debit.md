--- 
title: "ISO20022 tiesioginio debeto mokėjimo būdo nustatymas"
description: "Šioje procedūroje parodoma, kaip nustatyti kliento mokėjimo būdą, skirtą atlikti ISO20022 tiesioginio debeto arba bet kokio kito tipo mokėjimą, naudojant elektronines ataskaitas."
author: mrolecki
manager: AnnBe
ms.date: 10/13/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 57c184d5b8f6b42f738142e4f448aafe6225dcb0
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-method-of-payment-for-iso20022-direct-debit"></a><span data-ttu-id="9af4a-103">ISO20022 tiesioginio debeto mokėjimo būdo nustatymas</span><span class="sxs-lookup"><span data-stu-id="9af4a-103">Set up method of payment for ISO20022 direct debit</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="9af4a-104">Šioje procedūroje parodoma, kaip nustatyti kliento mokėjimo būdą, skirtą atlikti ISO20022 tiesioginio debeto arba bet kokio kito tipo mokėjimą, naudojant elektronines ataskaitas.</span><span class="sxs-lookup"><span data-stu-id="9af4a-104">This procedure shows how to set up the customer method of payment for ISO20022 direct debit or any other payment type using electronic reporting.</span></span> 



<span data-ttu-id="9af4a-105">Prieš atlikdami šią užduotį, turite nustatyti eksporto formato konfigūracijas ir mokėjimo sąskaitas.</span><span class="sxs-lookup"><span data-stu-id="9af4a-105">Before you complete this task, you must set up export format configurations and payment accounts.</span></span>



<span data-ttu-id="9af4a-106">Ši procedūra buvo sukurta naudojant demonstracinių duomenų įmonės DEMF.</span><span class="sxs-lookup"><span data-stu-id="9af4a-106">This procedure was created using the demo data company DEMF.</span></span>



<span data-ttu-id="9af4a-107">Tai yra trečioji iš penkių procedūrų, kuriose apibūdinamas kliento mokėjimo naudojant elektroninių ataskaitų konfigūracijas procesas.</span><span class="sxs-lookup"><span data-stu-id="9af4a-107">This is the third of five procedures that demonstrate the customer payment process using electronic reporting configurations.</span></span>

1. <span data-ttu-id="9af4a-108">Pasirinkite Gautinos sumos > Mokėjimų sąranka > Mokėjimo būdai.</span><span class="sxs-lookup"><span data-stu-id="9af4a-108">Go to Accounts receivable > Payments setup > Methods of payment.</span></span>
2. <span data-ttu-id="9af4a-109">Norėdami rasti įrašus, naudokite spartųjį filtrą.</span><span class="sxs-lookup"><span data-stu-id="9af4a-109">Use the Quick Filter to find records.</span></span> <span data-ttu-id="9af4a-110">Pvz., filtruokite lauką Mokėjimo būdas reikšme „ELEKTRONINIS“.</span><span class="sxs-lookup"><span data-stu-id="9af4a-110">For example, filter on the Method of payment field with a value of 'ELECTRONIC'.</span></span>
3. <span data-ttu-id="9af4a-111">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="9af4a-111">Click Edit.</span></span>
4. <span data-ttu-id="9af4a-112">Lauke Mokėjimo sąskaita nurodykite reikšmes „DEMF OPER‟.</span><span class="sxs-lookup"><span data-stu-id="9af4a-112">In the Payment account field, specify the values 'DEMF OPER'.</span></span>
5. <span data-ttu-id="9af4a-113">Išplėskite dalį Failo formatai.</span><span class="sxs-lookup"><span data-stu-id="9af4a-113">Expand the File formats section.</span></span>
6. <span data-ttu-id="9af4a-114">Lauke Bendrosios elektroninės ataskaitos pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="9af4a-114">Select Yes in the Generic electronic reporting field.</span></span>
7. <span data-ttu-id="9af4a-115">Lauke Eksportuoti formato konfigūraciją įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="9af4a-115">In the Export format configuration field, enter or select a value.</span></span>
    * <span data-ttu-id="9af4a-116">Sąraše pasirinkite ISO20022 tiesioginis debetas (DE).</span><span class="sxs-lookup"><span data-stu-id="9af4a-116">In the list, select ISO20022 Direct debit (DE).</span></span>  <span data-ttu-id="9af4a-117">Jei sąrašas yra tuščias, nėra importuotos ir aktyvios kliento mokėjimų eksporto formato konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="9af4a-117">If the list is empty, the customer payment export format configuration has not been imported and active.</span></span>  
8. <span data-ttu-id="9af4a-118">Lauke Reikalauti įgaliojimo pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="9af4a-118">Select Yes in the Require mandate field.</span></span>
    * <span data-ttu-id="9af4a-119">Pasirinkite kliento mokėjimo formatų parametrą Reikalauti įgaliojimo, kurį nustačius į mokėjimo pranešimą reikia įtraukti įgaliojimo informaciją, pvz., SEPA tiesioginis debetą.</span><span class="sxs-lookup"><span data-stu-id="9af4a-119">Select the Require mandate parameter for customer payment formats, which require including mandate information in the payment message, like SEPA direct debit.</span></span>  
9. <span data-ttu-id="9af4a-120">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="9af4a-120">Click Save.</span></span>

