---
title: SEPA-verzameling van automatische incasso | Microsoft Docs
description: Maak een incasso-opdracht en exporteer een XML-bestand dat u naar uw elektronische bank verzendt of uploadt voor verwerking.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct-debit, collection, payment, sepa
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: dbecf91050dbdf299ca11e8e5650b2a63b4ccc16
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-create-sepa-direct-debit-collection-entries-and-export-to-a-bank-file"></a><span data-ttu-id="edec2-103">Procedure: SEPA-verzamelingsposten van automatische incasso maken en exporteren naar een bankbestand</span><span class="sxs-lookup"><span data-stu-id="edec2-103">How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File</span></span>
<span data-ttu-id="edec2-104">Om de bank het bedrag van de bankrekening van de klant over te laten maken naar de rekening van uw bedrijf, moet u een incasso-opdracht maken met informatie over de bankrekening van de klant, de betreffende verkoopfacturen en de incassomachtiging.</span><span class="sxs-lookup"><span data-stu-id="edec2-104">To instruct the bank to transfer the payment amount from the customer’s bank account to your company’s account, you create a direct-debit collection, which holds information about the customer’s bank account, the affected sales invoices, and the direct-debit mandate.</span></span> <span data-ttu-id="edec2-105">Uit de resulterende verzamelingspost van automatische incasso export u vervolgens een XML-bestand dat u naar uw elektronische bank verzendt of uploadt voor verwerking.</span><span class="sxs-lookup"><span data-stu-id="edec2-105">From the resulting direct-debit collection entry, you then export an XML file that you send or upload to your electronic bank for processing.</span></span> <span data-ttu-id="edec2-106">Betalingen die niet konden worden verwerkt door de bank worden aan u gemeld door uw bank. U moet vervolgens handmatig de desbetreffende verzamelingsposten van automatische incasso weigeren.</span><span class="sxs-lookup"><span data-stu-id="edec2-106">Any payments that could not be processed by the bank will be communicated to you by your bank, and you must then manually reject the direct debit-collection entries in question.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="edec2-107">Om betalingen te innen via SEPA Incasso, moet de valuta in de verkoopfactuur EURO zijn.</span><span class="sxs-lookup"><span data-stu-id="edec2-107">To collect payments using SEPA Direct Debit, the currency on the sales invoice must be EURO.</span></span>  

### <a name="to-create-a-direct-debit-collection"></a><span data-ttu-id="edec2-108">Een incasso-opdracht maken</span><span class="sxs-lookup"><span data-stu-id="edec2-108">To create a direct-debit collection</span></span>  
1. <span data-ttu-id="edec2-109">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Incasso-opdrachten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="edec2-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="edec2-110">Kies in het venster **Incasso-opdrachten** op het tabblad **Start** in de groep **Nieuw** de optie **Incasso-opdracht maken**.</span><span class="sxs-lookup"><span data-stu-id="edec2-110">In the **Direct Debit Collections** window, on the **Home** tab, in the **New** group, choose **Create Direct Debit Collection**.</span></span>  
3. <span data-ttu-id="edec2-111">Vul in het venster **Incasso-opdracht maken** de velden in zoals wordt beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="edec2-111">In the **Create Direct Debit Collection** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="edec2-112">Veld</span><span class="sxs-lookup"><span data-stu-id="edec2-112">Field</span></span>|<span data-ttu-id="edec2-113">Description</span><span class="sxs-lookup"><span data-stu-id="edec2-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="edec2-114">**Vanaf vervaldatum**</span><span class="sxs-lookup"><span data-stu-id="edec2-114">**From Due Date**</span></span>|<span data-ttu-id="edec2-115">Geef de eerste betalingsvervaldatum aan op de verkoopfacturen die u wilt maken voor een incasso-opdracht.</span><span class="sxs-lookup"><span data-stu-id="edec2-115">Specify the earliest payment due date on sales invoices that you want to create a direct-debit collection for.</span></span>|  
    |<span data-ttu-id="edec2-116">**Tot vervaldatum**</span><span class="sxs-lookup"><span data-stu-id="edec2-116">**To Due Date**</span></span>|<span data-ttu-id="edec2-117">Geef de laatste betalingsvervaldatum aan op de verkoopfacturen die u wilt maken voor een automatische incasso-verzameling.</span><span class="sxs-lookup"><span data-stu-id="edec2-117">Specify the latest payment due date on sales invoices that you want to create a direct-debit collection for.</span></span>|  
    |<span data-ttu-id="edec2-118">**Partnersoort**</span><span class="sxs-lookup"><span data-stu-id="edec2-118">**Partner Type**</span></span>|<span data-ttu-id="edec2-119">Geef aan of de verzameling automatische incasso is gemaakt voor klanten van het type **Bedrijf** of **Persoon**.</span><span class="sxs-lookup"><span data-stu-id="edec2-119">Specify if the direct-debit collection is made for customers of type **Company** or **Person**.</span></span>|  
    |<span data-ttu-id="edec2-120">**Alleen klanten met geldige machtiging**</span><span class="sxs-lookup"><span data-stu-id="edec2-120">**Only Customers With Valid Mandate**</span></span>|<span data-ttu-id="edec2-121">Geef aan of een incasso-opdracht wordt gemaakt voor klanten die beschikken over een geldige incassomachtiging.</span><span class="sxs-lookup"><span data-stu-id="edec2-121">Specify if a direct-debit collection is created for customers who have a valid direct-debit mandate.</span></span> <span data-ttu-id="edec2-122">**Opmerking:** er wordt ook een automatische incasso-opdracht gemaakt als het veld **Machtigingsnummer voor incasso** niet is ingevuld op de verkoopfactuur.</span><span class="sxs-lookup"><span data-stu-id="edec2-122">**Note:**  A direct-debit collection is created even if the **Direct Debit Mandate ID** field is not filled on the sales invoice.</span></span>|  
    |<span data-ttu-id="edec2-123">**Alleen facturen met geldige machtiging**</span><span class="sxs-lookup"><span data-stu-id="edec2-123">**Only Invoices With Valid Mandate**</span></span>|<span data-ttu-id="edec2-124">Geef op of de incasso-opdracht alleen wordt gemaakt voor verkoopfacturen als een geldige incassomachtiging is geselecteerd in het veld **Machtigingsnummer voor incasso** op de verkoopfactuur.</span><span class="sxs-lookup"><span data-stu-id="edec2-124">Specify if a direct-debit collection is only created for sales invoices if a valid direct-debit mandate is selected in the **Direct Debit Mandate ID** field on the sales invoice.</span></span>|  
    |<span data-ttu-id="edec2-125">**Bankrekeningnr.**</span><span class="sxs-lookup"><span data-stu-id="edec2-125">**Bank Account No.**</span></span>|<span data-ttu-id="edec2-126">Geef op naar welke bankrekeningen van uw bedrijf de verzamelde betaling wordt overgeboekt van de bankrekening van de klant.</span><span class="sxs-lookup"><span data-stu-id="edec2-126">Specify which of your company’s bank accounts the collected payment will be transferred to from the customer’s bank account.</span></span>|  
    |<span data-ttu-id="edec2-127">**Bankrekeningnaam**</span><span class="sxs-lookup"><span data-stu-id="edec2-127">**Bank Account Name**</span></span>|<span data-ttu-id="edec2-128">Geeft de naam van de bankrekening weer die u selecteert in het veld **Bankrekeningnr.**.</span><span class="sxs-lookup"><span data-stu-id="edec2-128">Specifies the name of the bank account that you select in the **Bank Account No.** field.</span></span> <span data-ttu-id="edec2-129">Dit veld wordt automatisch ingevuld.</span><span class="sxs-lookup"><span data-stu-id="edec2-129">This field is filled automatically.</span></span>|  

4. <span data-ttu-id="edec2-130">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="edec2-130">Choose the **OK** button.</span></span>  

     <span data-ttu-id="edec2-131">Er wordt een automatische incasso-opdracht toegevoegd aan het venster **Incasso-opdrachten** en er worden een of meer automatische incasso-opdrachtposten gemaakt.</span><span class="sxs-lookup"><span data-stu-id="edec2-131">A direct-debit collection is added to the **Direct Debit Collections** window, and one or more direct-debit collection entries are created.</span></span>  

### <a name="to-export-a-direct-debit-collection-entry-to-a-bank-file"></a><span data-ttu-id="edec2-132">Verzamelingposten van automatische incasso exporteren naar een bankbestand</span><span class="sxs-lookup"><span data-stu-id="edec2-132">To export a direct-debit collection entry to a bank file</span></span>  
1. <span data-ttu-id="edec2-133">Kies in het venster **Incasso-opdrachten** op het tabblad **Start** in de groep **Verwerken** de optie **Verzamelingsposten van incasso**.</span><span class="sxs-lookup"><span data-stu-id="edec2-133">In the **Direct Debit Collections** window, on the **Home** tab, in the **Process** group, choose **Direct Debit Collect. Entries**.</span></span>  
2. <span data-ttu-id="edec2-134">Selecteer in het venster **Verzamelingsposten van incasso** de post die u wilt exporteren en kies vervolgens op het tabblad **Start** in de groep **Verwerken** de optie **Bestand van automatische incasso aanmaken**.</span><span class="sxs-lookup"><span data-stu-id="edec2-134">In the **Direct Debit Collect. Entries** window, select the entry that you want to export, and then, on the **Home** tab, in the **Process** group, choose **Create Direct Debit** File.</span></span>  
3. <span data-ttu-id="edec2-135">Het exportbestand opslaan naar de locatie van waar u verzendt of uploadt naar uw elektronische bank.</span><span class="sxs-lookup"><span data-stu-id="edec2-135">Save the export file to the location from where you send or upload it to your electronic bank.</span></span>  

     <span data-ttu-id="edec2-136">In het venster **Verzamelingsposten van incasso** verandert het veld **Incasso-opdrachtstatus** in Bestand gemaakt.</span><span class="sxs-lookup"><span data-stu-id="edec2-136">In the **Direct Debit Collect. Entries** window, the **Direct Debit Collection Status** field is changed to File Created.</span></span> <span data-ttu-id="edec2-137">In het venster **SEPA Incasso Machtiging** wordt het veld **Debetteller** bijgewerkt met één telling.</span><span class="sxs-lookup"><span data-stu-id="edec2-137">In the **SEPA Direct Debit Mandates** window, the **Debit Counter** field is updated with one count.</span></span>  

<span data-ttu-id="edec2-138">Als het geëxporteerde bestand niet kan worden verwerkt, bijvoorbeeld omdat de klant insolvent is, kunt u de incasso-opdrachtpost weigeren.</span><span class="sxs-lookup"><span data-stu-id="edec2-138">If the exported file cannot be processed, for example because the customer is insolvent, you can reject the direct-debit collection entry.</span></span> <span data-ttu-id="edec2-139">Als het geëxporteerde bestand met succes is verwerkt door de bank, worden de verschuldigde betalingen van de betrokken verkoopfacturen automatisch geïnd bij de betrokken klanten.</span><span class="sxs-lookup"><span data-stu-id="edec2-139">If the exported file is successfully processed by the bank, the due payments of the involved sales invoices are automatically collected from the involved customers.</span></span> <span data-ttu-id="edec2-140">In dat geval kunt u de incasso sluiten.</span><span class="sxs-lookup"><span data-stu-id="edec2-140">In that case you can close the collection.</span></span>  

### <a name="to-reject-a-direct-debit-collection-entry"></a><span data-ttu-id="edec2-141">Een incasso-opdrachtpost weigeren</span><span class="sxs-lookup"><span data-stu-id="edec2-141">To reject a direct-debit collection entry</span></span>  
* <span data-ttu-id="edec2-142">Selecteer in het venster **Verzamelingsposten van incasso** de post die niet goed is verwerkt en kies vervolgens op het tabblad **Start** in de groep **Verwerken** de optie **Post weigeren**.</span><span class="sxs-lookup"><span data-stu-id="edec2-142">In the **Direct Debit Collect. Entries** window, select the entry that was not successfully processed, and then, on the **Home** tab, in the **Process** group, choose **Reject Entry**.</span></span>  

     <span data-ttu-id="edec2-143">De waarde in het veld **Status** in het venster **Verzamelingsposten van incasso** verandert in **Geweigerd**.</span><span class="sxs-lookup"><span data-stu-id="edec2-143">The value in the **Status** field in the **Direct Debit Collect. Entries** window is changed to **Rejected**.</span></span>  

### <a name="to-close-a-direct-debit-collection"></a><span data-ttu-id="edec2-144">Een incasso-opdracht sluiten</span><span class="sxs-lookup"><span data-stu-id="edec2-144">To close a direct-debit collection</span></span>  
* <span data-ttu-id="edec2-145">Selecteer in het venster **Verzamelingsposten van incasso** de post die niet goed is verwerkt en kies vervolgens op het tabblad **Start** in de groep **Verwerken** de optie **Verzameling sluiten**.</span><span class="sxs-lookup"><span data-stu-id="edec2-145">In the **Direct Debit Collect. Entries** window, select the entry that was successfully processed, and then, on the **Home** tab, in the **Process** group, choose **Close Collection**.</span></span>  

     <span data-ttu-id="edec2-146">De bijbehorende verzameling automatische incasso is gesloten.</span><span class="sxs-lookup"><span data-stu-id="edec2-146">The related direct-debit collection is closed.</span></span>  

<span data-ttu-id="edec2-147">U kunt nu ontvangen betalingen voor de betrokken verkoopfacturen boeken.</span><span class="sxs-lookup"><span data-stu-id="edec2-147">You can now post receipts of payment for the involved sales invoices.</span></span> <span data-ttu-id="edec2-148">U kunt dit doen terwijl u, als gewoonlijk, betalingsontvangsten boekt, bijvoorbeeld in het venster **Betalingsregistratie**, of u kunt de gerelateerde betalingsontvangsten rechtstreeks boeken vanuit het venster **Verzamelingsposten van incasso**.</span><span class="sxs-lookup"><span data-stu-id="edec2-148">You can do this as you typically post payment receipts, such as in the **Payment Registration** window, or you can post the related payment receipts directly from the **Direct Debit Collect. Entries** window.</span></span> <span data-ttu-id="edec2-149">Zie voor meer informatie [Procedure: SEPA-betalingsontvangsten via automatische incasso boeken](finance-how-to-post-sepa-direct-debit-payment-receipts.md).</span><span class="sxs-lookup"><span data-stu-id="edec2-149">For more information, see [How to: Post SEPA Direct Debit Payment Receipts](finance-how-to-post-sepa-direct-debit-payment-receipts.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="edec2-150">Zie ook</span><span class="sxs-lookup"><span data-stu-id="edec2-150">See Also</span></span>  
<span data-ttu-id="edec2-151">[Procedure: Automatische incasso via SEPA instellen](finance-how-to-set-up-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="edec2-151">[How to: Set Up SEPA Direct Debit](finance-how-to-set-up-sepa-direct-debit.md) </span></span>  
<span data-ttu-id="edec2-152">[Procedure: SEPA-betalingsontvangsten via automatische incasso boeken](finance-how-to-post-sepa-direct-debit-payment-receipts.md) </span><span class="sxs-lookup"><span data-stu-id="edec2-152">[How to: Post SEPA Direct Debit Payment Receipts](finance-how-to-post-sepa-direct-debit-payment-receipts.md) </span></span>  
[<span data-ttu-id="edec2-153">Betalingen verzamelen via automatische incasso van SEPA</span><span class="sxs-lookup"><span data-stu-id="edec2-153">Collect Payments with SEPA Direct Debit</span></span>](finance-collect-payments-with-sepa-direct-debit.md)   
