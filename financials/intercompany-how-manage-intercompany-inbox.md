---
title: Inkomende en uitgaande IC-transacties verwerken | Microsoft Docs
description: Intercompany-transacties (IC-transacties) die u ontvangt van uw IC-partners worden weergegeven in de IC-inbox, waar u ze handmatig of automatisch verwerkt.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: incoming document
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5cf49fa7b1c2d4385cd05f44e10237078e1214a4
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-manage-the-intercompany-inbox-and-outbox"></a><span data-ttu-id="4ea1d-103">Procedure: De intercompany-inbox en outbox beheren</span><span class="sxs-lookup"><span data-stu-id="4ea1d-103">How to: Manage the Intercompany Inbox and Outbox</span></span>
<span data-ttu-id="4ea1d-104">Alle IC-transacties die u via elektronische weg ontvangt van uw IC-partners, worden weergegeven in de IC-inbox.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-104">All of the intercompany transactions that you receive electronically from your intercompany partners are listed in the intercompany Inbox.</span></span>  

## <a name="organizing-the-inbox"></a><span data-ttu-id="4ea1d-105">De IC-inbox ordenen</span><span class="sxs-lookup"><span data-stu-id="4ea1d-105">Organizing the Inbox</span></span>  
 <span data-ttu-id="4ea1d-106">Met de filtervelden boven aan het inboxvenster kunt u bepalen welke transacties worden weergegeven in het venster.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-106">You can use the filter fields at the top of the inbox window to determine which transactions are shown in the window.</span></span> <span data-ttu-id="4ea1d-107">Als u bijvoorbeeld alleen transacties wilt weergeven die door een bepaalde partner zijn gemaakt, kunt u filtercriteria invoeren in de filters **Transactiebron** en IC-**partnercode**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-107">For example, if you only want to look at transactions a particular partner created, you can enter filters in the **Transaction Source** and **Intercompany Partner Code** filters.</span></span>  

### <a name="transaction-source"></a><span data-ttu-id="4ea1d-108">Transactiebron</span><span class="sxs-lookup"><span data-stu-id="4ea1d-108">Transaction Source</span></span>  
<span data-ttu-id="4ea1d-109">Wat u met een transactie kunt doen, hangt af van het volgende:</span><span class="sxs-lookup"><span data-stu-id="4ea1d-109">What you can do with a transaction depends whether it was:</span></span>  

- <span data-ttu-id="4ea1d-110">Transactie gemaakt door uw IC-partner</span><span class="sxs-lookup"><span data-stu-id="4ea1d-110">Created by your intercompany partner</span></span>  
- <span data-ttu-id="4ea1d-111">Transactie geweigerd door uw IC-partner en aan u geretourneerd</span><span class="sxs-lookup"><span data-stu-id="4ea1d-111">Rejected by your intercompany partner and returned to you</span></span>  

<span data-ttu-id="4ea1d-112">Met het veld **Transactiebron weergeven** kunt u het venster **IC-inboxtransacties** filteren, zodat maar een van deze soorten transacties wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-112">You can use the **Show Transaction Source** field to filter the **Intercompany Inbox Transactions** window so that it displays only one of these types of transactions.</span></span> <span data-ttu-id="4ea1d-113">U kunt ook filteren op IC-partner of op de inhoud van het veld **Regelactie**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-113">(You can also filter by intercompany partner, or by the contents of the **Line Action** field.)</span></span>  

#### <a name="created-by-intercompany-partner"></a><span data-ttu-id="4ea1d-114">Transactie gemaakt door IC-partner</span><span class="sxs-lookup"><span data-stu-id="4ea1d-114">Created by Intercompany Partner</span></span>  
 <span data-ttu-id="4ea1d-115">Wanneer u een nieuwe transactie ontvangt die door uw partner is gemaakt, kunt u ervoor kiezen:</span><span class="sxs-lookup"><span data-stu-id="4ea1d-115">When you receive a new transaction that was created by your partner, you can choose to either:</span></span>

- <span data-ttu-id="4ea1d-116">De transactie te accepteren</span><span class="sxs-lookup"><span data-stu-id="4ea1d-116">Accept the transaction</span></span>  
- <span data-ttu-id="4ea1d-117">De transactie te weigeren (en aan de partner te retourneren)</span><span class="sxs-lookup"><span data-stu-id="4ea1d-117">Reject the transaction (Return to partner)</span></span>  
- <span data-ttu-id="4ea1d-118">De transactie te annuleren (de transactie verwijderen en niet retourneren aan uw partner)</span><span class="sxs-lookup"><span data-stu-id="4ea1d-118">Cancel the transaction (Delete the transaction but do not return it to your partner)</span></span>  

#### <a name="returned-from-intercompany-partner"></a><span data-ttu-id="4ea1d-119">Geretourneerd door IC-partner</span><span class="sxs-lookup"><span data-stu-id="4ea1d-119">Returned from Intercompany Partner</span></span>  
 <span data-ttu-id="4ea1d-120">Als de transactie is geweigerd door uw IC-partner, hebt u geen andere keuze dan de transactie in de inbox te annuleren.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-120">If the transaction was rejected by your intercompany partner, your only choice is to cancel the transaction in the inbox.</span></span> <span data-ttu-id="4ea1d-121">Vervolgens moet u correctieregels maken of het dagboek of document in uw bedrijf tegenboeken.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-121">Then you must create correction lines or reverse the journal or document in your company.</span></span>  

## <a name="re-creating-inbox-entries"></a><span data-ttu-id="4ea1d-122">Inboxitems opnieuw maken</span><span class="sxs-lookup"><span data-stu-id="4ea1d-122">Re-creating Inbox Entries</span></span>  
 <span data-ttu-id="4ea1d-123">Als u een transactie in uw inbox hebt geaccepteerd maar het document of dagboek vervolgens hebt verwijderd in plaats van geboekt, kunt u het inboxitem opnieuw maken en het nogmaals accepteren.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-123">If you accepted a transaction in your inbox but then deleted the document or journal instead of posting it, you can re-create the inbox entry and accept it again.</span></span>  

## <a name="getting-an-overview-of-intercompany-transactions-for-a-period"></a><span data-ttu-id="4ea1d-124">Een overzicht weergeven van IC-transacties voor een bepaalde periode</span><span class="sxs-lookup"><span data-stu-id="4ea1d-124">Getting an Overview of Intercompany Transactions for a Period</span></span>  
 <span data-ttu-id="4ea1d-125">U kunt een overzicht weergeven van alle IC-transacties die u in een bepaalde periode hebt verzonden en ontvangen.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-125">You can get an overview of all of the intercompany transactions that you have sent and received in a period.</span></span> <span data-ttu-id="4ea1d-126">In de lijst **IC-transacties** worden alle IC-grootboekposten, klantenposten en leveranciersposten weergegeven.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-126">The **Intercompany Transactions** report lists all intercompany G/L entries, customer ledger entries, and vendor ledger entries.</span></span>

 > [!NOTE]  
 > <span data-ttu-id="4ea1d-127">Als de IC-partners in dezelfde database zijn opgenomen, worden de transacties verzonden zonder dat een bestand of e-mail nodig is.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-127">If the intercompany partners are in the same database, then transactions are transferred without the need for file or email.</span></span> <span data-ttu-id="4ea1d-128">Zie het veld **Overdrachttype** in het venster **IC-partner**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-128">See the **Transfer Type** field in the **Intercompany Partner** window.</span></span> <br /><br />
<span data-ttu-id="4ea1d-129">In dat geval, kunt u in het systeem instellen om de inbox en de outbox over te slaan, door respectievelijk het selectievakje **Transacties automatisch accepteren** in het venster **IC-partner** en het selectievakje **Transacties automatisch verzenden** in het venster **IC-instellingen** in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-129">In that case, you can set the system up to bypass the inbox and outbox by selecting the **Auto. Accept Transactions** check box in the **Intercompany Partner** window and the **Auto. Send Transactions** check box in the **Intercompany Setup** window respectively.</span></span>

## <a name="to-import-intercompany-transactions-from-a-file"></a><span data-ttu-id="4ea1d-130">IC-transacties importeren uit een bestand</span><span class="sxs-lookup"><span data-stu-id="4ea1d-130">To import intercompany transactions from a file</span></span>  
<span data-ttu-id="4ea1d-131">Als u een IC-partner hebt die zich niet in dezelfde database bevindt als uw bedrijf, kunt u IC-transacties van die partner ophalen in een XML-bestand.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-131">If you have an intercompany partner that is not in the same database as your company, you can receive intercompany transactions from that partner in an .xml file.</span></span> <span data-ttu-id="4ea1d-132">Vervolgens moet u de transacties importeren in uw inbox.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-132">Then you must import the transactions into your inbox.</span></span>  

1.  <span data-ttu-id="4ea1d-133">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bedrijfsgegevens** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-133">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Company Information** , and then choose the related link.</span></span>
2. <span data-ttu-id="4ea1d-134">Sla het bestand op naar de locatie die u hebt opgegeven in het veld **Details IC-inbox** in het venster **Bedrijfsgegevens**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-134">Save the file to the location that you specified in the **Intercompany Inbox Details** field in the **Company Information** window.</span></span>  
3. <span data-ttu-id="4ea1d-135">Klik op het pictogram ![Zoeken naar pagina of rapport]pictogram (media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **IC-inboxtransacties** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Intercompany Inbox Transactions**, and then choose the related link.</span></span>
4. <span data-ttu-id="4ea1d-136">Kies in het venster **IC-inboxtransacties** de actie **Transactiebestand importeren**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-136">In the **Intercompany Inbox Transactions** window, choose the **Import Transaction File** action.</span></span>  
5. <span data-ttu-id="4ea1d-137">Selecteer in het venster dat wordt geopend het .xml-bestand dat de transacties bevat en klik vervolgens op **Openen**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-137">In the window that appears, select the .xml file that contains the transactions, and then choose the **Open** button.</span></span>  

<span data-ttu-id="4ea1d-138">De transacties worden geïmporteerd in de inbox en u kunt ze nu verwerken.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-138">The transactions are imported into the inbox and you can now process them.</span></span>

## <a name="to-process-incoming-intercompany-transactions"></a><span data-ttu-id="4ea1d-139">Inkomende IC-transacties verwerken</span><span class="sxs-lookup"><span data-stu-id="4ea1d-139">To process incoming intercompany transactions</span></span>  
<span data-ttu-id="4ea1d-140">Wanneer uw IC-partners u IC-transacties toesturen, komen de transacties terecht in uw IC-inbox.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-140">When your intercompany partners send you intercompany transactions, the transactions end up in your intercompany inbox.</span></span> <span data-ttu-id="4ea1d-141">U moet elke transactie in uw inbox evalueren en verwerken.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-141">You must evaluate each transaction in your inbox and act upon it.</span></span>  

1. <span data-ttu-id="4ea1d-142">Klik op het pictogram ![Zoeken naar pagina of rapport]pictogram (media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **IC-inboxtransacties** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-142">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Intercompany Inbox Transactions**, and then choose the related link.</span></span>  
2. <span data-ttu-id="4ea1d-143">Selecteer in het venster **IC-inboxtransacties** een regel en kies een actie om de regel te verwerken, zoals bijvoorbeeld **Goedkeuren**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-143">In the **Intercompany Inbox Transactions** window, select a line, and then choose an action, such as **Accept**, to process the line.</span></span>
3. <span data-ttu-id="4ea1d-144">Vul in het venster **Bewerking IC-inbox voltooien** de velden in met de benodigde gegevens.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-144">In the **Complete IC Inbox Action** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="4ea1d-145">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-145">Choose the **OK** button.</span></span>  

<span data-ttu-id="4ea1d-146">Bij regels die u verwerkt met de actie **Goedkeuren**, worden document- of dagboekregels aangemaakt in uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-146">For lines that you processed with the **Accept** action, document or journal lines will be created in your company.</span></span> <span data-ttu-id="4ea1d-147">Open elk document of dagboek, breng de gewenste wijzigingen aan en boek de regels.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-147">Open each document or journal, make any necessary changes, and then post them.</span></span>  

<span data-ttu-id="4ea1d-148">De regels die u verwerkt met de actie **Retour naar partner** worden verplaatst naar de IC-outbox, vanwaar u ze naar uw partner kunt verzenden.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-148">Lines that you processed with the **Return to Partner** action will be moved to the outbox from where you can then send them to your partner.</span></span>

<span data-ttu-id="4ea1d-149">Voor regels die u verwerkt met de actie **Retour door partner** moet u nu een correctie boeken op de oorspronkelijke transactie die u boekte in uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-149">For lines that you processed with the **Returned by Partner** action, you must now post a correction to the original transaction that you posted in your company.</span></span>

## <a name="to-process-outgoing-intercompany-transactions"></a><span data-ttu-id="4ea1d-150">Uitgaande IC-transacties verwerken</span><span class="sxs-lookup"><span data-stu-id="4ea1d-150">To process outgoing intercompany transactions</span></span>  
<span data-ttu-id="4ea1d-151">Wanneer u een IC-dagboek of -document boekt of een IC-orderbevestiging verzendt, worden de transacties verzonden naar uw IC-outbox.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-151">When you post an intercompany journal or document, or send an intercompany order confirmation, the transactions are sent to your intercompany outbox.</span></span> <span data-ttu-id="4ea1d-152">Als u deze wilt doorsturen naar uw IC-partners, moet u de outbox openen en de transacties verwerken.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-152">In order for them to be sent on to your intercompany partners, you must open the outbox and process them.</span></span>  

1.  <span data-ttu-id="4ea1d-153">Klik op het pictogram ![Zoeken naar pagina of rapport]pictogram(media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **IC-outboxtransacties** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-153">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Intercompany Outbox Transactions**, and then choose the related link.</span></span>  
2. <span data-ttu-id="4ea1d-154">Selecteer in het venster **IC-outboxtransacties** een regel en kies een actie om de regel te verwerken, zoals bijvoorbeeld **Terug naar inbox**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-154">In the **Intercompany Outbox Transactions** window, select a line, and then choose an action, such as **Return to Inbox**, to process the line.</span></span>

<span data-ttu-id="4ea1d-155">Regels die u verwerkt met de actie **Verzenden naar IC-partner** worden verzonden naar de inbox van de betreffende partner.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-155">Lines that you processed with the **Send to Intercompany Partner** action will be sent to the relevant partner's inbox.</span></span>

<span data-ttu-id="4ea1d-156">De regels die u verwerkt met de actie **Terug naar inbox** worden naar de inbox verplaatst, waar u ze kunt goedkeuren om documenten of dagboekregels in uw bedrijf te maken.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-156">Lines that you processed with the **Return to Inbox** action will be moved to the inbox where you can then accept them to create documents or journal lines in your company.</span></span>  

<span data-ttu-id="4ea1d-157">Voor regels die u verwerkt met de actie **Annuleren** moet u nu een correctie boeken op de oorspronkelijke transactie die u boekte in uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-157">For lines that you processed with the **Cancel** action, you must now post a correction to the original transaction that you posted in your company.</span></span>  

## <a name="to-recreate-intercompany-inbox-transactions"></a><span data-ttu-id="4ea1d-158">IC-inboxtransacties opnieuw maken</span><span class="sxs-lookup"><span data-stu-id="4ea1d-158">To recreate intercompany inbox transactions</span></span>  
<span data-ttu-id="4ea1d-159">Het kan voorkomen dat u een transactie in de inbox of outbox opnieuw wilt maken.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-159">Occasionally, you may want to re-create a transaction in the inbox or outbox.</span></span> <span data-ttu-id="4ea1d-160">Als u een transactie in uw inbox bijvoorbeeld hebt geaccepteerd maar het document of dagboek vervolgens hebt verwijderd in plaats van geboekt, kunt u de inboxpost opnieuw maken en deze nogmaals accepteren.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-160">For example, if you accepted a transaction in your inbox but then deleted the document or journal instead of posting it, you can re-create the inbox entry and accept it again.</span></span>  

<span data-ttu-id="4ea1d-161">In de volgende procedure wordt beschreven hoe u inboxtransacties opnieuw kunt maken. De procedure voor de outbox is hetzelfde.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-161">The following procedure describes to re-create inbox transactions, but the same steps also apply to the outbox.</span></span>

  1.  <span data-ttu-id="4ea1d-162">Klik op het pictogram ![Zoeken naar pagina of rapport]pictogram(media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **Verwerkte IC-inboxtransacties** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-162">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Handled IC Inbox Transactions**, and then choose the related link.</span></span>  

  2.  <span data-ttu-id="4ea1d-163">Open het venster **Verwerkte IC-inboxtransacties**, selecteer de regel met de transactie die u opnieuw wilt maken in de inbox en selecteer de actie **Inboxtransacties opnieuw maken**.</span><span class="sxs-lookup"><span data-stu-id="4ea1d-163">In the **Handled IC Inbox Transactions** window, select the line with the transaction that you want to re-create in the inbox, and then choose the **Re-create Inbox Transaction** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="4ea1d-164">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4ea1d-164">See Also</span></span>
[<span data-ttu-id="4ea1d-165">Intercompany-transacties beheren</span><span class="sxs-lookup"><span data-stu-id="4ea1d-165">Managing Intercompany Transactions</span></span>](intercompany-manage.md)  
[<span data-ttu-id="4ea1d-166">Financiën</span><span class="sxs-lookup"><span data-stu-id="4ea1d-166">Finance</span></span>](finance.md)  
[<span data-ttu-id="4ea1d-167">Financiën instellen</span><span class="sxs-lookup"><span data-stu-id="4ea1d-167">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="4ea1d-168">Werken met diversendagboeken</span><span class="sxs-lookup"><span data-stu-id="4ea1d-168">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="4ea1d-169">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4ea1d-169">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
