--- 
title: "Ataskaitų generavimas „Microsoft Office“ formatais su įdėtaisiais vaizdais elektroninėse ataskaitose (ER)"
description: "Šie veiksmai paaiškina, kaip sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmenį turintis vartotojas gali sukurti naują elektroninių ataskaitų teikimo (ER) konfigūraciją, skirtą elektroninių dokumentų, turinčių įdėtųjų vaizdų, generavimui „MS office“ formatais („Excel“ ir „Word“)."
author: NickSelin
manager: AnnBe
ms.date: 06/13/2017
ms.topic: business-process
ms.prod: 
ms.service: dynamics-ax-applications
ms.technology: 
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.translationtype: HT
ms.sourcegitcommit: 663da58ef01b705c0c984fbfd3fce8bc31be04c6
ms.openlocfilehash: de2840ebc6c91e313546859f5c0d8939eb80977b
ms.contentlocale: lt-lt
ms.lasthandoff: 08/29/2017

---
# <a name="generate-reports-in-microsoft-office-formats-with-embedded-images-for-electronic-reporting-er"></a><span data-ttu-id="f60bb-103">Ataskaitų generavimas „Microsoft Office“ formatais su įdėtaisiais vaizdais elektroninėse ataskaitose (ER)</span><span class="sxs-lookup"><span data-stu-id="f60bb-103">Generate reports in Microsoft Office formats with embedded images for electronic reporting (ER)</span></span>

[!include[task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="f60bb-104">Šie veiksmai paaiškina, kaip sistemos administratoriaus arba elektroninių ataskaitų kūrėjo vaidmenį turintis vartotojas gali sukurti naują elektroninių ataskaitų teikimo (ER) konfigūraciją, skirtą elektroninių dokumentų, turinčių įdėtųjų vaizdų, generavimui „MS office“ formatais („Excel“ ir „Word“).</span><span class="sxs-lookup"><span data-stu-id="f60bb-104">The following steps explain how a user playing either ‘System administrator’ or ‘Electronic reporting developer’ role can design Electronic reporting (ER) configurations to generate electronic documents in MS office formats (Excel and Word) containing embedded images.</span></span>

<span data-ttu-id="f60bb-105">Šiame pavyzdyje naudosite sukurtas pavyzdinės įmonės „Litware, Inc.“ ER konfigūracijas.</span><span class="sxs-lookup"><span data-stu-id="f60bb-105">In this example, you will use created ER configurations for sample company, ‘Litware, Inc.’.</span></span>  <span data-ttu-id="f60bb-106">Norėdami atlikti šiuos veiksmus, turite užbaigti veiksmus užduočių vedlyje „ER padaryti ataskaitas „MS Office“ formatais su įdėtaisiais vaizdais (2 dalis: peržiūrėti konfigūracijas)“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-106">To complete these steps, you must first complete the steps in the “ER Make reports in MS Office formats with embedded images (Part 2: Review configurations)” task guide.</span></span> <span data-ttu-id="f60bb-107">Šiuos veiksmus galima atlikti USMF įmonėje.</span><span class="sxs-lookup"><span data-stu-id="f60bb-107">These steps can be performed in ‘USMF’ company.</span></span>


## <a name="run-format-with-initial-model-mapping"></a><span data-ttu-id="f60bb-108">Paleiskite formatą pradiniu modelio susiejimu</span><span class="sxs-lookup"><span data-stu-id="f60bb-108">Run format with initial model mapping</span></span>
1. <span data-ttu-id="f60bb-109">Pasirinkite Grynųjų pinigų ir banko valdymas > Banko kodai > Banko kodai.</span><span class="sxs-lookup"><span data-stu-id="f60bb-109">Go to Cash and bank management > Bank accounts > Bank accounts.</span></span>
2. <span data-ttu-id="f60bb-110">Naudokite spartųjį filtrą, kad filtruotumėte lauką Banko sąskaita reikšme „USMF OPER‟.</span><span class="sxs-lookup"><span data-stu-id="f60bb-110">Use the Quick Filter to filter on the Bank account field with a value of 'USMF OPER'.</span></span>
3. <span data-ttu-id="f60bb-111">Veiksmų srityje spustelėkite Nustatyti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-111">On the Action Pane, click Set up.</span></span>
4. <span data-ttu-id="f60bb-112">Spustelėkite Tikrinti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-112">Click Check.</span></span>
5. <span data-ttu-id="f60bb-113">Spustelėkite Spausdinti testą.</span><span class="sxs-lookup"><span data-stu-id="f60bb-113">Click Print test.</span></span>
    * <span data-ttu-id="f60bb-114">Paleiskite formatą bandymams.</span><span class="sxs-lookup"><span data-stu-id="f60bb-114">Run the format for testing purposes.</span></span>  
6. <span data-ttu-id="f60bb-115">Lauke Perduodamo čekio formatas pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="f60bb-115">Select Yes in the Negotiable check format field.</span></span>
7. <span data-ttu-id="f60bb-116">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="f60bb-116">Click OK.</span></span>
    * <span data-ttu-id="f60bb-117">Peržiūrėkite sukurtą išvestį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-117">Review the created output.</span></span> <span data-ttu-id="f60bb-118">Atkreipkite dėmesį, kad įmonės logotipas pateikiamas ataskaitoje, taip pat ir įgalioto asmens parašas.</span><span class="sxs-lookup"><span data-stu-id="f60bb-118">Note that the company logo is presented in the report as well as the authorized person’s signature.</span></span> <span data-ttu-id="f60bb-119">Parašo vaizdas paimamas iš čekio išdėstymo įrašo duomenų tipo „Konteineris“ lauko, kuris susietas su pasirinkta banko sąskaita.</span><span class="sxs-lookup"><span data-stu-id="f60bb-119">The signature image is taken from the field of the ‘Container’ data type of the cheque layout record which is associated with the selected bank account.</span></span>  
8. <span data-ttu-id="f60bb-120">Išplėskite skyrių Kopijos.</span><span class="sxs-lookup"><span data-stu-id="f60bb-120">Expand the Copies section.</span></span>
9. <span data-ttu-id="f60bb-121">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-121">Click Edit.</span></span>
10. <span data-ttu-id="f60bb-122">Lauke Vandenženklis įveskite „Spausdinti vandenženklį kaip anuliuotą“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-122">In the Watermark field, enter 'Print watermark as Void'.</span></span>
    * <span data-ttu-id="f60bb-123">Pakeisti vandenženklio išdėstymo nustatymą, kad būtų rodomas vandenženklio tekstas generuojant dokumentą „Excel“ formos elemente.</span><span class="sxs-lookup"><span data-stu-id="f60bb-123">Change the watermark layout setting to show the watermark text in generating document in an Excel shape element.</span></span>  
11. <span data-ttu-id="f60bb-124">Spustelėkite Spausdinti testą.</span><span class="sxs-lookup"><span data-stu-id="f60bb-124">Click Print test.</span></span>
12. <span data-ttu-id="f60bb-125">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="f60bb-125">Click OK.</span></span>
    * <span data-ttu-id="f60bb-126">Peržiūrėkite sukurtą išvestį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-126">Review the created output.</span></span> <span data-ttu-id="f60bb-127">Atkreipkite dėmesį, kad vandenženklis rodomas sukurtoje ataskaitoje pagal žymėjimo parinktį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-127">Note that the watermark is shown in the created report in accordance to the selection option.</span></span>  
13. <span data-ttu-id="f60bb-128">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-128">Close the page.</span></span>
14. <span data-ttu-id="f60bb-129">Veiksmų srityje spustelėkite Valdyti mokėjimus.</span><span class="sxs-lookup"><span data-stu-id="f60bb-129">On the Action Pane, click Manage payments.</span></span>
15. <span data-ttu-id="f60bb-130">Spustelėkite Tikrinimai.</span><span class="sxs-lookup"><span data-stu-id="f60bb-130">Click Checks.</span></span>
16. <span data-ttu-id="f60bb-131">Spustelėkite Rodyti filtrus.</span><span class="sxs-lookup"><span data-stu-id="f60bb-131">Click Show filters.</span></span>
17. <span data-ttu-id="f60bb-132">Taikykite šiuos filtrus: įveskite filtro reikšmę „381“, „385“, „389“ lauke „Čekio numeris“, naudodami filtro operatorių „vienas iš“</span><span class="sxs-lookup"><span data-stu-id="f60bb-132">Apply the following filters: Enter a filter value of "381","385","389" on the "Check number" field using the "is one of" filter operator.</span></span>
18. <span data-ttu-id="f60bb-133">Sąraše pažymėkite visas eilutes.</span><span class="sxs-lookup"><span data-stu-id="f60bb-133">In the list, mark all rows.</span></span>
19. <span data-ttu-id="f60bb-134">Spustelėkite Spausdinti čekio kopiją.</span><span class="sxs-lookup"><span data-stu-id="f60bb-134">Click Print check copy.</span></span>
    * <span data-ttu-id="f60bb-135">Paleiskite formatą iš naujo spausdinti pasirinktus čekius.</span><span class="sxs-lookup"><span data-stu-id="f60bb-135">Run the format to re-print the selected cheques.</span></span>  
    * <span data-ttu-id="f60bb-136">Peržiūrėkite sukurtą išvestį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-136">Review the created output.</span></span> <span data-ttu-id="f60bb-137">Atkreipkite dėmesį, kad turite iš naujo išspausdinti pasirinktus čekius.</span><span class="sxs-lookup"><span data-stu-id="f60bb-137">Note that the selected cheques have been re-printed.</span></span> <span data-ttu-id="f60bb-138">Įmonės logotipas ir etiketės nespausdinamos, nes jos pateikiamos iš anksto išspausdintoje formoje.</span><span class="sxs-lookup"><span data-stu-id="f60bb-138">The company logo and labels are not printed out since they are presented on the pre-printed form.</span></span>  

## <a name="modify-the-mapping-of-the-imported-data-model"></a><span data-ttu-id="f60bb-139">Pakeiskite importuoto duomenų modelio susiejimą</span><span class="sxs-lookup"><span data-stu-id="f60bb-139">Modify the mapping of the imported data model</span></span>
1. <span data-ttu-id="f60bb-140">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-140">Close the page.</span></span>
2. <span data-ttu-id="f60bb-141">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-141">Close the page.</span></span>
3. <span data-ttu-id="f60bb-142">Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="f60bb-142">Go to Organization administration > Electronic reporting > Configurations.</span></span>
4. <span data-ttu-id="f60bb-143">Medyje pasirinkite „Model for cheques“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-143">In the tree, select 'Model for cheques'.</span></span>
5. <span data-ttu-id="f60bb-144">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="f60bb-144">Click Designer.</span></span>
6. <span data-ttu-id="f60bb-145">Spustelėkite „Susieti modelį su duomenų šaltiniu“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-145">Click Map model to datasource.</span></span>
7. <span data-ttu-id="f60bb-146">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="f60bb-146">Click Designer.</span></span>
    * <span data-ttu-id="f60bb-147">Mes pakeisime duomenų modelio parašo elemento susiejimą, kad gautume parašo vaizdą iš failo, pridėto prie čekio maketo įrašo, susieto su pasirinkta banko sąskaita.</span><span class="sxs-lookup"><span data-stu-id="f60bb-147">We will change the binding of the data model’s signature item to get the signature image from the file that has been attached to the cheque layout record which is associated with the selected bank account.</span></span>  
8. <span data-ttu-id="f60bb-148">Išjunkite Rodyti išsamią informaciją.</span><span class="sxs-lookup"><span data-stu-id="f60bb-148">Turn Show details off.</span></span>
9. <span data-ttu-id="f60bb-149">Medyje išplėskite „layout“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-149">In the tree, expand 'layout'.</span></span>
10. <span data-ttu-id="f60bb-150">Medyje išplėskite „layout\signature“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-150">In the tree, expand 'layout\signature'.</span></span>
11. <span data-ttu-id="f60bb-151">Medyje pasirinkite „layout\signature\image = chequesaccount.'<Relations'.BankChequeLayout.Signature1Bmp“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-151">In the tree, select 'layout\signature\image = chequesaccount.'<Relations'.BankChequeLayout.Signature1Bmp'.</span></span>
12. <span data-ttu-id="f60bb-152">Medyje išplėskite „chequesaccount“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-152">In the tree, expand 'chequesaccount'.</span></span>
13. <span data-ttu-id="f60bb-153">Medyje išplėskite „chequesaccount\<Relations“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-153">In the tree, expand 'chequesaccount\<Relations'.</span></span>
14. <span data-ttu-id="f60bb-154">Medyje pasirinkite „chequesaccount\<Relations\BankChequeLayout“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-154">In the tree, expand 'chequesaccount\<Relations\BankChequeLayout'.</span></span>
15. <span data-ttu-id="f60bb-155">Medyje išplėskite „chequesaccount\<Relations\BankChequeLayout\<Relations“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-155">In the tree, expand 'chequesaccount\<Relations\BankChequeLayout\<Relations'.</span></span>
16. <span data-ttu-id="f60bb-156">Medyje išplėskite „chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-156">In the tree, expand 'chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents'.</span></span>
17. <span data-ttu-id="f60bb-157">Medyje pasirinkite „chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents\getFileContentAsContainer()“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-157">In the tree, select 'chequesaccount\<Relations\BankChequeLayout\<Relations\<Documents\getFileContentAsContainer()'.</span></span>
18. <span data-ttu-id="f60bb-158">Spustelėkite Susieti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-158">Click Bind.</span></span>
19. <span data-ttu-id="f60bb-159">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-159">Click Save.</span></span>
20. <span data-ttu-id="f60bb-160">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-160">Close the page.</span></span>
21. <span data-ttu-id="f60bb-161">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-161">Close the page.</span></span>
22. <span data-ttu-id="f60bb-162">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-162">Close the page.</span></span>
23. <span data-ttu-id="f60bb-163">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-163">Close the page.</span></span>

## <a name="run-format-using-the-adjusted-model-mapping"></a><span data-ttu-id="f60bb-164">Vykdykite formatą, naudodami pakoreguotą modelio susiejimą</span><span class="sxs-lookup"><span data-stu-id="f60bb-164">Run format using the adjusted model mapping</span></span>
1. <span data-ttu-id="f60bb-165">Pasirinkite Grynųjų pinigų ir banko valdymas > Banko kodai > Banko kodai.</span><span class="sxs-lookup"><span data-stu-id="f60bb-165">Go to Cash and bank management > Bank accounts > Bank accounts.</span></span>
2. <span data-ttu-id="f60bb-166">Norėdami rasti įrašus, naudokite spartųjį filtrą.</span><span class="sxs-lookup"><span data-stu-id="f60bb-166">Use the Quick Filter to find records.</span></span> <span data-ttu-id="f60bb-167">Pavyzdžiui, filtruokite lauką Banko sąskaita, naudodami reikšmę „USMF OPER“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-167">For example, filter on the Bank account field with a value of 'USMF OPER'.</span></span>
3. <span data-ttu-id="f60bb-168">Veiksmų srityje spustelėkite Nustatyti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-168">On the Action Pane, click Set up.</span></span>
4. <span data-ttu-id="f60bb-169">Spustelėkite Tikrinti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-169">Click Check.</span></span>
5. <span data-ttu-id="f60bb-170">Spustelėkite Spausdinti testą.</span><span class="sxs-lookup"><span data-stu-id="f60bb-170">Click Print test.</span></span>
6. <span data-ttu-id="f60bb-171">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="f60bb-171">Click OK.</span></span>
    * <span data-ttu-id="f60bb-172">Peržiūrėkite sukurtą išvestį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-172">Review the created output.</span></span> <span data-ttu-id="f60bb-173">Atkreipkite dėmesį, kad vaizdas iš dokumentų valdymo priedo pateikiamas kaip įgalioto asmens parašas.</span><span class="sxs-lookup"><span data-stu-id="f60bb-173">Note that the image from the Document Management attachment is presented as the signature of an authorized person.</span></span>  

## <a name="use-ms-word-document-as-a-template-in-the-imported-format"></a><span data-ttu-id="f60bb-174">Naudokite „MS Word“ dokumentą kaip šabloną importuotame formate</span><span class="sxs-lookup"><span data-stu-id="f60bb-174">Use MS Word document as a template in the imported format</span></span>
1. <span data-ttu-id="f60bb-175">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-175">Close the page.</span></span>
2. <span data-ttu-id="f60bb-176">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-176">Close the page.</span></span>
3. <span data-ttu-id="f60bb-177">Eikite į Organizacijos administravimas > Elektroninės ataskaitos > Konfigūracijos.</span><span class="sxs-lookup"><span data-stu-id="f60bb-177">Go to Organization administration > Electronic reporting > Configurations.</span></span>
4. <span data-ttu-id="f60bb-178">Medyje išplėskite „Model for cheques“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-178">In the tree, expand 'Model for cheques'.</span></span>
5. <span data-ttu-id="f60bb-179">Medyje pasirinkite „Model for cheques\Cheques printing format“.</span><span class="sxs-lookup"><span data-stu-id="f60bb-179">In the tree, select 'Model for cheques\Cheques printing format'.</span></span>
6. <span data-ttu-id="f60bb-180">Spustelėkite Konstruktorius.</span><span class="sxs-lookup"><span data-stu-id="f60bb-180">Click Designer.</span></span>
7. <span data-ttu-id="f60bb-181">Spustelėkite Priedai.</span><span class="sxs-lookup"><span data-stu-id="f60bb-181">Click Attachments.</span></span>
8. <span data-ttu-id="f60bb-182">Spustelėkite Naikinti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-182">Click Delete.</span></span>
9. <span data-ttu-id="f60bb-183">Spustelėkite Taip.</span><span class="sxs-lookup"><span data-stu-id="f60bb-183">Click Yes.</span></span>
10. <span data-ttu-id="f60bb-184">Spustelėkite Naujas.</span><span class="sxs-lookup"><span data-stu-id="f60bb-184">Click New.</span></span>
11. <span data-ttu-id="f60bb-185">Spustelėkite Failas.</span><span class="sxs-lookup"><span data-stu-id="f60bb-185">Click File.</span></span>
    * <span data-ttu-id="f60bb-186">Spustelėkite Naršyti ir pasirinkite atsisiųstą iš anksto „Cheque template Word.docx" failą.</span><span class="sxs-lookup"><span data-stu-id="f60bb-186">Click Browse and select the downloaded in advance ‘Cheque template Word.docx’ file.</span></span>  
12. <span data-ttu-id="f60bb-187">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-187">Close the page.</span></span>
13. <span data-ttu-id="f60bb-188">Lauke Šablonas įveskite arba pasirinkite reikšmę.</span><span class="sxs-lookup"><span data-stu-id="f60bb-188">In the Template field, enter or select a value.</span></span>
14. <span data-ttu-id="f60bb-189">Spustelėkite Įrašyti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-189">Click Save.</span></span>
15. <span data-ttu-id="f60bb-190">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-190">Close the page.</span></span>
16. <span data-ttu-id="f60bb-191">Spustelėkite Redaguoti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-191">Click Edit.</span></span>
17. <span data-ttu-id="f60bb-192">Lauke Paleisti juodraštį pasirinkite Taip.</span><span class="sxs-lookup"><span data-stu-id="f60bb-192">Select Yes in the Run Draft field.</span></span>
18. <span data-ttu-id="f60bb-193">Uždarykite puslapį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-193">Close the page.</span></span>
19. <span data-ttu-id="f60bb-194">Pasirinkite Grynųjų pinigų ir banko valdymas > Banko kodai > Banko kodai.</span><span class="sxs-lookup"><span data-stu-id="f60bb-194">Go to Cash and bank management > Bank accounts > Bank accounts.</span></span>
20. <span data-ttu-id="f60bb-195">Naudokite spartųjį filtrą, kad filtruotumėte lauką Banko sąskaita reikšme „USMF OPER‟.</span><span class="sxs-lookup"><span data-stu-id="f60bb-195">Use the Quick Filter to filter on the Bank account field with a value of 'USMF OPER'.</span></span>
21. <span data-ttu-id="f60bb-196">Spustelėkite Tikrinti.</span><span class="sxs-lookup"><span data-stu-id="f60bb-196">Click Check.</span></span>
22. <span data-ttu-id="f60bb-197">Spustelėkite Spausdinti testą.</span><span class="sxs-lookup"><span data-stu-id="f60bb-197">Click Print test.</span></span>
23. <span data-ttu-id="f60bb-198">Spustelėkite GERAI.</span><span class="sxs-lookup"><span data-stu-id="f60bb-198">Click OK.</span></span>
    * <span data-ttu-id="f60bb-199">Peržiūrėkite sukurtą išvestį.</span><span class="sxs-lookup"><span data-stu-id="f60bb-199">Review the created output.</span></span> <span data-ttu-id="f60bb-200">Atkreipkite dėmesį, kad išvestis sugeneruota kaip „Microsoft Word“ dokumentas su įdėtaisiais vaizdais, pateikiant įmonės logotipą, įgalioto asmens parašą ir pažymėtą vandenženklio tekstą.</span><span class="sxs-lookup"><span data-stu-id="f60bb-200">Note that the output has been generated as a MS Word document with embedded images presenting the company logo, the signature of an authorized person and the selected text of the watermark.</span></span>  

