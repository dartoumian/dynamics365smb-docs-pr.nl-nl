---
title: Vaste activa herwaarderen| Microsoft Docs
description: Leren hoe u de waarde van vaste activa aanpast, nieuwe bedragen vastlegt als waardevermindering of waardevermeerdering en extra aanschafkosten boekt.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 5dd885d32c0ca08bdf51770669ee569c3a7a98ed
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="revalue-fixed-assets"></a><span data-ttu-id="179ed-103">Vaste activa herwaarderen</span><span class="sxs-lookup"><span data-stu-id="179ed-103">Revalue Fixed Assets</span></span>
<span data-ttu-id="179ed-104">De herwaardering van vaste activa kan bestaan uit waardevermeerderingen, waardeverminderingen of algemene waardecorrecties.</span><span class="sxs-lookup"><span data-stu-id="179ed-104">Revaluation of fixed assets can consist of appreciations, write-downs, or general value adjustments.</span></span>

<span data-ttu-id="179ed-105">Als de waarde van een vast activum is gestegen, boekt u een dagboekregel met een hoger bedrag, een waardevermeerdering, naar het afschrijvingsboek.</span><span class="sxs-lookup"><span data-stu-id="179ed-105">When the value of a fixed asset has increased, you post a journal line with a higher amount, an appreciation, to the depreciation book.</span></span> <span data-ttu-id="179ed-106">Het nieuwe bedrag wordt als een waardevermeerdering vastgelegd op basis van de instelling van de boeking van het vaste activum.</span><span class="sxs-lookup"><span data-stu-id="179ed-106">The new amount is recorded as an appreciation according to the fixed asset posting setup.</span></span>

<span data-ttu-id="179ed-107">Als de waarde van een vast activum is gedaald, boekt u een dagboekregel met een lager bedrag, een waardevermindering naar het afschrijvingsboek.</span><span class="sxs-lookup"><span data-stu-id="179ed-107">When the value of a fixed asset has decreased, you post a journal line with a lower amount, a write-down, to the depreciation book.</span></span> <span data-ttu-id="179ed-108">Het nieuwe bedrag wordt als een waardevermindering vastgelegd op basis van de instelling van de boeking van het vaste activum.</span><span class="sxs-lookup"><span data-stu-id="179ed-108">The new amount is recorded as a write-down according to the fixed asset posting setup.</span></span>

<span data-ttu-id="179ed-109">Indexering wordt gebruikt om meerdere waarden voor vaste activa aan te passen op basis van algemene prijswijzigingen.</span><span class="sxs-lookup"><span data-stu-id="179ed-109">Indexation is used to adjust multiple fixed asset values, for example per general price changes.</span></span> <span data-ttu-id="179ed-110">Met de batchverwerking **Vaste activa indexeren** kunt u diverse bedragen wijzigen, zoals waardeverminderingsbedragen en waardevermeerderingsbedragen.</span><span class="sxs-lookup"><span data-stu-id="179ed-110">The **Index Fixed Assets** batch job can be used to change various amounts, such as write-down and appreciation amounts.</span></span>

## <a name="to-post-an-appreciation-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="179ed-111">Een waardevermeerdering boeken vanuit het financieel dagboek voor vaste activa</span><span class="sxs-lookup"><span data-stu-id="179ed-111">To post an appreciation from the fixed asset G/L journal</span></span>
1. <span data-ttu-id="179ed-112">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **VA-fin. dagboeken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="179ed-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="179ed-113">Maak een eerste dagboekregel en vul de velden indien nodig in.</span><span class="sxs-lookup"><span data-stu-id="179ed-113">Create an initial journal line and fill in the fields as necessary.</span></span>
3. <span data-ttu-id="179ed-114">In het veld **VA-boekingssoort** selecteert u **Herwaardering**.</span><span class="sxs-lookup"><span data-stu-id="179ed-114">In the **FA Posting Type** field, select **Revaluation**.</span></span>
4. <span data-ttu-id="179ed-115">Kies de actie **VA-tegenrekening invoegen**.</span><span class="sxs-lookup"><span data-stu-id="179ed-115">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="179ed-116">Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van de waardevermeerdering is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="179ed-116">A second journal line is created for the balancing account that is set up for appreciation posting.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="179ed-117">Stap 4 werkt alleen als u het volgende hebt ingesteld: in het venster **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Waardevermeerderingsrekening** de gootboekdebetrekening en het veld **Tegenrekening waardevermeerdering** bevat de grootboekrekening waarnaar u tegenrekeningsposten voor waardevermeerdering wilt boeken.</span><span class="sxs-lookup"><span data-stu-id="179ed-117">Step 4 only works if you have set up the following: In the **FA Posting Group Card** window for the posting group of the fixed asset, the **Appreciation Account** field contains the general ledger debit account and the **Appreciation Bal. Account** field contains the general ledger account to which you want to post balancing entries for appreciation.</span></span> <span data-ttu-id="179ed-118">Zie het gedeelte 'Boekingsgroepen voor vaste activa instellen' in [Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="179ed-118">For more information, see the "To set up fixed asset posting groups" section in [Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>  
5. <span data-ttu-id="179ed-119">Kies de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="179ed-119">Choose the **Post** action.</span></span>

## <a name="to-post-a-write-down-from-the-fixed-asset-gl-journal"></a><span data-ttu-id="179ed-120">Een waardevermindering boeken vanuit het financieel dagboek voor vaste activa</span><span class="sxs-lookup"><span data-stu-id="179ed-120">To post a write-down from the fixed asset G/L journal</span></span>
1. <span data-ttu-id="179ed-121">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **VA-fin. dagboeken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="179ed-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="179ed-122">Maak een eerste dagboekregel en vul de velden indien nodig in.</span><span class="sxs-lookup"><span data-stu-id="179ed-122">Create an initial journal line, and fill in the fields as necessary.</span></span>
3. <span data-ttu-id="179ed-123">In het veld **VA-boekingssoort** selecteert u **Waardevermindering**.</span><span class="sxs-lookup"><span data-stu-id="179ed-123">In the **FA Posting Type** field, select **Write-Down**.</span></span>
4. <span data-ttu-id="179ed-124">Kies de actie **VA-tegenrekening invoegen**.</span><span class="sxs-lookup"><span data-stu-id="179ed-124">Choose the **Insert FA Bal. Account** action.</span></span> <span data-ttu-id="179ed-125">Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van de waardevermindering is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="179ed-125">A second journal line is created for the balancing account that is set up for write-down posting.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="179ed-126">Stap 4 werkt alleen als u het volgende hebt ingesteld: in het venster **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Waardeverminderingsrekening** de grootboekrekening en het veld **Waardeverminderingskostenrekening** bevat de grootboekdebetrekening waarnaar u tegenrekeningsposten voor waardeverminderingen wilt boeken.</span><span class="sxs-lookup"><span data-stu-id="179ed-126">Step 4 only works if you have set up the following: In the **FA Posting Group Card** window for the posting group of the fixed asset, the **Write-Down Account** field contains the general ledger credit account and the **Write-Down Expense Account** field contains the general ledger debit account to which you want to post balancing entries for write-downs.</span></span> <span data-ttu-id="179ed-127">Zie het gedeelte 'Boekingsgroepen voor vaste activa instellen' in [Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="179ed-127">For more information, see the "To set up fixed asset posting groups" section in [Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>
5. <span data-ttu-id="179ed-128">Kies de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="179ed-128">Choose the **Post** action.</span></span>

## <a name="to-perform-general-revaluation-of-fixed-assets"></a><span data-ttu-id="179ed-129">Algemene herwaardering van vaste activa uitvoeren</span><span class="sxs-lookup"><span data-stu-id="179ed-129">To perform general revaluation of fixed assets</span></span>
<span data-ttu-id="179ed-130">Indexering wordt gebruikt om meerdere waarden voor vaste activa aan te passen op basis van algemene prijswijzigingen.</span><span class="sxs-lookup"><span data-stu-id="179ed-130">Indexation is used to adjust multiple fixed asset values, for example per general price changes.</span></span> <span data-ttu-id="179ed-131">Met de batchverwerking **Vaste activa indexeren** kunt u diverse bedragen wijzigen, zoals waardeverminderingsbedragen en waardevermeerderingsbedragen.</span><span class="sxs-lookup"><span data-stu-id="179ed-131">The **Index Fixed Assets** batch job can be used to change various amounts, such as write-down and appreciation amounts.</span></span> <span data-ttu-id="179ed-132">Het selectievakje **Indexering toegestaan** in het venster **Afschrijvingsboek** moet zijn ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="179ed-132">The **Allow Indexation** check box in the **Depreciation Book** window must be selected.</span></span>

1. <span data-ttu-id="179ed-133">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vast activum indexeren** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="179ed-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Index Fixed Assets**, and then choose the related link.</span></span>  
2. <span data-ttu-id="179ed-134">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="179ed-134">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="179ed-135">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="179ed-135">Choose the **OK** button.</span></span>

    <span data-ttu-id="179ed-136">De herwaardering regels worden gemaakt op basis van uw instellingen in stap 2.</span><span class="sxs-lookup"><span data-stu-id="179ed-136">Revaluation lines are created per your settings in step 2.</span></span> <span data-ttu-id="179ed-137">De regels worden gemaakt in het dagboek voor vaste activa of het financieel dagboek voor vaste activa, afhankelijk van uw sjabloon en batchinstellingen in het venster **VA-dagboekinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="179ed-137">The lines are created in either the fixed asset journal or the fixed asset G/L journal, depending on your template and batch setup in the **FA Journal Setup** window.</span></span> <span data-ttu-id="179ed-138">Zie [Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="179ed-138">For more information, see [Set Up General Fixed Asset Information](fa-how-setup-general.md).</span></span>
4. <span data-ttu-id="179ed-139">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **VA-fin. dagboeken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="179ed-139">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **FA G/L Journals**, and then choose the related link.</span></span>  
5. <span data-ttu-id="179ed-140">Selecteer het dagboek met de vaste activa die u wilt herwaarderen en kies vervolgens de actie **Posten**.</span><span class="sxs-lookup"><span data-stu-id="179ed-140">Select the journal with the fixed assets that you want to revalue, and then choose the **Ledger Entries** action.</span></span>  
6. <span data-ttu-id="179ed-141">Controleer de gemaakte posten en kies vervolgens de actie **Boeken** om het dagboek te boeken.</span><span class="sxs-lookup"><span data-stu-id="179ed-141">Check the created entries, and then choose the **Post** action to post the journal.</span></span>

    > [!TIP]  
>   <span data-ttu-id="179ed-142">Als de indexcijfers alleen voor simulaties worden gebruikt, kunt u een speciaal afschrijvingsboek maken om ze in op te slaan.</span><span class="sxs-lookup"><span data-stu-id="179ed-142">If the index figures are for simulation purposes only, you can create a special depreciation book to store them in.</span></span> <span data-ttu-id="179ed-143">Deze posten zijn dan niet van invloed op de andere afschrijvingsboeken.</span><span class="sxs-lookup"><span data-stu-id="179ed-143">Then these entries will not affect any of the other depreciation books.</span></span>

   ## <a name="to-post-additional-acquisition-costs"></a><span data-ttu-id="179ed-144">Aanvullende aanschafkosten boeken</span><span class="sxs-lookup"><span data-stu-id="179ed-144">To post additional acquisition costs</span></span>
   <span data-ttu-id="179ed-145">U boekt extra aanschafkosten voor een vast activum op dezelfde manier als u de oorspronkelijke aanschafkosten boekt: vanaf een inkoopfactuur of vanuit een dagboek voor vaste activa.</span><span class="sxs-lookup"><span data-stu-id="179ed-145">You post additional acquisition cost for a fixed asset in the same way as you post the original acquisition cost: from a purchase invoice or from a fixed asset journal.</span></span> <span data-ttu-id="179ed-146">Zie [Vaste activa aanschaffen](fa-how-acquire.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="179ed-146">For more information, see [Acquire Fixed Assets](fa-how-acquire.md).</span></span>  

<span data-ttu-id="179ed-147">Als de afschrijving al is berekend voor het vaste activum, schakelt u het selectievakje **Afschrijving aanschafkosten** in om de extra aanschafkosten af te schrijven, verminderd met de restwaarde. Dit bedrag is evenredig aan het bedrag dat al op het eerder aangeschafte vaste activum is afgeschreven.</span><span class="sxs-lookup"><span data-stu-id="179ed-147">If depreciation has already been calculated for the fixed asset, select the **Depr. Acquisition Cost** check box to have the additional acquisition cost less the salvage value depreciated in proportion to the amount by which the previously acquired fixed asset has already been depreciated.</span></span> <span data-ttu-id="179ed-148">Hiermee wordt ervoor gezorgd dat de afschrijvingsperiode niet wordt gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="179ed-148">This ensures that the depreciation period is not changed.</span></span>  

<span data-ttu-id="179ed-149">Het afschrijvingspercentage wordt als volgt berekend:</span><span class="sxs-lookup"><span data-stu-id="179ed-149">The depreciation percentage is calculated as:</span></span>  

<span data-ttu-id="179ed-150">*P = (totale afschrijving x 100) / afschrijvingsbasis*</span><span class="sxs-lookup"><span data-stu-id="179ed-150">*P = (total depreciation x 100) / depreciable basis*</span></span>

<span data-ttu-id="179ed-151">*Afschrijvingsbedrag = (P/100) x (extra aanschafkosten - restwaarde)*</span><span class="sxs-lookup"><span data-stu-id="179ed-151">*Depreciation amount = (P/100) x (extra acquisition cost - salvage value)*</span></span>  

<span data-ttu-id="179ed-152">Vergeet niet om het selectievakje **Afschrijving tot VA-boekingsdatum** in te schakelen op de factuur en het financieel dagboek voor vaste activa of de dagboekregels voor vaste activa te selecteren om ervoor te zorgen dat de afschrijving wordt berekend vanaf de laatste boekingsdatum voor vaste activa tot de boekingsdatum van de aanvullende aanschafkosten.</span><span class="sxs-lookup"><span data-stu-id="179ed-152">Remember to select the **Depr. until FA Posting Date** check box on the invoice, the fixed asset G/L journal, or the fixed asset journal lines to ensure that depreciation is calculated from the last fixed asset posting date to the posting date of the additional acquisition cost.</span></span>

### <a name="example---posting-additional-acquisition-costs"></a><span data-ttu-id="179ed-153">Voorbeeld - aanvullende aanschafkosten boeken</span><span class="sxs-lookup"><span data-stu-id="179ed-153">Example - Posting Additional Acquisition Costs</span></span>
<span data-ttu-id="179ed-154">Een machine is aangeschaft op 1 augustus 2000.</span><span class="sxs-lookup"><span data-stu-id="179ed-154">A machine is purchased on August 1, 2000.</span></span> <span data-ttu-id="179ed-155">De aanschafkosten bedragen LV 4.800.</span><span class="sxs-lookup"><span data-stu-id="179ed-155">The acquisition cost is 4,800.</span></span> <span data-ttu-id="179ed-156">De afschrijvingsmethode is lineair over vier jaar.</span><span class="sxs-lookup"><span data-stu-id="179ed-156">The depreciation method is straight-line over four years.</span></span>

<span data-ttu-id="179ed-157">Op 31 augustus 2000 wordt de batchverwerking **Afschrijving berekenen** uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="179ed-157">On August 31, 2000, the **Calculate Depreciation** batch job is run.</span></span> <span data-ttu-id="179ed-158">De afschrijving wordt berekend als:</span><span class="sxs-lookup"><span data-stu-id="179ed-158">Depreciation is calculated as:</span></span>

<span data-ttu-id="179ed-159">*boekwaarde x aantal afschrijvingsdagen/totaal aantal afschrijvingsdagen = 4800 x 30 / 1440 = 100*</span><span class="sxs-lookup"><span data-stu-id="179ed-159">*book value x number of depreciation days / total number of depreciation days = 4800 x 30 / 1440 = 100*</span></span>  

<span data-ttu-id="179ed-160">Op 15 september 2000 wordt een factuur geboekt voor het schilderen van de machine.</span><span class="sxs-lookup"><span data-stu-id="179ed-160">On September 15, 2000, an invoice is posted for painting the machine.</span></span> <span data-ttu-id="179ed-161">Het factuurbedrag is LV 480.</span><span class="sxs-lookup"><span data-stu-id="179ed-161">The invoice amount is 480.</span></span>

<span data-ttu-id="179ed-162">Als u het selectievakje **Afschrijving tot VA-boekingsdatum** op de factuur hebt ingeschakeld voordat u deze boekt, wordt de volgende berekening gemaakt:</span><span class="sxs-lookup"><span data-stu-id="179ed-162">If you selected the **Depr. until FA Posting Date** check box on the invoice before posting, the following calculation is made:</span></span>  

<span data-ttu-id="179ed-163">15 afschrijvingsdagen (09-01-00 t/m 09-15-00) worden berekend als:</span><span class="sxs-lookup"><span data-stu-id="179ed-163">15 days of depreciation (from 09/01/00 to 09/15/00) is calculated as:</span></span>

<span data-ttu-id="179ed-164">*boekwaarde x aantal afschrijvingsdagen/resterend aantal afschrijvingsdagen = (4800 - 100) x 15 / 1410 = 50*</span><span class="sxs-lookup"><span data-stu-id="179ed-164">*book value x number of depreciation days / remaining number of depreciation days = (4800 - 100) x 15 / 1410 = 50*</span></span>

<span data-ttu-id="179ed-165">Als u het selectievakje **Afschrijving aanschafkosten** op de factuur hebt ingeschakeld voordat u deze boekt, wordt de volgende berekening gemaakt:</span><span class="sxs-lookup"><span data-stu-id="179ed-165">If you selected the **Depr. Acquisition Cost** check box on the invoice before posting, the following calculation is made:</span></span>  

<span data-ttu-id="179ed-166">*De extra aanschafkosten worden afgeschreven met ((150 x 100) / 4800) / 100 x 480 = 15*</span><span class="sxs-lookup"><span data-stu-id="179ed-166">*The additional acquisition cost is depreciated by ((150 x 100) / 4800) / 100 x 480 = 15*</span></span>

<span data-ttu-id="179ed-167">De afschrijvingsbasis is nu *5280 = (4800 + 480)* en de gecumuleerde afschrijving is *165 = (100 + 50 + 15)*, wat overeenkomt met 45 afschrijvingsdagen van de totale aanschafkosten.</span><span class="sxs-lookup"><span data-stu-id="179ed-167">The depreciable basis is now *5280 = (4800 + 480)*, and the accumulated depreciation is *165 = (100 + 50 + 15)*, corresponding to 45 days of depreciation of the total acquisition cost.</span></span> <span data-ttu-id="179ed-168">Dit betekent dat het activum volledig wordt afgeschreven binnen de verwachte levensduur van vier jaar.</span><span class="sxs-lookup"><span data-stu-id="179ed-168">This means that the asset will be totally depreciated within the estimated lifetime of four years.</span></span>  

<span data-ttu-id="179ed-169">Als de batchverwerking **Afschrijving berekenen** wordt uitgevoerd op 30-09-0, wordt de volgende berekening gemaakt:</span><span class="sxs-lookup"><span data-stu-id="179ed-169">When the **Calculate Depreciation** batch job is run on 09/30/00, the following calculation is made:</span></span>  

<span data-ttu-id="179ed-170">*Resterende afschrijfbare levensduur is 3 jaar, 10 maanden en 15 dagen = 1395 dagen*</span><span class="sxs-lookup"><span data-stu-id="179ed-170">*Remaining depreciable life is 3 years, 10 months and 15 days = 1395 days*</span></span>  

<span data-ttu-id="179ed-171">*Boekwaarde is (5.280 - 165) = LV 5115*</span><span class="sxs-lookup"><span data-stu-id="179ed-171">*Book value is (5280 - 165) = 5115*</span></span>  

<span data-ttu-id="179ed-172">*Afschrijvingsbedrag voor september 2000: 5115 x 15 / 1395 = 55,00*</span><span class="sxs-lookup"><span data-stu-id="179ed-172">*Depreciation amount for September 2000: 5115 x 15 / 1395 = 55.00*</span></span>  

<span data-ttu-id="179ed-173">*Totale afschrijving = 165 + 55 = 220*</span><span class="sxs-lookup"><span data-stu-id="179ed-173">*Total of depreciation = 165 + 55 = 220*</span></span>  

<span data-ttu-id="179ed-174">Als u het selectievakje **Afschrijving tot VA-boekingsdatum** niet hebt ingeschakeld, verliest het activum 15 afschrijvingsdagen omdat de batchverwerking **Afschrijving berekenen** die op 30-09-00 is uitgevoerd, de afschrijving berekent vanaf 15-09-00 t/m 30-09-00.</span><span class="sxs-lookup"><span data-stu-id="179ed-174">If you did not select the **Depr. until FA Posting Date** check box, the asset would lose 15 days of depreciation because the **Calculate Depreciation** batch job run on 09/30/00 would calculate depreciation from 09/15/00 to 09/30/00.</span></span> <span data-ttu-id="179ed-175">Als de batchverwerking **Afschrijving berekenen** op 30-09-00 wordt uitgevoerd, is de berekening dus als volgt:</span><span class="sxs-lookup"><span data-stu-id="179ed-175">This means that when the **Calculate Depreciation** batch job is run on 09/30/00, the calculation is as follows:</span></span>  

<span data-ttu-id="179ed-176">*Resterende levensduur is 3 jaar, 10 maanden en 15 dagen = 1395 dagen*</span><span class="sxs-lookup"><span data-stu-id="179ed-176">*Remaining life time is 3 years, 10 months and 15 days = 1395 days*</span></span>  

<span data-ttu-id="179ed-177">*Boekwaarde is (4.800 + 480 - 100 - 15) = LV 5165*</span><span class="sxs-lookup"><span data-stu-id="179ed-177">*Book value is (4800 + 480 - 100 - 15) = 5165*</span></span>

<span data-ttu-id="179ed-178">*Afschrijvingsbedrag voor september 2000: 5165 x 15 / 1395 = 55,54*</span><span class="sxs-lookup"><span data-stu-id="179ed-178">*Depreciation amount for September 2000: 5165 x 15 / 1395 = 55.54*</span></span>  

<span data-ttu-id="179ed-179">*Totale afschrijving = 100 +15 + 55,54 = 170,54*</span><span class="sxs-lookup"><span data-stu-id="179ed-179">*Total of depreciation = 100 + 15 + 55.54 = 170.54*</span></span>

## <a name="see-also"></a><span data-ttu-id="179ed-180">Zie ook</span><span class="sxs-lookup"><span data-stu-id="179ed-180">See Also</span></span>
[<span data-ttu-id="179ed-181">Vaste activa</span><span class="sxs-lookup"><span data-stu-id="179ed-181">Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="179ed-182">Vaste activa instellen</span><span class="sxs-lookup"><span data-stu-id="179ed-182">Setting Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="179ed-183">Financiën</span><span class="sxs-lookup"><span data-stu-id="179ed-183">Finance</span></span>](finance.md)  
<span data-ttu-id="179ed-184">[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="179ed-184">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="179ed-185">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="179ed-185">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
