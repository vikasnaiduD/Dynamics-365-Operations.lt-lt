--- 
title: "Kurti vienkartinio tiekėjo pirkimo užsakymą"
description: "Šia procedūra parodoma, kaip neautomatiniu būdu kurti vienkartinio tiekėjo pirkimo užsakymą."
author: FrankDahl
manager: AnnBe
ms.date: 08/23/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: bis
ms.search.scope: Operations
ms.search.region: Global
ms.author: fdahl
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 2d4dabaf6e1d79cbd626294ee4e327f2725a5e43
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="create-a-purchase-order-for-a-one-time-supplier"></a><span data-ttu-id="d4a60-103">Kurti vienkartinio tiekėjo pirkimo užsakymą</span><span class="sxs-lookup"><span data-stu-id="d4a60-103">Create a purchase order for a one-time supplier</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="d4a60-104">Šia procedūra parodoma, kaip neautomatiniu būdu kurti vienkartinio tiekėjo pirkimo užsakymą.</span><span class="sxs-lookup"><span data-stu-id="d4a60-104">This procedure shows you how to create a purchase order for a one-time supplier.</span></span> <span data-ttu-id="d4a60-105">Tiekėjas yra automatiškai sukuriamas kartu su pirkimo užsakymu, užuot tiekėjo kodą kūrus neautomatiškai.</span><span class="sxs-lookup"><span data-stu-id="d4a60-105">The supplier is created automatically with the purchase order, rather than having to create the vendor account manually.</span></span> <span data-ttu-id="d4a60-106">Pirkimo užsakymus paprastai kuria pirkimo agentas.</span><span class="sxs-lookup"><span data-stu-id="d4a60-106">Purchase orders are typically created by a purchasing agent.</span></span> <span data-ttu-id="d4a60-107">Šiame vedlyje pateikiamą pavyzdį galima naudoti demonstracinių duomenų įmonėje USMF.</span><span class="sxs-lookup"><span data-stu-id="d4a60-107">The example shown in this guide can be used in the USMF demo data company.</span></span> <span data-ttu-id="d4a60-108">Būtina vienkartinį tiekėjo kodą nustatyti puslapyje Mokėtinų sumų parametrai.</span><span class="sxs-lookup"><span data-stu-id="d4a60-108">It is a prerequisite that a one-time vendor account has been set up in the Account payable parameters page.</span></span>


## <a name="create-a-purchase-order-for-a-one-time-supplier"></a><span data-ttu-id="d4a60-109">Kurti vienkartinio tiekėjo pirkimo užsakymą</span><span class="sxs-lookup"><span data-stu-id="d4a60-109">Create a purchase order for a one-time supplier</span></span>
1. <span data-ttu-id="d4a60-110">Pasirinkite Įsigijimas ir šaltinio pasirinkimas > Pirkimo užsakymai > Visi pirkimo užsakymai.</span><span class="sxs-lookup"><span data-stu-id="d4a60-110">Go to Procurement and sourcing > Purchase orders > All purchase orders.</span></span>
2. <span data-ttu-id="d4a60-111">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="d4a60-111">Click New.</span></span>
3. <span data-ttu-id="d4a60-112">Lauke Vienkartinis tiekėjas pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="d4a60-112">Select Yes in the One-time supplier field.</span></span>
    * <span data-ttu-id="d4a60-113">Tiekėjo kodas automatiškai sukuriamas ir priskiriamas pirkimo užsakymui.</span><span class="sxs-lookup"><span data-stu-id="d4a60-113">A vendor account is automatically created and assigned to the purchase order.</span></span> <span data-ttu-id="d4a60-114">Tiekėjo kodas sukuriamas pagal šabloną, kuris nurodytas puslapio Mokėtinų sumų parametrai skirtuke Bendra.</span><span class="sxs-lookup"><span data-stu-id="d4a60-114">The vendor account is created based on the template that is specified on the General tab in the Accounts payable parameters page.</span></span>  
4. <span data-ttu-id="d4a60-115">Lauke Pavadinimas įveskite tiekėjo pavadinimą.</span><span class="sxs-lookup"><span data-stu-id="d4a60-115">In the Name field, type a name for the supplier.</span></span>
5. <span data-ttu-id="d4a60-116">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="d4a60-116">Click OK.</span></span>
    * <span data-ttu-id="d4a60-117">Dabar pirkimo užsakymą galima baigti ir apdoroti kaip bet kurį kitą užsakymą.</span><span class="sxs-lookup"><span data-stu-id="d4a60-117">The purchase order can now be completed and processed like any other order.</span></span> <span data-ttu-id="d4a60-118">Nėra jokių specialių charakteristikų, susijusių su tuo, kaip tai daroma.</span><span class="sxs-lookup"><span data-stu-id="d4a60-118">There are no special characteristics related to how this is done.</span></span> <span data-ttu-id="d4a60-119">SF bus apskaityta apmokėtina tiekėjo kodo, sukurto kartu su užsakymu, operacija ir tada mokėjimas bus apdorotas.</span><span class="sxs-lookup"><span data-stu-id="d4a60-119">The invoice will account a due transaction on the vendor account that was created with the order, and payment will then be processed.</span></span> <span data-ttu-id="d4a60-120">Tai atlikus, tiekėjo kodą galima panaikinti.</span><span class="sxs-lookup"><span data-stu-id="d4a60-120">When this is completed, the vendor account can be deleted.</span></span> <span data-ttu-id="d4a60-121">Paprastai tai atlieka mokėtinų sumų padalinys.</span><span class="sxs-lookup"><span data-stu-id="d4a60-121">This is typically done by the accounts payable department.</span></span>  

