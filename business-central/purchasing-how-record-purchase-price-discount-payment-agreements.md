---
title: Speciale en alternatieve leveranciersprijzen en -kortingen instellen | Microsoft Docs
description: "U kunt verschillende alternatieve prijzen en kortingen definiëren en deze toepassen op inkoopdocumenten voor leveranciers."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: special price, alternate price, pricing
ms.date: 07/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 021eac95fe22cfb37a6eaf851a5da11fd3ce9d30
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="record-special-purchase-prices-and-discounts"></a><span data-ttu-id="86a45-103">Speciale inkoopprijzen en kortingen registreren</span><span class="sxs-lookup"><span data-stu-id="86a45-103">Record Special Purchase Prices and Discounts</span></span>
<span data-ttu-id="86a45-104">De verschillende prijs- en kortingsovereenkomsten die van toepassing zijn wanneer u koopt van verschillende leveranciers, moeten worden gedefinieerd, zodat de overeengekomen regels en waarden worden toegepast op documenten die u voor de leveranciers maakt.</span><span class="sxs-lookup"><span data-stu-id="86a45-104">The different price and discount agreements that apply when you buy from different vendors must be defined so that the agreed rules and values are applied to purchase documents that you create for the vendors.</span></span>

<span data-ttu-id="86a45-105">Wanneer u speciale prijzen en regelkortingen voor verkopen en inkopen hebt geregistreerd, wordt er in [!INCLUDE[d365fin](includes/d365fin_md.md)] voor gezorgd dat uw winst op artikelhandel altijd optimaal is door de beste prijs op verkoop- en inkoopdocumenten en op project- en artikeldagboekregels automatisch te berekenen.</span><span class="sxs-lookup"><span data-stu-id="86a45-105">When you have recorded special prices and line discounts for sales and purchases, [!INCLUDE[d365fin](includes/d365fin_md.md)] ensures that your profit on item trade is always optimal by automatically calculating the best price on sales and purchase documents and on job and item journal lines.</span></span> <span data-ttu-id="86a45-106">Zie voor meer informatie de sectie "De beste prijs berekenen".</span><span class="sxs-lookup"><span data-stu-id="86a45-106">For more information, see the "Best Price Calculation" section.</span></span>

<span data-ttu-id="86a45-107">U kunt een speciale inkoopprijs op inkoopregels laten invoegen als een bepaalde combinatie bestaat van leverancier, artikel, minimumaantal, maateenheid of begin- en einddatum.</span><span class="sxs-lookup"><span data-stu-id="86a45-107">Concerning prices, you can have a special purchase price inserted on purchase lines if a certain combination of vendor, item, minimum quantity, unit of measure, or starting/ending date exists.</span></span>

<span data-ttu-id="86a45-108">U kunt twee soorten inkoopkortingen instellen en gebruiken:</span><span class="sxs-lookup"><span data-stu-id="86a45-108">Concerning discounts, you can set up and use two types of purchase discounts:</span></span>

| <span data-ttu-id="86a45-109">Type korting</span><span class="sxs-lookup"><span data-stu-id="86a45-109">Discount Type</span></span> | <span data-ttu-id="86a45-110">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="86a45-110">Description</span></span> |
| --- | --- |
| <span data-ttu-id="86a45-111">**Inkoopregelkorting**</span><span class="sxs-lookup"><span data-stu-id="86a45-111">**Purchase Line Discount**</span></span> |<span data-ttu-id="86a45-112">Een kortingsbedrag dat op inkoopregels wordt ingevoegd als een bepaalde combinatie bestaat van leverancier, artikel, minimumaantal, maateenheid of begin- en einddatum.</span><span class="sxs-lookup"><span data-stu-id="86a45-112">An amount discount that is inserted on purchase lines if a certain combination of vendor, item, minimum quantity, unit of measure, or starting/ending date exists.</span></span> <span data-ttu-id="86a45-113">Dit werkt op dezelfde manier als bij inkoopprijzen.</span><span class="sxs-lookup"><span data-stu-id="86a45-113">This works in the same way as for purchase prices.</span></span> |
| <span data-ttu-id="86a45-114">**Factuurkorting**</span><span class="sxs-lookup"><span data-stu-id="86a45-114">**Invoice Discount**</span></span> |<span data-ttu-id="86a45-115">Een percentagekorting die van het documenttotaal wordt afgetrokken als het waardebedrag van alle regels in een inkoopdocument een bepaald minimum overschrijdt.</span><span class="sxs-lookup"><span data-stu-id="86a45-115">A percentage discount that is subtracted from the document total if the value amount of all lines on a purchase document exceeds a certain minimum.</span></span> |

<span data-ttu-id="86a45-116">Omdat inkoopregelkortingen en inkoopprijzen gebaseerd zijn op een combinatie van artikel en leverancier, kunt u deze configuratie ook invoeren vanuit de artikelkaart, waarop de regels en waarden zijn gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="86a45-116">Because purchase line discounts and purchase prices are based on a combination of item and vendor, you can also enter this configuration from the item card, where the rules and values are defined.</span></span> <span data-ttu-id="86a45-117">Zie voor meer informatie [Nieuwe artikelen registreren](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="86a45-117">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span>

## <a name="to-set-up-a-special-purchase-price-for-a-vendor"></a><span data-ttu-id="86a45-118">Een speciale inkoopprijs voor een leverancier instellen</span><span class="sxs-lookup"><span data-stu-id="86a45-118">To set up a special purchase price for a vendor</span></span>
1. <span data-ttu-id="86a45-119">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="86a45-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="86a45-120">Open de desbetreffende leverancierskaart en kies vervolgens de actie **Prijzen**.</span><span class="sxs-lookup"><span data-stu-id="86a45-120">Open the relevant vendor card, and then choose the **Prices** action.</span></span>

    <span data-ttu-id="86a45-121">Het veld **Soort inkoop** wordt vooraf ingevuld met **Leverancier** en het veld **Inkoopcode** wordt vooraf ingevuld met het leveranciersnummer.</span><span class="sxs-lookup"><span data-stu-id="86a45-121">The **Purchase Type** field is prefilled with **Vendor**, and the **Purchase Code** field is prefilled with the vendor number.</span></span>
3. <span data-ttu-id="86a45-122">Vul de velden indien nodig op de regel in.</span><span class="sxs-lookup"><span data-stu-id="86a45-122">Fill in the fields on the line as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="86a45-123">Vul een regel in voor elke combinatie waarvoor de leverancier u een inkoopregelkorting verleent.</span><span class="sxs-lookup"><span data-stu-id="86a45-123">Fill a line for each combination for which the vendor grants you a purchase line discount.</span></span>

## <a name="to-set-up-a-line-discount-for-a-vendor"></a><span data-ttu-id="86a45-124">Een speciale regelkorting voor een leverancier instellen</span><span class="sxs-lookup"><span data-stu-id="86a45-124">To set up a line discount for a vendor</span></span>
1. <span data-ttu-id="86a45-125">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="86a45-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="86a45-126">Open de desbetreffende leverancierskaart en kies vervolgens de actie **Regelkortingen**.</span><span class="sxs-lookup"><span data-stu-id="86a45-126">Open the relevant vendor card, and then choose the **Line Discounts** action.</span></span>

    <span data-ttu-id="86a45-127">Het veld **Soort inkoop** wordt vooraf ingevuld met **Leverancier** en het veld **Inkoopcode** wordt vooraf ingevuld met het leveranciersnummer.</span><span class="sxs-lookup"><span data-stu-id="86a45-127">The **Purchase Type** field is prefilled with **Vendor**, and the **Purchase Code** field is prefilled with the vendor number.</span></span>
3. <span data-ttu-id="86a45-128">Vul de velden indien nodig op de regel in.</span><span class="sxs-lookup"><span data-stu-id="86a45-128">Fill in the fields on the line as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="86a45-129">Vul een regel in voor elke combinatie waarvoor de leverancier u een inkoopregelkorting verleent.</span><span class="sxs-lookup"><span data-stu-id="86a45-129">Fill a line for each combination for which the vendor grants you a purchase line discount.</span></span>

## <a name="to-set-up-an-invoice-discount-for-a-vendor"></a><span data-ttu-id="86a45-130">Een factuurkorting voor een leverancier instellen</span><span class="sxs-lookup"><span data-stu-id="86a45-130">To set up an invoice discount for a vendor</span></span>
<span data-ttu-id="86a45-131">Wanneer uw leveranciers u hebben geïnformeerd welke factuurkortingen ze verlenen, voert u de factuurkortingscodes op de leverancierskaarten in en stelt u de condities voor elke code in.</span><span class="sxs-lookup"><span data-stu-id="86a45-131">When your vendors have informed you which invoice discounts they grant, enter the invoice discount code on the vendor cards and set up the terms for each code.</span></span>

1. <span data-ttu-id="86a45-132">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="86a45-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="86a45-133">Open de leverancierskaart voor een leverancier die voor factuurkortingen in aanmerking komt.</span><span class="sxs-lookup"><span data-stu-id="86a45-133">Open the vendor card for a vendor that will be eligible for invoice discounts.</span></span>
3. <span data-ttu-id="86a45-134">Selecteer in het veld **Factuurkortingscode** een code voor de desbetreffende factuurkortingscondities om te gebruiken voor het berekenen van factuurkortingen voor de leverancier.</span><span class="sxs-lookup"><span data-stu-id="86a45-134">In the **Invoice Disc. Code** field, select a code for the relevant invoice discount terms to use to calculate invoice discounts for the vendor.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="86a45-135">Factuurkortingscodes worden weergegeven door bestaande leverancierskaarten.</span><span class="sxs-lookup"><span data-stu-id="86a45-135">Invoice discount codes are represented by existing vendor cards.</span></span> <span data-ttu-id="86a45-136">Zo kunt u snel factuurkortingscondities aan leveranciers toewijzen door de naam van een andere leverancier te kiezen die dezelfde condities heeft.</span><span class="sxs-lookup"><span data-stu-id="86a45-136">This enables you to quickly assign invoice discount terms to vendors by picking the name of another vendors who will have the same terms.</span></span>

    <span data-ttu-id="86a45-137">Ga door met het instellen van de condities voor de nieuwe inkoopfactuurkorting.</span><span class="sxs-lookup"><span data-stu-id="86a45-137">Proceed to set up new the purchase invoice discount terms.</span></span>
4. <span data-ttu-id="86a45-138">Kies in het venster **Leverancierskaart** de actie **Factuurkortingen**.</span><span class="sxs-lookup"><span data-stu-id="86a45-138">In the **Vendor Card** window, choose the **Invoice Discounts** action.</span></span> <span data-ttu-id="86a45-139">Het venster **Inkoopfactuurkortingen** verschijnt.</span><span class="sxs-lookup"><span data-stu-id="86a45-139">The **Vend. Invoice Discounts** window opens.</span></span>
5. <span data-ttu-id="86a45-140">Geef in het veld **Valutacode** de code op voor een valuta waarvoor de factuurkortingscondities op de regel van toepassing zijn.</span><span class="sxs-lookup"><span data-stu-id="86a45-140">In the **Currency Code** field, enter the code for a currency that the invoice discount terms on the line applies to.</span></span> <span data-ttu-id="86a45-141">Laat het veld leeg als u factuurkortingscondities in de lokale valuta wilt instellen.</span><span class="sxs-lookup"><span data-stu-id="86a45-141">Leave the field blank to set up invoice discount terms in USD.</span></span>
6. <span data-ttu-id="86a45-142">Geef in het veld **Minimumbedrag** op hoe hoog het factuurbedrag minimaal moet zijn voordat een korting wordt berekend.</span><span class="sxs-lookup"><span data-stu-id="86a45-142">In the **Minimum Amount** field, enter the minimum amount that an invoice must have to be eligible for the discount.</span></span>
7. <span data-ttu-id="86a45-143">Voer in het veld **Korting %** de factuurkorting in als percentage van het factuurbedrag.</span><span class="sxs-lookup"><span data-stu-id="86a45-143">In the **Discount %** field, enter the invoice discount as a percentage of the invoice amount.</span></span>
8. <span data-ttu-id="86a45-144">Herhaal stap 5 tot en met 7 voor elke valuta waarvoor de leverancier een andere factuurkorting ontvangt.</span><span class="sxs-lookup"><span data-stu-id="86a45-144">Repeat steps 5 through 7 for each currency that the vendor will receive a different invoice discount for.</span></span>

<span data-ttu-id="86a45-145">De factuurkorting is nu ingesteld en toegewezen aan de leverancier in kwestie.</span><span class="sxs-lookup"><span data-stu-id="86a45-145">The invoice discount is now set up and assigned to the vendor in question.</span></span> <span data-ttu-id="86a45-146">Wanneer u de leveranciercode selecteert in het veld **Factuurkortingscode** op andere leverancierskaarten, wordt dezelfde factuurkorting toegewezen aan die leverancier.</span><span class="sxs-lookup"><span data-stu-id="86a45-146">When you select the vendor code in the **Invoice Disc. Code** field on other vendor cards, the same invoice discount is assigned to those vendor.</span></span>

## <a name="to-choose-a-principle-for-posting-purchase-discounts"></a><span data-ttu-id="86a45-147">Een methode voor het boeken van inkoopkortingen kiezen</span><span class="sxs-lookup"><span data-stu-id="86a45-147">To choose a principle for posting purchase discounts</span></span>  
<span data-ttu-id="86a45-148">Wanneer u een inkoopfactuur boekt die een of meer kortingen bevat, kunt u de kortingsbedragen op twee manieren boeken.</span><span class="sxs-lookup"><span data-stu-id="86a45-148">When you post a purchase invoice that includes one or more discounts, you can choose between two principles for posting discount amounts.</span></span> <span data-ttu-id="86a45-149">U kunt kortingen apart boeken of kortingen van factuurbedragen aftrekken.</span><span class="sxs-lookup"><span data-stu-id="86a45-149">You can post discounts separately or you can subtract discounts from invoice discounts.</span></span>  

<span data-ttu-id="86a45-150">Voordat u dit kunt doen, moet u de benodigde rekeningen voor het boeken van kortingsbedragen in het rekeningschema al hebben ingesteld.</span><span class="sxs-lookup"><span data-stu-id="86a45-150">Before you can do this, you must have already set up the necessary accounts for posting discount amounts in the chart of accounts.</span></span> <span data-ttu-id="86a45-151">U moet ook controleren of u de juiste rekeningnummers hebt ingevoerd in de boekingsgroepinstellingen in de velden **Inkoopregelkortingsrekening** en **Inkoopfactuurkortingsrekening**.</span><span class="sxs-lookup"><span data-stu-id="86a45-151">You must also check that you have entered the correct account numbers in the general posting setup in the **Purch. Line Disc. Account** and **Purch. Inv. Disc. Account** fields.</span></span>

1. <span data-ttu-id="86a45-152">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopinstellingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="86a45-152">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="86a45-153">Kies in het veld **Korting boeken** een van de volgende principes voor het boeken van kortingen.</span><span class="sxs-lookup"><span data-stu-id="86a45-153">In the **Discount Posting** field, choose one of the following principles for posting discounts.</span></span>

|<span data-ttu-id="86a45-154">**Korting boeken**</span><span class="sxs-lookup"><span data-stu-id="86a45-154">**Discount Posting Principle**</span></span>|<span data-ttu-id="86a45-155">**Factuurkorting**</span><span class="sxs-lookup"><span data-stu-id="86a45-155">**Invoice Discount**</span></span>|<span data-ttu-id="86a45-156">**Regelkorting**</span><span class="sxs-lookup"><span data-stu-id="86a45-156">**Line Discount**</span></span>|  
|------------------------------------|--------------------------|-----------------------|  
|<span data-ttu-id="86a45-157">**Alle**</span><span class="sxs-lookup"><span data-stu-id="86a45-157">**All Discounts**</span></span>|<span data-ttu-id="86a45-158">Afzonderlijk geboekt</span><span class="sxs-lookup"><span data-stu-id="86a45-158">Posted separately</span></span>|<span data-ttu-id="86a45-159">Afzonderlijk geboekt</span><span class="sxs-lookup"><span data-stu-id="86a45-159">Posted separately</span></span>|  
|<span data-ttu-id="86a45-160">**Factuurkorting**</span><span class="sxs-lookup"><span data-stu-id="86a45-160">**Invoice Discounts**</span></span>|<span data-ttu-id="86a45-161">Afzonderlijk geboekt</span><span class="sxs-lookup"><span data-stu-id="86a45-161">Posted separately</span></span>|<span data-ttu-id="86a45-162">Ervan afgetrokken</span><span class="sxs-lookup"><span data-stu-id="86a45-162">Subtracted</span></span>|  
|<span data-ttu-id="86a45-163">**Regelkorting**</span><span class="sxs-lookup"><span data-stu-id="86a45-163">**Line Discounts**</span></span>|<span data-ttu-id="86a45-164">Ervan afgetrokken</span><span class="sxs-lookup"><span data-stu-id="86a45-164">Subtracted</span></span>|<span data-ttu-id="86a45-165">Afzonderlijk geboekt</span><span class="sxs-lookup"><span data-stu-id="86a45-165">Posted separately</span></span>|  
|<span data-ttu-id="86a45-166">**Geen kortingen**</span><span class="sxs-lookup"><span data-stu-id="86a45-166">**No Discounts**</span></span>|<span data-ttu-id="86a45-167">Ervan afgetrokken</span><span class="sxs-lookup"><span data-stu-id="86a45-167">Subtracted</span></span>|<span data-ttu-id="86a45-168">Ervan afgetrokken</span><span class="sxs-lookup"><span data-stu-id="86a45-168">Subtracted</span></span>|  

## <a name="purchase-invoice-discounts-and-service-charges"></a><span data-ttu-id="86a45-169">Inkoopfactuurkortingen en administratiekosten</span><span class="sxs-lookup"><span data-stu-id="86a45-169">Purchase Invoice Discounts and Service Charges</span></span>
<span data-ttu-id="86a45-170">Als u vaste afspraken met leveranciers hebt over kwantumkortingen, kunt u voor deze leveranciers de kortingsvoorwaarden invoeren.</span><span class="sxs-lookup"><span data-stu-id="86a45-170">If you have fixed terms for invoice discounts with any vendors, you can enter them for those vendors.</span></span> <span data-ttu-id="86a45-171">In dat geval wordt de korting berekend wanneer u een inkoopfactuur invult.</span><span class="sxs-lookup"><span data-stu-id="86a45-171">Then the discount will be calculated when you fill in a purchase invoice.</span></span>  

 <span data-ttu-id="86a45-172">Voordat u factuurkortingen voor inkoop kunt gebruiken, moet u aangeven van welke leveranciers u de kortingen ontvangt.</span><span class="sxs-lookup"><span data-stu-id="86a45-172">Before you can use invoice discounts with purchases, you must specify the vendors that offer you the discounts.</span></span>  

 <span data-ttu-id="86a45-173">U koppelt kortingspercentages aan specifieke factuurbedragen in het venster **Inkoopfactuurkortingen**.</span><span class="sxs-lookup"><span data-stu-id="86a45-173">You link discount percentages to specific invoice amounts in **Vend. Invoice Discounts** windows.</span></span> <span data-ttu-id="86a45-174">U kunt een willekeurig aantal percentages invoeren in elk venster.</span><span class="sxs-lookup"><span data-stu-id="86a45-174">You can enter any number of percentages in each window.</span></span> <span data-ttu-id="86a45-175">U kunt voor elke leverancier een eigen venster hebben, of u kunt verschillende leveranciers aan hetzelfde venster koppelen.</span><span class="sxs-lookup"><span data-stu-id="86a45-175">Each vendor can have its own window, or you can link several vendors to the same window.</span></span>  

 <span data-ttu-id="86a45-176">Naast een kortingspercentage kunt u een bedrag voor administratiekosten aan een specifiek factuurbedrag koppelen.</span><span class="sxs-lookup"><span data-stu-id="86a45-176">In addition to a discount percentage, you can link a service charge amount to a specific invoice amount.</span></span>  

 <span data-ttu-id="86a45-177">U kunt de condities voor de factuurkorting definiëren in de lokale valuta voor binnenlandse leveranciers en in vreemde valuta's voor buitenlandse leveranciers.</span><span class="sxs-lookup"><span data-stu-id="86a45-177">You can define the terms of the invoice discount in LCY for domestic vendors and in foreign currency for foreign vendors.</span></span>  

 <span data-ttu-id="86a45-178">U kunt aangeven dat de factuurkortingen automatisch door [!INCLUDE[d365fin](includes/d365fin_md.md)] moeten worden berekend voor offertes, raamcontracten, orders, facturen of creditnota's.</span><span class="sxs-lookup"><span data-stu-id="86a45-178">You can choose to have [!INCLUDE[d365fin](includes/d365fin_md.md)] automatically calculate the invoice discounts for quotes, blanket orders, orders, invoices, or credit memos.</span></span>  

> [!TIP]  
>  <span data-ttu-id="86a45-179">Voordat u deze gegevens invoert, kunt u het beste een ontwerp maken van de kortingsstructuur die u wilt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="86a45-179">Before you enter this information, it is a good idea to prepare an outline of the discount structure that you want to use.</span></span> <span data-ttu-id="86a45-180">Zo ziet u vrijwel meteen welke leveranciers aan hetzelfde factuurkortingsvenster kunnen worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="86a45-180">This makes it easier to see which vendors can be linked to the same invoice discount window.</span></span> <span data-ttu-id="86a45-181">Hoe minder vensters u hebt ingesteld, des te sneller kunt u de basisgegevens invoeren.</span><span class="sxs-lookup"><span data-stu-id="86a45-181">The fewer windows that you have to set up, the faster that you can enter the basic information.</span></span>

## <a name="best-price-calculation"></a><span data-ttu-id="86a45-182">Berekening van beste prijs</span><span class="sxs-lookup"><span data-stu-id="86a45-182">Best Price Calculation</span></span>
<span data-ttu-id="86a45-183">Wanneer u speciale prijzen en regelkortingen voor verkopen en inkopen hebt geregistreerd, wordt er in [!INCLUDE[d365fin](includes/d365fin_md.md)] voor gezorgd dat uw winst op artikelhandel altijd optimaal is door de beste prijs op verkoop- en inkoopdocumenten en op project- en artikeldagboekregels automatisch te berekenen.</span><span class="sxs-lookup"><span data-stu-id="86a45-183">When you have recorded special prices and line discounts for sales and purchases, [!INCLUDE[d365fin](includes/d365fin_md.md)] ensures that your profit on item trade is always optimal by automatically calculating the best price on sales and purchase documents and on job and item journal lines.</span></span>

<span data-ttu-id="86a45-184">De beste prijs is de laagst toegestane prijs met de hoogst toegestane regelkorting op een bepaalde datum.</span><span class="sxs-lookup"><span data-stu-id="86a45-184">The best price is the lowest permissible price with the highest permissible line discount on a given date.</span></span> <span data-ttu-id="86a45-185">In [!INCLUDE[d365fin](includes/d365fin_md.md)] wordt dit automatisch berekend wanneer de eenheidsprijs en het regelkortingspercentage voor artikelen op nieuwe document- en dagboekregels worden ingevoegd.</span><span class="sxs-lookup"><span data-stu-id="86a45-185">[!INCLUDE[d365fin](includes/d365fin_md.md)] automatically calculates this when it inserts the unit price and the line discount percentage for items on new document and journal lines.</span></span>

> [!NOTE]  
>   <span data-ttu-id="86a45-186">Hierna wordt beschreven hoe de beste prijs voor verkoop wordt berekend.</span><span class="sxs-lookup"><span data-stu-id="86a45-186">The following describes how the best price is calculated for sales.</span></span> <span data-ttu-id="86a45-187">De berekening is hetzelfde voor inkopen.</span><span class="sxs-lookup"><span data-stu-id="86a45-187">The calculation is the same for purchases.</span></span>

1. <span data-ttu-id="86a45-188">In [!INCLUDE[d365fin](includes/d365fin_md.md)] wordt de combinatie van de factuurklant en het artikel gecontroleerd en vervolgens worden de eenheidsprijs en het regelkortingspercentage die van toepassing zijn berekend op basis van de volgende criteria:</span><span class="sxs-lookup"><span data-stu-id="86a45-188">[!INCLUDE[d365fin](includes/d365fin_md.md)] checks the combination of the bill-to customer and the item and then calculates the applicable unit price and line discount percentage, using the following criteria:</span></span>

    - <span data-ttu-id="86a45-189">Is er een prijs-/kortingsafspraak voor de klant of behoort de klant tot een groep waarvoor een dergelijke afspraak geldt?</span><span class="sxs-lookup"><span data-stu-id="86a45-189">Does the customer have a price/discount agreement, or does the customer belong to a group that does?</span></span>
    - <span data-ttu-id="86a45-190">Zijn er dergelijke prijs-/kortingsafspraken van toepassing op het artikel of de artikelkortingsgroep op de regel?</span><span class="sxs-lookup"><span data-stu-id="86a45-190">Is the item or the item discount group on the line included in any of these price/discount agreements?</span></span>
    - <span data-ttu-id="86a45-191">Valt de besteldatum (of de boekingsdatum van de factuur en creditnota) binnen de begin- en einddatum van de prijs-/kortingsafspraak?</span><span class="sxs-lookup"><span data-stu-id="86a45-191">Is the order date (or the posting date for the invoice and credit memo) within the starting and ending date of the price/discount agreement?</span></span>
    - <span data-ttu-id="86a45-192">Is er een eenheidscode opgegeven?</span><span class="sxs-lookup"><span data-stu-id="86a45-192">Is a unit of measure code specified?</span></span> <span data-ttu-id="86a45-193">In dat geval controleert [!INCLUDE[d365fin](includes/d365fin_md.md)] op prijzen/kortingen met dezelfde eenheidscode en op prijzen/kortingen zonder eenheidscode.</span><span class="sxs-lookup"><span data-stu-id="86a45-193">If so, [!INCLUDE[d365fin](includes/d365fin_md.md)] checks for prices/discounts with the same unit of measure code, and prices/discounts with no unit of measure code.</span></span>

2. [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="86a45-194"> controleert of eventuele prijs-/kortingsafspraken van toepassing zijn op gegevens in het document of de dagboekregel, en voegt vervolgens de betreffende eenheidsprijs en het regelkortingspercentage in op basis van de volgende criteria:</span><span class="sxs-lookup"><span data-stu-id="86a45-194"> checks if any price/discount agreements apply to information on the document or journal line, and then inserts the applicable unit price and line discount percentage, using the following criteria:</span></span>

    - <span data-ttu-id="86a45-195">Is er een minimale hoeveelheidsvereiste in de prijs-/kortingsafspraak waaraan wordt voldaan?</span><span class="sxs-lookup"><span data-stu-id="86a45-195">Is there a minimum quantity requirement in the price/discount agreement that is fulfilled?</span></span>
    - <span data-ttu-id="86a45-196">Is er een valutavereiste in de prijs-/kortingsafspraak waaraan wordt voldaan?</span><span class="sxs-lookup"><span data-stu-id="86a45-196">Is there a currency requirement in the price/discount agreement that is fulfilled?</span></span> <span data-ttu-id="86a45-197">Zo ja, dan worden de laagste prijs en de hoogste regelkorting voor deze valuta ingevoegd, zelfs als de lokale valuta een betere prijs geeft.</span><span class="sxs-lookup"><span data-stu-id="86a45-197">If so, the lowest price and the highest line discount for that currency are inserted, even if LCY would provide a better price.</span></span> <span data-ttu-id="86a45-198">Als er geen prijs-/kortingsafspraak voor de opgegeven valutacode is, worden in [!INCLUDE[d365fin](includes/d365fin_md.md)] de laagste prijs en de hoogste regelkorting in lokale valuta ingevoegd.</span><span class="sxs-lookup"><span data-stu-id="86a45-198">If there is no price/discount agreement for the specified currency code, [!INCLUDE[d365fin](includes/d365fin_md.md)] inserts the lowest price and the highest line discount in LCY.</span></span>

<span data-ttu-id="86a45-199">Als er geen speciale prijs kan worden berekend voor het artikel op de regel, worden de laatste directe kosten of de eenheidsprijs van de artikelkaart ingevoegd.</span><span class="sxs-lookup"><span data-stu-id="86a45-199">If no special price can be calculated for the item on the line, then either the last direct cost or the unit price from the item card is inserted.</span></span>

## <a name="see-also"></a><span data-ttu-id="86a45-200">Zie ook</span><span class="sxs-lookup"><span data-stu-id="86a45-200">See Also</span></span>
[<span data-ttu-id="86a45-201">Inkoop instellen</span><span class="sxs-lookup"><span data-stu-id="86a45-201">Setting Up Purchasing</span></span>](purchasing-setup-purchasing.md)  
[<span data-ttu-id="86a45-202">Inkoop</span><span class="sxs-lookup"><span data-stu-id="86a45-202">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="86a45-203">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="86a45-203">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
