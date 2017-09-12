--- 
title: "Nustatyti mokėtinų sumų SF sugretinimo patvirtinimą"
description: "Šiame įraše naudojama demonstracinė įmonė USMF."
author: abruer
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
ms.author: abruer
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: 2bdb7b5f871aac780cb891b88d6aa614e6b21c4e
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="set-up-accounts-payable-invoice-matching-validation"></a><span data-ttu-id="57ac5-103">Nustatyti mokėtinų sumų SF sugretinimo patvirtinimą</span><span class="sxs-lookup"><span data-stu-id="57ac5-103">Set up accounts payable invoice matching validation</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="57ac5-104">Šiame įraše naudojama demonstracinė įmonė USMF.</span><span class="sxs-lookup"><span data-stu-id="57ac5-104">This recording uses the USMF demo company.</span></span> <span data-ttu-id="57ac5-105">Šiuos veiksmus paprastai atlieka mokėtinų sumų vadovo arba apskaitos vadovo vaidmuo.</span><span class="sxs-lookup"><span data-stu-id="57ac5-105">The accounts payable manager or accounting manager role would perform these steps.</span></span> <span data-ttu-id="57ac5-106">Prieš pradėdami įsitikinkite, kad pasirinktas SF gretinimo konfigūracijos raktas.</span><span class="sxs-lookup"><span data-stu-id="57ac5-106">Before you begin, make sure that the Invoice matching configuration key is selected.</span></span> <span data-ttu-id="57ac5-107">Jei jūsų juridinis subjektas seka išlaidas, pavyzdžiui, transportavimo, įsitikinkite, kad pasirinktas konfigūracijos raktas Išlaidos.</span><span class="sxs-lookup"><span data-stu-id="57ac5-107">If your legal entity tracks expenses, such as freight, by using charges, make sure that the Charges configuration key is selected.</span></span>  <span data-ttu-id="57ac5-108">Mokėtinų sumų SF gretinimas yra tiekėjo SF, pirkimo užsakymo ir produkto gavimo kvito informacijos gretinimo procesas.</span><span class="sxs-lookup"><span data-stu-id="57ac5-108">Accounts payable invoice matching is the process of matching vendor invoice, purchase order, and product receipt information.</span></span> <span data-ttu-id="57ac5-109">Skirtumai tarp šių dokumentų vadinami gretinimo neatitikimais.</span><span class="sxs-lookup"><span data-stu-id="57ac5-109">Differences among these documents are called matching discrepancies.</span></span> <span data-ttu-id="57ac5-110">Gretinimo nesutapimai lyginami su nurodytais leistinais nuokrypiais.</span><span class="sxs-lookup"><span data-stu-id="57ac5-110">Matching discrepancies are compared with the tolerances that are specified.</span></span> <span data-ttu-id="57ac5-111">Jei gretinimo neatitikimas viršija leistino nuokrypio procentą ar sumą, formoje Tiekėjo SF ir formoje SF gretinimo informacija rodomos gretinimo nuokrypio piktogramos.</span><span class="sxs-lookup"><span data-stu-id="57ac5-111">If a matching discrepancy exceeds the tolerance percentage or amount, match variance icons are displayed in the Vendor invoice form and in the Invoice matching details form.</span></span>

1. <span data-ttu-id="57ac5-112">Pasirinkite Mokėtinos sumos > Sąranka > Mokėtinų sumų parametrai.</span><span class="sxs-lookup"><span data-stu-id="57ac5-112">Go to Accounts payable > Setup > Accounts payable parameters.</span></span>
2. <span data-ttu-id="57ac5-113">Spustelėkite skirtuką SF tikrinimas.</span><span class="sxs-lookup"><span data-stu-id="57ac5-113">Click the Invoice validation tab.</span></span>
3. <span data-ttu-id="57ac5-114">Pažymėkite arba atžymėkite žymės langelį Įgalinti SF gretinimo tikrinimą.</span><span class="sxs-lookup"><span data-stu-id="57ac5-114">Check or uncheck the Enable invoice matching validation checkbox.</span></span>
    * <span data-ttu-id="57ac5-115">Pasirinkite, ar reikalauti patvirtinimo prieš registruojant SF, kurioje yra SF gretinimo nesutapimų.</span><span class="sxs-lookup"><span data-stu-id="57ac5-115">Select whether approval is required before an invoice that contains discrepancies for invoice matching can be posted.</span></span> <span data-ttu-id="57ac5-116">Jei nustatyta Leisti įspėjant, kai SF gretinimo nesutapimas viršys leistiną nuokrypį, tai bus vizualiai parodoma.</span><span class="sxs-lookup"><span data-stu-id="57ac5-116">If this is set to Allow with warning, visual indication will display when a discrepancy for invoice matching exceeds the tolerance.</span></span> <span data-ttu-id="57ac5-117">Tačiau SF galėsite registruoti.</span><span class="sxs-lookup"><span data-stu-id="57ac5-117">However, you will be able to post the invoice.</span></span> <span data-ttu-id="57ac5-118">Norėdami kartu naudoti darbo eigas ir SF gretinimo tvirtinimą, įsitikinkite, kad laukas Registruoti SF su nesutapimais nustatytas į Leisti įspėjant, kad nereikėtų tvirtinti kelis kartus.</span><span class="sxs-lookup"><span data-stu-id="57ac5-118">To use workflows together with invoice matching validation, make sure that the Post invoice with discrepancies field is set to Allow with warning to avoid having to approve multiple times.</span></span>  
    * <span data-ttu-id="57ac5-119">Lauke Automatiškai atnaujinti sąskaitos faktūros antraštės atitikimo būseną pasirinkite, ar sistemai įvedant SF duomenis, gretinimas bus atliekamas automatiškai.</span><span class="sxs-lookup"><span data-stu-id="57ac5-119">In the Automatically update invoice header match status field, select whether matching will be performed automatically during invoice data entry by the system.</span></span> <span data-ttu-id="57ac5-120">Rekomenduojama nuostata yra Taip, nebent susiduriate su duomenų įvedimo efektyvumo problemomis.</span><span class="sxs-lookup"><span data-stu-id="57ac5-120">The recommended setting is Yes, unless you are experiencing data entry performance concerns.</span></span> <span data-ttu-id="57ac5-121">Išjungus automatinius atnaujinimus gali pagreitėti sistemos efektyvumas, nes SF gretinimo tikrinimas įvedant duomenis bus praleistas.</span><span class="sxs-lookup"><span data-stu-id="57ac5-121">Disabling automatic updates may enable faster system performance because the invoice matching validation will be bypassed during data entry.</span></span> <span data-ttu-id="57ac5-122">Kai nustatyta Ne, duomenų įvedimo klerkas turės rankiniu būdu atnaujinti SF gretinimo būseną, kad matytų SF gretinimo tikrinimo rezultatus.</span><span class="sxs-lookup"><span data-stu-id="57ac5-122">The data entry clerk will need to manually update the invoice’s match status to see the invoice matching validation results when this is set to No.</span></span>  
4. <span data-ttu-id="57ac5-123">Perjunkite dalies SF bendrųjų sumų gretinimas išplėtimą.</span><span class="sxs-lookup"><span data-stu-id="57ac5-123">Toggle the expansion of the Invoice totals matching section.</span></span>
5. <span data-ttu-id="57ac5-124">Pažymėkite arba atžymėkite žymės langelį Gretinti SF sumas, kad sugretintumėte faktines SF sumas su numatomomis sumomis.</span><span class="sxs-lookup"><span data-stu-id="57ac5-124">Check or uncheck the Match invoice totals checkbox to match actual invoice totals with expected totals.</span></span>
    * <span data-ttu-id="57ac5-125">Pasirinkite, ar rodyti piktogramą, jei SF gretinimo neatitikimas viršija leidžiamą nuokrypį.</span><span class="sxs-lookup"><span data-stu-id="57ac5-125">Select whether an icon is displayed if a discrepancy for invoice matching exceeds the tolerance.</span></span> <span data-ttu-id="57ac5-126">Galite pasirinkti rodyti piktogramą, kai teigiamas neatitikimas viršija leidžiamą nuokrypį arba kai teigiamas ar neigiamas neatitikimas viršija leidžiamą nuokrypį.</span><span class="sxs-lookup"><span data-stu-id="57ac5-126">You can select to display the icon when a positive discrepancy exceeds the tolerance, or when either a positive or a negative discrepancy exceeds the tolerance.</span></span>  
    * <span data-ttu-id="57ac5-127">Pvz., leidžiamas nuokrypis yra 5 proc., o pirkimo užsakymo bendroji SF suma yra 100,00.</span><span class="sxs-lookup"><span data-stu-id="57ac5-127">For example, the tolerance is 5 percent, and the total invoice amount on the purchase order is 100.00.</span></span> <span data-ttu-id="57ac5-128">Todėl kainų gretinimo piktograma rodoma, jei SF bendroji suma viršija 105,00.</span><span class="sxs-lookup"><span data-stu-id="57ac5-128">Therefore, a price match icon is displayed if the total invoice amount on the invoice exceeds 105.00.</span></span> <span data-ttu-id="57ac5-129">Pažymėjus parinktį Jei didesnis arba mažesnis nei leidžiamas nuokrypis, piktograma taip pat rodoma, kai SF suma yra mažesnė nei 95,00.</span><span class="sxs-lookup"><span data-stu-id="57ac5-129">If you select If greater than or less than tolerance, the icon is also displayed if the invoice amount is less than 95.00.</span></span>  
6. <span data-ttu-id="57ac5-130">Lauke SF sumų leistino nuokrypio procentas įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="57ac5-130">In the Invoice totals tolerance percentage field, enter a number.</span></span>
7. <span data-ttu-id="57ac5-131">Perjunkite dalies Kainos ir kiekio gretinimas išplėtimą.</span><span class="sxs-lookup"><span data-stu-id="57ac5-131">Toggle the expansion of the Price and quantity matching section.</span></span>
    * <span data-ttu-id="57ac5-132">Lauke Eilučių atitikimo strategija pasirinkite reikšmę, naudotiną kaip numatytoji juridinio subjekto, su kuriuo dirbate, strategija.</span><span class="sxs-lookup"><span data-stu-id="57ac5-132">In the Line matching policy field, select a value to be used as the default policy for the legal entity that you are working with.</span></span> <span data-ttu-id="57ac5-133">„Nebūtina‟ reiškia, kad nereikia tikrinti atskirų SF eilučių kainų ir pirkimo užsakymo kainų bei SF kiekių ir važtaraščio kiekių.</span><span class="sxs-lookup"><span data-stu-id="57ac5-133">“Not required” means there is no verification of individual invoice line prices to purchase order price or invoice quantities to packing slip quantities required.</span></span> <span data-ttu-id="57ac5-134">„Dvišalis atitikimas‟ reiškia, kad tikrinti SF eilutes reikia, bet tikrinant įtraukiami tik pirkimo užsakymo ir tiekėjo SF dokumentai.</span><span class="sxs-lookup"><span data-stu-id="57ac5-134">“Two-Way Match” means that the verification of invoice lines is required but only the purchase order and the supplier’s invoice documents are involved in the verification.</span></span> <span data-ttu-id="57ac5-135">Produkto gavimo kvitas į gretinimo tikrinimus neįtraukiamas.</span><span class="sxs-lookup"><span data-stu-id="57ac5-135">The product receipt isn’t factored into the matching validations.</span></span> <span data-ttu-id="57ac5-136">„Trišalis atitikimas‟ reiškia, kad SF grynoji prekės kaina bus lyginama su pirkimo užsakymo grynąja prekės kaina, o atitinkantis produkto gavimo kvito kiekis bus lyginamas su SF kiekiu.</span><span class="sxs-lookup"><span data-stu-id="57ac5-136">“Three-Way Match” means that the invoice net unit price will be compared to the purchase order’s net unit price and the matching product receipt quantity will be compared to the invoice quantity.</span></span>  
    * <span data-ttu-id="57ac5-137">Jei naudojate eilučių atitikimo strategiją Dvišalis atitikimas arba Trišalis atitikimas, puslapyje Leistinas prekių kainų nuokrypis galite nustatyti juridinio subjekto, prekių ir tiekėjų leistino kainų nuokrypio procentus.</span><span class="sxs-lookup"><span data-stu-id="57ac5-137">If you use a line matching policy of Two-way matching or Three-way matching, you can set up price tolerance percentages for your legal entity, items, and vendors on the Item price tolerance page.</span></span> <span data-ttu-id="57ac5-138">Kai tiekėjo SF palyginamos su pirkimo užsakymų informacija, ieškoma taikytino leidžiamo kainų nuokrypio procento.</span><span class="sxs-lookup"><span data-stu-id="57ac5-138">When vendor invoices are compared with the information on purchase orders, the applicable price tolerance percentage is searched for.</span></span>  
8. <span data-ttu-id="57ac5-139">Lauke Eilučių atitikimo strategija pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="57ac5-139">In the Line matching policy field, select an option.</span></span>
    * <span data-ttu-id="57ac5-140">Norėdami leisti prekei, tiekėjui, tiekėjo ir prekės deriniui arba pirkimo užsakymo eilutei taikyti skirtingą gretinimo lygį, pasirinkite reikšmę lauke Leisti nepaisyti atitikimo strategijos.</span><span class="sxs-lookup"><span data-stu-id="57ac5-140">To allow a different level of matching to be applied for an item, vendor, vendor and item combination, or purchase order line, select a value in the Allow matching policy override field.</span></span> <span data-ttu-id="57ac5-141">Konkretaus tiekėjo, prekės ar tiekėjo ir prekės derinio juridinio subjekto eilučių atitikimo strategiją galima pakeisti puslapyje Atitikimo strategija.</span><span class="sxs-lookup"><span data-stu-id="57ac5-141">The legal entity line matching policy can be overridden for a specific vendor, item, or vendor and item combination in the Matching policy page.</span></span>  
    * <span data-ttu-id="57ac5-142">Norėdami sugretinti SF eilučių prekių bendrąsias kainas, pasirinkite reikšmę lauke Gretinti kainų sumas.</span><span class="sxs-lookup"><span data-stu-id="57ac5-142">To match price totals for line items on invoices, select a value in the Match price totals field.</span></span> <span data-ttu-id="57ac5-143">Šis gretinimo tipas yra naudingas, kai tiekėjas už tą pačią pirkimo užsakymo eilutę siunčia kelias SF.</span><span class="sxs-lookup"><span data-stu-id="57ac5-143">This type of matching is useful when the vendor sends multiple invoices for the same purchase order line.</span></span> <span data-ttu-id="57ac5-144">Kiekvienos SF eilutės ir visų laukiančių bei anksčiau užregistruotų SF eilučių grynosios sumos kainos informaciją galite palyginti su atitinkamos pirkimo užsakymo eilutės grynąja suma.</span><span class="sxs-lookup"><span data-stu-id="57ac5-144">You can compare price information for the net amount of each line on the invoice and all pending and previously posted invoice lines, with the net amount of the corresponding purchase order line.</span></span>  
9. <span data-ttu-id="57ac5-145">Lauke Gretinti kainų sumas pasirinkite parinktį.</span><span class="sxs-lookup"><span data-stu-id="57ac5-145">In the Match price totals field, select an option.</span></span>
10. <span data-ttu-id="57ac5-146">Lauke Pirkimo kainos visas leistinas nuokrypis įveskite skaičių.</span><span class="sxs-lookup"><span data-stu-id="57ac5-146">In the Purchase price total tolerance field, enter a number.</span></span>
11. <span data-ttu-id="57ac5-147">Perjunkite dalies Išlaidų gretinimas išplėtimą.</span><span class="sxs-lookup"><span data-stu-id="57ac5-147">Toggle the expansion of the Charges matching section.</span></span>
12. <span data-ttu-id="57ac5-148">Norėdami sugretinti faktines išlaidas ir tikėtinas išlaidas, remdamiesi pirkimo užsakymo informacija, pažymėkite žymės langelį Gretinti išlaidas.</span><span class="sxs-lookup"><span data-stu-id="57ac5-148">To match actual charges with expected charges, based on information on the purchase order, select the Match charges check box.</span></span>
13. <span data-ttu-id="57ac5-149">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="57ac5-149">Close the page.</span></span>

