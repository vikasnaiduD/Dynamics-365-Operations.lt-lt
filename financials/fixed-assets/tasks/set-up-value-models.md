--- 
title: Nustatyti knygas
description: "Šioje procedūroje parodoma, kaip kurti naują ilgalaikio turto knygą ir susieti ją su ilgalaikio turto grupe."
author: saraschi2
manager: AnnBe
ms.date: 10/11/2016
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: a29cae6cdcd03903359a3a468243c6ad03c7adc6
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-books"></a><span data-ttu-id="c1590-103">Nustatyti knygas</span><span class="sxs-lookup"><span data-stu-id="c1590-103">Set up books</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="c1590-104">Šioje procedūroje parodoma, kaip kurti naują ilgalaikio turto knygą ir susieti ją su ilgalaikio turto grupe.</span><span class="sxs-lookup"><span data-stu-id="c1590-104">This procedure shows you to how create a new fixed asset book and associate it with a fixed asset group.</span></span> <span data-ttu-id="c1590-105">Joje naudojamas vaidmuo Buhalteris ir USMF juridinio subjekto demonstraciniai duomenys.</span><span class="sxs-lookup"><span data-stu-id="c1590-105">It uses the accountant role and demo data for the USMF legal entity.</span></span>


## <a name="create-a-book"></a><span data-ttu-id="c1590-106">Knygos kūrimas</span><span class="sxs-lookup"><span data-stu-id="c1590-106">Create a book</span></span>
1. <span data-ttu-id="c1590-107">Pasirinkite Ilgalaikis turtas > Sąranka > Knygos.</span><span class="sxs-lookup"><span data-stu-id="c1590-107">Go to Fixed assets > Setup > Books.</span></span>
2. <span data-ttu-id="c1590-108">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="c1590-108">Click New.</span></span>
3. <span data-ttu-id="c1590-109">Lauke Knyga įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c1590-109">In the Book field, type a value.</span></span>
4. <span data-ttu-id="c1590-110">Lauke Aprašas įveskite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c1590-110">In the Description field, type a value.</span></span>
    * <span data-ttu-id="c1590-111">Pasirinkus Skaičiuoti nusidėvėjimą, susijusi knyga bus įtraukta į nusidėvėjimo pasiūlymus.</span><span class="sxs-lookup"><span data-stu-id="c1590-111">If Calculate depreciation is selected, the associated asset book will be included in depreciation proposals.</span></span> <span data-ttu-id="c1590-112">Jei parinktis nepasirinkta, turto knyga nebus automatiškai nudėvima.</span><span class="sxs-lookup"><span data-stu-id="c1590-112">If it is not selected, the asset book will not be automatically depreciated.</span></span>  
5. <span data-ttu-id="c1590-113">Lauke Skaičiuoti nusidėvėjimą pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="c1590-113">Select Yes in the Calculate depreciation field.</span></span>
6. <span data-ttu-id="c1590-114">Lauke Nusidėvėjimo šablonas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c1590-114">In the Depreciation profile field, enter or select a value.</span></span>
    * <span data-ttu-id="c1590-115">Alternatyvus nusidėvėjimo šablonas taip pat vadinamas nusidėvėjimo perjungimo metodu.</span><span class="sxs-lookup"><span data-stu-id="c1590-115">An alternative depreciation profile is also known as a switchover method of depreciation.</span></span> <span data-ttu-id="c1590-116">Į šį šabloną nusidėvėjimo pasiūlymas persijungs, kai alternatyvus šablonas apskaičiuos nusidėvėjimo sumą, kuri yra lygi numatytajam nusidėvėjimo šablonui arba už jį didesnė.</span><span class="sxs-lookup"><span data-stu-id="c1590-116">The depreciation proposal will switch to this profile when the alternative profile calculates a depreciation amount that is equal to or greater than the default depreciation profile.</span></span>  
    * <span data-ttu-id="c1590-117">Visiško nusidėvėjimo šablonas naudojamas neįprastas atvejais papildomai skaičiuojant turto nusidėvėjimą.</span><span class="sxs-lookup"><span data-stu-id="c1590-117">The Extraordinary depreciation profile is used for additional depreciation of an asset in unusual circumstances.</span></span> <span data-ttu-id="c1590-118">Pavyzdžiui, galite tai naudoti norėdami įrašyti nusidėvėjimą įvykus gamtos katastrofai.</span><span class="sxs-lookup"><span data-stu-id="c1590-118">For example, you might use this to record depreciation that results from a natural disaster.</span></span>  
    * <span data-ttu-id="c1590-119">Pasirinkus Kurti nusidėvėjimo koregavimus su pagrindo koregavimais, nusidėvėjimo koregavimai bus automatiškai sukurti atnaujinus turto vertę.</span><span class="sxs-lookup"><span data-stu-id="c1590-119">If Create depreciation adjustments with basis adjustments is selected, depreciation adjustments will be automatically created when the value of the asset is updated.</span></span> <span data-ttu-id="c1590-120">Jei parinktis nepasirinkta, atnaujinta turto vertė turės įtakos tik tolimesniems nusidėvėjimo skaičiavimams.</span><span class="sxs-lookup"><span data-stu-id="c1590-120">If it is not selected, the updated asset value will only affect depreciation calculations going forward.</span></span>  
7. <span data-ttu-id="c1590-121">Lauke Kurti nusidėvėjimo koregavimus su pagrindo koregavimais pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="c1590-121">Select Yes in the Create depreciation adjustments with basis adjustments field.</span></span>
    * <span data-ttu-id="c1590-122">Pagal numatytuosius parametrus ilgalaikio turto knygos operacijos bus registruojamos DK.</span><span class="sxs-lookup"><span data-stu-id="c1590-122">By default, fixed asset book transactions will post to the general ledger.</span></span> <span data-ttu-id="c1590-123">Galite išjungti knygos registravimo DK funkciją, nustatydami lauką Registruoti DK į parinktį Ne.</span><span class="sxs-lookup"><span data-stu-id="c1590-123">You can disable posting to the general ledger for the book by setting the Post to general ledger field to No.</span></span> <span data-ttu-id="c1590-124">Knygos, kurios neregistruojamos DK, paprastai naudojamos mokesčių registravimo tikslais.</span><span class="sxs-lookup"><span data-stu-id="c1590-124">Books that do not post to the general ledger are typically used for tax reporting purposes.</span></span> <span data-ttu-id="c1590-125">Taip suteikiama daugiau lankstumo naikinant ankstesnes turto knygos operacijas, nes jos nebuvo perkeltos į DK.</span><span class="sxs-lookup"><span data-stu-id="c1590-125">This gives you additional flexibility to delete historical transactions for the asset book because they have not been committed to the general ledger.</span></span>  
    * <span data-ttu-id="c1590-126">Pagal numatytuosius parametrus registravimo sluoksnis nustatomas į parinktį Dabartinis sluoksnis, jei knyga registruojama DK, arba į parinktį Nė vienas, jei knyga neregistruojama DK.</span><span class="sxs-lookup"><span data-stu-id="c1590-126">The Posting layer defaults to the Current layer if the book posts to general ledger, and None if it does not post to general ledger.</span></span> <span data-ttu-id="c1590-127">Jei reikia, kad šios knygos operacijos būtų registruojamos į kitą sluoksnį, atnaujinkite registravimo sluoksnį.</span><span class="sxs-lookup"><span data-stu-id="c1590-127">Update Posting layer if you need transactions for this book to be posted to a different layer.</span></span>  
8. <span data-ttu-id="c1590-128">Lauke Kalendorius įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c1590-128">In the Calendar field, enter or select a value.</span></span>
    * <span data-ttu-id="c1590-129">Išvestinių knygų operacijos bus registruojamos kitose knygose tuo pačiu metu.</span><span class="sxs-lookup"><span data-stu-id="c1590-129">Derived books will post transactions to different books at the same time.</span></span> <span data-ttu-id="c1590-130">Galite kurti operacijas naudodami pagrindinę knygą – tada registravimo metu tikslios operacijų kopijos užregistruojamos išvestinėse knygose.</span><span class="sxs-lookup"><span data-stu-id="c1590-130">You create the transactions with the primary book and during posting, an exact copy of the transaction is posted to the derived book.</span></span> <span data-ttu-id="c1590-131">Išvestinės knygos operacijos nėra perskaičiuojamos, todėl jos neturėtų būti naudojamos atliekant nusidėvėjimo operacijas.</span><span class="sxs-lookup"><span data-stu-id="c1590-131">There is no recalculation with derived book transactions, so it should not be used for depreciation transactions.</span></span>  

## <a name="associate-the-book-with-a-fixed-asset-group"></a><span data-ttu-id="c1590-132">Knygos susiejimas su ilgalaikio turto grupe</span><span class="sxs-lookup"><span data-stu-id="c1590-132">Associate the book with a fixed asset group</span></span>
1. <span data-ttu-id="c1590-133">Spustelėkite Ilgalaikio turto grupės.</span><span class="sxs-lookup"><span data-stu-id="c1590-133">Click Fixed asset groups.</span></span>
2. <span data-ttu-id="c1590-134">Lauke Ilgalaikio turto grupė įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="c1590-134">In the Fixed asset group field, enter or select a value.</span></span>
3. <span data-ttu-id="c1590-135">Lauke Dėvėjimo laikas įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="c1590-135">In the Service life field, enter a number.</span></span>
    * <span data-ttu-id="c1590-136">Atkreipkite dėmesį, kad lauko Nusidėvėjimo laikotarpiai reikšmė apskaičiuojama nustačius dėvėjimo laiką.</span><span class="sxs-lookup"><span data-stu-id="c1590-136">Note that Depreciation periods is calculated after setting the Service life.</span></span>  
    * <span data-ttu-id="c1590-137">Mokesčių tvarkymo tikslais galite pagal poreikį nustatyti nusidėvėjimo konvenciją.</span><span class="sxs-lookup"><span data-stu-id="c1590-137">You are able to set the depreciation convention as required for tax purposes.</span></span>  

