---
title: "Leveranciersbetalingen handmatig reconciliëren| Microsoft Docs"
description: Als u leveranciersbetalingen of terugbetalingen handmatig wilt verwerken, vereffent u het bedrag met een of meer openstaande leveranciersposten.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment application, payment processing, match payments
ms.date: 06/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f6b0ab4131f26a91953b28991276d3a19a8918ad
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="reconcile-vendor-payments-manually"></a><span data-ttu-id="4d113-103">Leveranciersbetalingen handmatig reconciliëren</span><span class="sxs-lookup"><span data-stu-id="4d113-103">Reconcile Vendor Payments Manually</span></span>
<span data-ttu-id="4d113-104">Wanneer u een betaling of terugbetaling van een leverancier ontvangt, moet u beslissen of u de betaling of terugbetaling vereffent met een of meer openstaande posten.</span><span class="sxs-lookup"><span data-stu-id="4d113-104">When you send a payment or receive a refund from a vendor, you must decide whether to apply the payment or refund to one or more open entries.</span></span> <span data-ttu-id="4d113-105">U kunt het exacte bedrag opgeven waarmee u de betalingsontvangst of terugbetaling wilt vereffenen, en de leveranciersposten vervolgens slechts gedeeltelijk vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-105">You can specify the exact amount that you want to apply to the payment receipt or refund, and then only partially apply vendor ledger entries.</span></span> <span data-ttu-id="4d113-106">U moet alle leveranciersposten vereffenen om correcte leverancierstatistieken en -rapporten te verkrijgen van de rekeningoverzichten en rentefacturen.</span><span class="sxs-lookup"><span data-stu-id="4d113-106">You must apply all vendor ledger entries to obtain correct vendor statistics and reports of the account statements and finance charges.</span></span>

> [!NOTE]  
>   <span data-ttu-id="4d113-107">Leveranciers geven soms een terugbetaling in plaats van een creditnota die als tegenrekening dient voor toekomstige facturen, met name wanneer u artikelen terugzendt die u al hebt betaald of wanneer u te veel hebt betaald voor een factuur.</span><span class="sxs-lookup"><span data-stu-id="4d113-107">Vendors may sometimes give a payment refund instead of a credit memo to offset against future invoices, especially when you return items that you have already paid for or when you have overpaid an invoice.</span></span>

<span data-ttu-id="4d113-108">U kunt als volgt leveranciersposten vereffenen op drie verschillende manieren:</span><span class="sxs-lookup"><span data-stu-id="4d113-108">You can apply vendor ledger entries in three different ways:</span></span>

* <span data-ttu-id="4d113-109">Door gegevens in bepaalde vensters in te voeren, zoals het venster **Betalingsdagboek** en het venster **Dagboek betalingsreconciliatie**.</span><span class="sxs-lookup"><span data-stu-id="4d113-109">By entering information in dedicated windows, such as the **Payment Journal** window and the **Payment Reconciliation Journal** window.</span></span>
* <span data-ttu-id="4d113-110">Vanuit inkoopcreditnotadocumenten.</span><span class="sxs-lookup"><span data-stu-id="4d113-110">From purchase credit memo documents.</span></span>
* <span data-ttu-id="4d113-111">Vanuit leveranciersposten, nadat inkoopdocumenten zijn geboekt maar nog niet vereffend.</span><span class="sxs-lookup"><span data-stu-id="4d113-111">From vendor ledger entries after purchase documents are posted but not applied.</span></span>

> [!NOTE]  
>   <span data-ttu-id="4d113-112">Als het veld **Vereffeningsmethode** op de leverancierskaart **Saldo** bevat, kunnen betalingen handmatig worden vereffend met de oudste openstaande creditpost, als u niet handmatig opgeeft met welke post moet worden vereffend.</span><span class="sxs-lookup"><span data-stu-id="4d113-112">If the **Application Method** field on the vendor card contains **Apply to Oldest**, then payments will automatically be applied to the oldest open credit entry if you do not manually specify which entry to apply to.</span></span> <span data-ttu-id="4d113-113">Als de vereffeningsmethode voor een klant **Handmatig** is, moet u posten handmatig vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-113">If the application method for a customer is **Manual**, then you must apply entries manually.</span></span>

<span data-ttu-id="4d113-114">U kunt leveranciersbetalingen handmatig op de gerelateerde inkoopdocumenten toepassen wanneer u de betalingen boekt in het venster **Betalingsdagboek**.</span><span class="sxs-lookup"><span data-stu-id="4d113-114">You can apply vendor payments manually to their related purchase documents when you post the payments in the **Payment Journal** window.</span></span> <span data-ttu-id="4d113-115">Zie voor meer informatie over het invullen van het betalingsdagboek [Betalingen uitvoeren](payables-make-payments.md).</span><span class="sxs-lookup"><span data-stu-id="4d113-115">For information about filling the payment journal, see [Making Payments](payables-make-payments.md).</span></span>

<span data-ttu-id="4d113-116">U kunt ook leveranciersbetalingen en klantbetalingen vereffenen nadat de betalingen worden weergegeven als negatieve banktransacties bij uw bank.</span><span class="sxs-lookup"><span data-stu-id="4d113-116">You can also apply vendor payments, and customer payments, after the payments appear as negative bank transactions in your bank.</span></span> <span data-ttu-id="4d113-117">In het venster **Dagboek betalingsreconciliatie** kunt u functies voor het importeren van bankafschriften, automatische vereffening en bankrekeningvereffening gebruiken.</span><span class="sxs-lookup"><span data-stu-id="4d113-117">In the **Payment Reconciliation Journal** window, you can use functions for bank statement import, automatic application, and bank account reconciliation.</span></span> <span data-ttu-id="4d113-118">Zie voor meer informatie [Betalingen vereffenen met automatische vereffening](receivables-how-reconcile-payments-auto-application.md).</span><span class="sxs-lookup"><span data-stu-id="4d113-118">For more information, see [Reconcile Payments Using Automatic Application](receivables-how-reconcile-payments-auto-application.md).</span></span>

## <a name="to-apply-a-payment-to-a-single-or-multiple-vendor-ledger-entries"></a><span data-ttu-id="4d113-119">Een betaling vereffenen met een of meer leveranciersposten</span><span class="sxs-lookup"><span data-stu-id="4d113-119">To apply a payment to a single or multiple vendor ledger entries</span></span>
1. <span data-ttu-id="4d113-120">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Betalingsdagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4d113-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d113-121">Voer in het venster **Betalingsdagboek** op de eerste dagboekregel de betreffende gegevens over de betalingspost in.</span><span class="sxs-lookup"><span data-stu-id="4d113-121">In the **Payment Journal** window, on the first journal line, enter the relevant information about the payment entry.</span></span>
3. <span data-ttu-id="4d113-122">Eén leverancierspost vereffenen:</span><span class="sxs-lookup"><span data-stu-id="4d113-122">To apply a single vendor ledger entry:</span></span>
   1. <span data-ttu-id="4d113-123">Selecteer in het veld **Vereffeningsnr.** het veld voor het openen van het venster **Leveranciersposten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-123">In the **Applies-to Doc. No.** field, choose the field to open the **Apply Vendor Entries** window.</span></span>
   2. <span data-ttu-id="4d113-124">Selecteer in het venster **Leveranciersposten vereffenen** de post waarmee de betaling moet worden vereffend.</span><span class="sxs-lookup"><span data-stu-id="4d113-124">In the **Apply Vendor Entries** window, select the entry to apply the payment to.</span></span>
   3. <span data-ttu-id="4d113-125">Voer op de regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de post wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-125">On the line in the **Amount to Apply** field, enter the amount to apply to the entry.</span></span>
4. <span data-ttu-id="4d113-126">Of meerdere leveranciersposten vereffenen:</span><span class="sxs-lookup"><span data-stu-id="4d113-126">Or, to apply multiple vendor ledger entries:</span></span>

   1. <span data-ttu-id="4d113-127">Kies de actie **Posten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-127">Choose the **Apply Entries** action.</span></span>
   2. <span data-ttu-id="4d113-128">In het venster **Leveranciersposten vereffenen** selecteert u de regels met de posten die u met de betaling wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-128">In the **Apply Vendor Entries** window, select the lines with the entries to apply the payment to.</span></span>
   3. <span data-ttu-id="4d113-129">Kies de actie **Id toekennen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-129">Choose the **Set Applies-to ID** action.</span></span>  
   4. <span data-ttu-id="4d113-130">Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-130">On each line in the **Amount to Apply** field, enter the amount to apply to the individual entry.</span></span>

      <span data-ttu-id="4d113-131">Als u geen bedrag opgeeft, wordt automatisch het maximumbedrag gebruikt.</span><span class="sxs-lookup"><span data-stu-id="4d113-131">If you do not enter an amount, then the maximum amount is automatically applied.</span></span> <span data-ttu-id="4d113-132">Onder aan het venster **Leveranciersposten vereffenen** ziet u het bedrag in het veld Vereffend bedrag en kunt u controleren of de vereffening sluitend is.</span><span class="sxs-lookup"><span data-stu-id="4d113-132">At the bottom of the **Apply Vendor Entries** window, you can see the amount in the Applied Amount field, and you can see whether the application balances.</span></span>
5. <span data-ttu-id="4d113-133">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="4d113-133">Choose the **OK** button.</span></span>
6. <span data-ttu-id="4d113-134">Kies de actie **Boeken** om het betalingsdagboek te boeken.</span><span class="sxs-lookup"><span data-stu-id="4d113-134">Choose the **Post** action to post the payment journal.</span></span>

## <a name="to-apply-a-credit-memo-to-a-single-or-multiple-vendor-ledger-entries"></a><span data-ttu-id="4d113-135">Een creditnota vereffenen met een of meer leveranciersposten:</span><span class="sxs-lookup"><span data-stu-id="4d113-135">To apply a credit memo to a single or multiple vendor ledger entries</span></span>
1. <span data-ttu-id="4d113-136">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoop - Creditnota** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4d113-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Credit Memo**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d113-137">Open de creditnota die u wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-137">Open the credit memo that you want to apply.</span></span>
3. <span data-ttu-id="4d113-138">Voer de betreffende gegevens in de kop in.</span><span class="sxs-lookup"><span data-stu-id="4d113-138">Enter the relevant information in the header.</span></span>
4. <span data-ttu-id="4d113-139">Als u een enkele leverancierspost wilt vereffenen, selecteert u op het sneltabblad **Vereffening** in het veld **Vereffeningsnr.**, de post waarmee u het krediet wilt vereffenen. In het veld **Te vereffenen bedrag** voert u vervolgens het bedrag in waarmee de post moet worden vereffend.</span><span class="sxs-lookup"><span data-stu-id="4d113-139">To apply a single vendor ledger entry, on the **Application** FastTab, in the **Applies-to Doc. No.** field, select the entry to apply the credit to, and then, in the **Amount to Apply** field, enter the amount to apply to the entry.</span></span>
5. <span data-ttu-id="4d113-140">Of meerdere leveranciersposten vereffenen:</span><span class="sxs-lookup"><span data-stu-id="4d113-140">Or, to apply multiple vendor ledger entries:</span></span>

   1. <span data-ttu-id="4d113-141">Kies de actie **Posten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-141">Choose the **Apply Entries** action.</span></span>
   2. <span data-ttu-id="4d113-142">Selecteer de regels met de posten waarmee u de creditnota wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-142">Select the lines with the entries to apply the credit memo to.</span></span>
   3. <span data-ttu-id="4d113-143">Kies de actie **Id toekennen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-143">Choose the **Set Applies-to ID** action.</span></span>  
   4. <span data-ttu-id="4d113-144">Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-144">On each line in the **Amount to Apply** field, enter the amount to apply to the individual entry.</span></span>

       <span data-ttu-id="4d113-145">Als u geen bedrag opgeeft, wordt automatisch het maximumbedrag gebruikt.</span><span class="sxs-lookup"><span data-stu-id="4d113-145">If you do not enter an amount, then the maximum amount is automatically applied.</span></span> <span data-ttu-id="4d113-146">Onder aan het venster **Leveranciersposten vereffenen** ziet u het bedrag in het veld **Vereffend bedrag** en kunt u controleren of de vereffening sluitend is.</span><span class="sxs-lookup"><span data-stu-id="4d113-146">At the bottom of the **Apply Vendor Entries** window, you can see the amount in the **Applied Amount** field, and you can see whether the application balances.</span></span>
6. <span data-ttu-id="4d113-147">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="4d113-147">Choose the **OK** button.</span></span>  
   <span data-ttu-id="4d113-148">Het venster **Inkoopcreditnota** bevat de post die u hebt geselecteerd in de velden **Vereffeningssoort** en **Vereffeningsnr.**</span><span class="sxs-lookup"><span data-stu-id="4d113-148">The **Purchase Credit Memo** window shows the entry that you have selected in the **Applies-to Doc. Type** field and the **Applies-to Doc. No.** field.</span></span> <span data-ttu-id="4d113-149">Het venster bevat ook het bedrag van de creditnota dat moet worden geboekt, geherwaardeerd voor de mogelijke contantkortingen.</span><span class="sxs-lookup"><span data-stu-id="4d113-149">The window also shows the amount of the credit memo to be posted, adjusted for any payment discounts.</span></span>
7. <span data-ttu-id="4d113-150">Kies de knop **Boeken** om de inkoopcreditnota te boeken.</span><span class="sxs-lookup"><span data-stu-id="4d113-150">Choose the **Post** button to post the purchase credit memo.</span></span>

## <a name="to-apply-posted-vendor-ledger-entries"></a><span data-ttu-id="4d113-151">Geboekte leveranciersposten vereffenen</span><span class="sxs-lookup"><span data-stu-id="4d113-151">To apply posted vendor ledger entries</span></span>
1. <span data-ttu-id="4d113-152">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4d113-152">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d113-153">Open de betreffende leverancier met posten die reeds zijn geboekt.</span><span class="sxs-lookup"><span data-stu-id="4d113-153">Open the relevant vendor with entries that have already been posted.</span></span>
3. <span data-ttu-id="4d113-154">Kies de actie **Posten** en kies vervolgens de actie **Posten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-154">Choose the **Ledger Entries** action, and then choose the **Apply Entries** action.</span></span>
4. <span data-ttu-id="4d113-155">In het venster **Leveranciersposten vereffenen** ziet u de openstaande posten voor de leverancier.</span><span class="sxs-lookup"><span data-stu-id="4d113-155">In the **Apply Vendor Entries** window, you can see the open entries for the vendor.</span></span>
5. <span data-ttu-id="4d113-156">Selecteer de regel met de post die wordt vereffend.</span><span class="sxs-lookup"><span data-stu-id="4d113-156">Select the line with the entry that will be applied.</span></span>
6. <span data-ttu-id="4d113-157">Kies de actie **Id toekennen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-157">Choose the **Set Applies-to ID** action.</span></span>

    <span data-ttu-id="4d113-158">Het veld **Vereffenings-id** bevat drie sterretjes als u in een systeem met één gebruiker werkt, of bevat uw gebruikers-id als u in een systeem met meerdere gebruikers werkt.</span><span class="sxs-lookup"><span data-stu-id="4d113-158">The **Applies-to ID** field displays three asterisks if you work in a single-user system or your user ID if you work in a multiuser system.</span></span>  
7. <span data-ttu-id="4d113-159">Voer op elke regel in het veld **Te vereffenen bedrag** het bedrag in waarmee u de afzonderlijke post wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-159">For each line in the **Amount to Apply** field, enter the amount to apply to the individual entry.</span></span>

    <span data-ttu-id="4d113-160">Als u geen bedrag opgeeft, wordt automatisch het maximumbedrag gebruikt.</span><span class="sxs-lookup"><span data-stu-id="4d113-160">If you do not enter an amount, then the maximum amount is automatically applied.</span></span> <span data-ttu-id="4d113-161">U ziet het bedrag in het veld **Vereffend bedrag**, onder aan het venster **Leveranciersposten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-161">You can see the amount in the **Applied Amount** field at the bottom of the **Apply Vendor Entries** window.</span></span>
8. <span data-ttu-id="4d113-162">Kies de actie **Vereffening boeken**.</span><span class="sxs-lookup"><span data-stu-id="4d113-162">Choose the **Post Application** action.</span></span>  

    <span data-ttu-id="4d113-163">Het venster **Vereffening boeken** verschijnt met het documentnummer van de vereffeningspost en de boekingsdatum van de post met de meest recente boekingsdatum.</span><span class="sxs-lookup"><span data-stu-id="4d113-163">The **Post Application** window opens with the document number of the applying entry and the posting date of the entry with the most recent posting date.</span></span>
9. <span data-ttu-id="4d113-164">Kies de knop **OK** om de vereffening te boeken.</span><span class="sxs-lookup"><span data-stu-id="4d113-164">Choose the **OK** button to post the application.</span></span>

## <a name="to-apply-vendor-ledger-entries-in-different-currencies-to-one-another"></a><span data-ttu-id="4d113-165">Leveranciersposten in verschillende valuta's onderling vereffenen</span><span class="sxs-lookup"><span data-stu-id="4d113-165">To apply vendor ledger entries in different currencies to one another</span></span>
<span data-ttu-id="4d113-166">Als u van een leverancier koopt in de ene valuta en betaalt in de andere, kunt u de factuur toch met de betaling vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-166">If you buy from a vendor in one currency and make payment in another currency, you can still apply the invoice to the payment.</span></span>

<span data-ttu-id="4d113-167">Als u een post (Post 1) in de ene valuta vereffent met een post (Post 2) in een andere valuta, wordt de boekingsdatum van Post 1 gebruikt om de juiste wisselkoers te bepalen voor de conversie van de bedragen van Post 2.</span><span class="sxs-lookup"><span data-stu-id="4d113-167">If you apply an entry (Entry 1) in one currency to an entry (Entry 2) in a different currency, the posting date on Entry 1 is used to find the relevant exchange rate to convert amounts on Entry 2.</span></span> <span data-ttu-id="4d113-168">De juiste wisselkoers wordt opgezocht in het venster **Valutawisselkoersen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-168">The relevant exchange rate is found in the **Currency Exchange Rates** window.</span></span> <span data-ttu-id="4d113-169">In dat geval moet u vereffening van leveranciersposten in verschillende valuta's inschakelen.</span><span class="sxs-lookup"><span data-stu-id="4d113-169">In that case, you must enable application of vendor ledger entries in different currencies.</span></span> <span data-ttu-id="4d113-170">Zie voor meer informatie [Vereffening van posten in verschillende valuta's inschakelen](finance-how-enable-application-ledger-entries-different-currencies.md)</span><span class="sxs-lookup"><span data-stu-id="4d113-170">For more information, see [Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md)</span></span>

1. <span data-ttu-id="4d113-171">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Betalingsdagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4d113-171">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d113-172">Open het journaal dat u wilt gebruiken en vul de eerste lege dagboekregel in met een valutacode.</span><span class="sxs-lookup"><span data-stu-id="4d113-172">Open the journal you want, and fill in the first empty journal line using a currency code.</span></span>
3. <span data-ttu-id="4d113-173">Kies de actie **Posten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="4d113-173">Choose the **Apply Entries** action.</span></span>
4. <span data-ttu-id="4d113-174">Selecteer de regel met de post waarmee u de post in het betalingsdagboek wilt vereffenen, kies de actie **Id toekennen** en selecteer vervolgens de post waarmee u wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="4d113-174">Select the line with the entry you want to apply to the entry in the payment journal, choose the **Set Applies-to ID** action, and then select the entry you want to apply to.</span></span>
5. <span data-ttu-id="4d113-175">Klik op **OK** om terug te gaan naar het betalingsdagboek.</span><span class="sxs-lookup"><span data-stu-id="4d113-175">Choose the **OK** button to return to the payment journal.</span></span>
6. <span data-ttu-id="4d113-176">Boek het betalingsdagboek.</span><span class="sxs-lookup"><span data-stu-id="4d113-176">Post the payment journal.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="4d113-177">Wanneer u posten in verschillende valuta's onderling vereffent, worden de posten automatisch omgezet in USD.</span><span class="sxs-lookup"><span data-stu-id="4d113-177">When you apply entries in different currencies to one another, the entries are converted to USD.</span></span> <span data-ttu-id="4d113-178">Zelfs bij een vaste wisselkoers tussen de twee relevante valuta's, bijvoorbeeld USD en EUR, kan er een klein verschilbedrag ontstaan wanneer bedragen in de vreemde valuta worden omgezet naar de lokale valuta.</span><span class="sxs-lookup"><span data-stu-id="4d113-178">Even though the exchange rates for the two relevant currencies are fixed, for example between USD and EUR, there may be a small residual amount when these foreign-currency amounts are converted to USD.</span></span> <span data-ttu-id="4d113-179">Deze kleine verschilbedragen worden als winst- of verliesbedragen geboekt naar de rekening die u hebt opgegeven in de velden **Gereal. koerswinstrekening** of **Gereal. koersverliesrekening** van het venster **Valuta's**.</span><span class="sxs-lookup"><span data-stu-id="4d113-179">These small residual amounts are posted as gains and losses to the account specified in the **Realized Gains Account** or **Realized Losses Account** field in the **Currencies** window.</span></span> <span data-ttu-id="4d113-180">Het veld **Bedrag (lokale valuta)** wordt ook aangepast in de relevante leveranciersposten.</span><span class="sxs-lookup"><span data-stu-id="4d113-180">The **Amount (USD)** field is also adjusted on the relevant vendor ledger entries.</span></span>

## <a name="to-unapply-an-application-of-vendor-entries"></a><span data-ttu-id="4d113-181">De vereffening van leveranciersposten ongedaan maken</span><span class="sxs-lookup"><span data-stu-id="4d113-181">To unapply an application of vendor entries</span></span>
<span data-ttu-id="4d113-182">Als u een verkeerde vereffening ongedaan maakt, worden er stornoposten gemaakt die identiek zijn aan de oorspronkelijke post maar met een tegengesteld teken in het bedragveld, en geboekt voor alle posten, inclusief alle GB-boekingen die uit de vereffening voortkomen zoals contantkortingen en valutawinst- en verlies.</span><span class="sxs-lookup"><span data-stu-id="4d113-182">When you unapply an erroneous application, correcting entries that are identical to the original entry but with opposite sign in the amount field are created and posted for all entries, including all general ledger posting derived from the application, such as payment discount and currency gains/losses.</span></span> <span data-ttu-id="4d113-183">De posten die waren afgesloten door de toepassing worden heropend.</span><span class="sxs-lookup"><span data-stu-id="4d113-183">The entries that were closed by the application are reopened.</span></span>

1. <span data-ttu-id="4d113-184">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4d113-184">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="4d113-185">Open de desbetreffende leverancierskaart.</span><span class="sxs-lookup"><span data-stu-id="4d113-185">Open the relevant vendor card.</span></span>
3. <span data-ttu-id="4d113-186">Kies de actie **Posten**.</span><span class="sxs-lookup"><span data-stu-id="4d113-186">Choose the **Ledger Entries** action.</span></span>
4. <span data-ttu-id="4d113-187">Selecteer de betreffende post en kies de actie **Vereffening posten ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="4d113-187">Select the relevant ledger entry, and then choose the **Unapply Entries** action.</span></span>
5. <span data-ttu-id="4d113-188">Of kies de actie **Gedetailleerde post**.</span><span class="sxs-lookup"><span data-stu-id="4d113-188">Alternatively, choose the **Detailed Ledger Entry** action.</span></span>
6. <span data-ttu-id="4d113-189">Selecteer de vereffeningspost en kies de actie **Vereffening posten ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="4d113-189">Select the application entry, and then choose the **Unapply Entries** action.</span></span>
7. <span data-ttu-id="4d113-190">Vul de velden in de kop in en klik vervolgens op de knop **Vereffening ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="4d113-190">Fill in the fields in the header, and then choose the **Unapply** action.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="4d113-191">Als een post is vereffend door meer dan één vereffeningspost, moet u de vereffening van de laatste vereffeningspost het eerst ongedaan maken.</span><span class="sxs-lookup"><span data-stu-id="4d113-191">If an entry has been applied by more than one application entry, you must unapply the latest application entry first.</span></span>

## <a name="see-also"></a><span data-ttu-id="4d113-192">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4d113-192">See Also</span></span>
[<span data-ttu-id="4d113-193">Schulden</span><span class="sxs-lookup"><span data-stu-id="4d113-193">Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="4d113-194">Inkoop</span><span class="sxs-lookup"><span data-stu-id="4d113-194">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="4d113-195">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4d113-195">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
