---
title: Een verkoopaanbod voor een klant maken | Microsoft Docs
description: Beschrijft hoe u een verkoopaanbieding of een offerteaanvraagdocument maakt om uw aanbod aan een klant vast te leggen om producten onder bepaalde voorwaarden te verkopen.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 08/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 60ee3c2226e45bb904d91243c861a2d747447abc
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="make-offers"></a><span data-ttu-id="d8ac1-103">Aanbiedingen doen</span><span class="sxs-lookup"><span data-stu-id="d8ac1-103">Make Offers</span></span>
<span data-ttu-id="d8ac1-104">U maakt een verkoopofferte aan om uw aanbod aan een klant vast te leggen om producten tegen bepaalde leverings- en betalingscondities te verkopen.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-104">You create a sales quote to record your offer to a customer to sell certain products on certain delivery and payment terms.</span></span> <span data-ttu-id="d8ac1-105">U kunt de verkoopofferte aan de klant verzenden om het aanbod te bevestigen.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-105">You can send the sales quote to the customer to communicate the offer.</span></span> <span data-ttu-id="d8ac1-106">U kunt het document als een PDF-bijlage via e-mail versturen.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-106">You can email the document as a PDF attachment.</span></span> <span data-ttu-id="d8ac1-107">U kunt ook de hoofdtekst van de e-mail vooraf laten invullen met een overzicht van de offerte.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-107">You can also have the email body prefilled with a summary of the quote.</span></span> <span data-ttu-id="d8ac1-108">Zie [Documenten per e-mail verzenden](ui-how-send-documents-email.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-108">For more information, see [Send Documents by Email](ui-how-send-documents-email.md).</span></span>

<span data-ttu-id="d8ac1-109">Terwijl u met de klant onderhandelt, kunt u zo veel als u wenst de verkoopofferte wijzigen en opnieuw zenden.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-109">While you negotiate with the customer, you can change and resend the sales quote as much as needed.</span></span> <span data-ttu-id="d8ac1-110">Als de klant de offerte accepteert, zet u de verkoopofferte om in een verkoopfactuur of een verkooporder waarin u de verkoop verwerkt.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-110">When the customer accepts the quote, you convert the sales quote to a sales invoice or a sales order in which you process the sale.</span></span> <span data-ttu-id="d8ac1-111">Zie [Verkopen factureren](sales-how-invoice-sales.md) of [Producten verkopen](sales-how-sell-products.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-111">For more information, see [Invoice Sales](sales-how-invoice-sales.md) or [Sell Products](sales-how-sell-products.md).</span></span>

<span data-ttu-id="d8ac1-112">U kunt klantvelden op de verkoopofferte op twee manieren invullen afhankelijk van de vraag of de klant reeds is geregistreerd.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-112">You can fill customer fields on the sales quote in two ways depending on whether the customer is already registered.</span></span> <span data-ttu-id="d8ac1-113">Zie de stappen 2 en 3 in de volgende procedure.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-113">See steps 2 and 3 in the following procedure.</span></span>

## <a name="to-create-a-sales-quote"></a><span data-ttu-id="d8ac1-114">Een verkoopofferte maken</span><span class="sxs-lookup"><span data-stu-id="d8ac1-114">To create a sales quote</span></span>
1. <span data-ttu-id="d8ac1-115">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkoopoffertes** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Quotes**, and then choose the related link.</span></span>
2. <span data-ttu-id="d8ac1-116">Voer in het veld **Klant** de naam in van een bestaande klant.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-116">In the **Customer** field, enter the name of an existing customer.</span></span>

   <span data-ttu-id="d8ac1-117">Overige velden in het venster **Verkoopofferte** bevatten standaardinformatie over de geselecteerde klant.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-117">Other fields in the **Sales Quote** window contain standard information of the selected customer.</span></span> <span data-ttu-id="d8ac1-118">Als de klant niet is geregistreerd, volgt u deze stappen:</span><span class="sxs-lookup"><span data-stu-id="d8ac1-118">If the customer is not registered, follow these steps:</span></span>
3. <span data-ttu-id="d8ac1-119">Voer in het veld **Klant** de naam van de nieuwe klant in.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-119">In the **Customer** field, enter the name of the new customer.</span></span>
4. <span data-ttu-id="d8ac1-120">Kies in dialoogvenster voor het registreren van de nieuwe klant de knop **Ja**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-120">In the dialog box about registering the new customer, choose the **Yes** button.</span></span>
5. <span data-ttu-id="d8ac1-121">Kies in het venster **Selecteer een sjabloon voor een nieuwe klant** een sjabloon waarop u de nieuwe klantenkaart wilt baseren en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-121">In the **Select a template for a new customer** window, choose a template to base the new customer card on, and then choose the **OK** button.</span></span>
6. <span data-ttu-id="d8ac1-122">In een nieuwe klantenkaart wordt de informatie uit de geselecteerde klantensjabloon getoond.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-122">A new customer card displays the information on the selected customer template.</span></span> <span data-ttu-id="d8ac1-123">Vul de overige velden in.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-123">Fill in the remaining fields.</span></span> <span data-ttu-id="d8ac1-124">Zie voor meer informatie [Nieuwe klanten registreren](sales-how-register-new-customers.md).</span><span class="sxs-lookup"><span data-stu-id="d8ac1-124">For more information, see [Register New Customers](sales-how-register-new-customers.md).</span></span>  
7. <span data-ttu-id="d8ac1-125">Wanneer u de klantenkaart hebt ingevuld, kiest u de knop **OK** om terug te keren naar het venster **Verkoopofferte**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-125">When you have completed the customer card, choose the **OK** button to return to the **Sales Quote** window.</span></span>

   <span data-ttu-id="d8ac1-126">Verschillende velden op de verkoopofferte worden nu ingevuld met gegevens die u hebt opgegeven op de nieuwe klantenkaart.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-126">Several fields on the sales quote are now filled with information that you specified on the new customer card.</span></span>  
8. <span data-ttu-id="d8ac1-127">Vul indien nodig de overige velden in het venster **Verkoopofferte** in.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-127">Fill in the remaining fields in the **Sales Quote** window as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

<span data-ttu-id="d8ac1-128">U kunt nu verkooporderregels invullen voor producten die u aan de klant verkoopt of voor elke transactie met de klant die u in een grootboekrekening wilt registreren.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-128">You are now ready to fill in the sales order lines for products that you are selling to the customer or for any transaction with the customer that you want to record in a G/L account.</span></span>   

<span data-ttu-id="d8ac1-129">Als u terugkerende verkoopregels voor de klant hebt ingesteld, zoals een maandelijkse aanvullingsorder, kunt u deze regels invoegen op de order door de actie **Terugkerende verkoopregels ophalen** te kiezen.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-129">If you have set up recurring sales lines for the customer, such as a monthly replenishment order, then you can insert these lines on the order by choosing the **Get Recurring Sales Lines** action.</span></span>  
9. <span data-ttu-id="d8ac1-130">Selecteer op het sneltabblad **Regels** in het veld **Soort** het type product, kosten of transactie die u wilt boeken voor de klant met deze verkoopregel.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-130">On the **Lines** FastTab, in the **Type** field, select what type of product, charge, or transaction that you will post for the customer with the sales line.</span></span>
10. <span data-ttu-id="d8ac1-131">Voer in het veld **Nr.**</span><span class="sxs-lookup"><span data-stu-id="d8ac1-131">In the **No.**</span></span> <span data-ttu-id="d8ac1-132">een record die u wilt boeken op basis van de waarde in het veld **Soort**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-132">field, select a record to post according to the value in the **Type** field.</span></span>

 <span data-ttu-id="d8ac1-133">Laat het veld **Nr.**</span><span class="sxs-lookup"><span data-stu-id="d8ac1-133">You leave the **No.**</span></span> <span data-ttu-id="d8ac1-134">leeg in de volgende gevallen: - Als de regel voor een opmerking is.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-134">field empty in the following cases: -If the line is for a comment.</span></span> <span data-ttu-id="d8ac1-135">Schrijf de opmerking in het veld **Omschrijving**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-135">Write the comment in the **Description** field.</span></span>
 <span data-ttu-id="d8ac1-136">- Als de regel voor een niet-voorraadartikel is.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-136">-If the line is for a nonstock item.</span></span> <span data-ttu-id="d8ac1-137">Kies de actie **Niet-voorraadartikelen selecteren**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-137">Choose the **Select Nonstock Items** action.</span></span> <span data-ttu-id="d8ac1-138">Zie voor meer informatie [Werken met niet-voorraadartikelen](inventory-how-work-nonstock-items.md).</span><span class="sxs-lookup"><span data-stu-id="d8ac1-138">For more information, see [Work With Nonstock Items](inventory-how-work-nonstock-items.md).</span></span>

11. <span data-ttu-id="d8ac1-139">Voer in het veld **Aantal** in hoeveel eenheden van het product, de kosten of de transactie met de regel voor de klant worden geregistreerd.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-139">In the **Quantity** field, enter how many units of the product, charge, or transaction that the line will record for the customer.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="d8ac1-140">Als het een artikel van de soort **Artikel - Service** of **Resource** betreft, is de hoeveelheid een tijdseenheid, bijvoorbeeld uren, zoals aangegeven in het veld **Eenheidscode** op de regel.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-140">If the item is of type **Item - Service** or **Resource**, the quantity is a time unit, such as hours, as indicated in the **Unit of Measure Code** field on the line.</span></span>  

    <span data-ttu-id="d8ac1-141">De waarde in het veld **Regelbedrag** wordt berekend als *Eenheidsprijs* x *Aantal*.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-141">The value in the **Line Amount** field is calculated as *Unit Price* x *Quantity*.</span></span>  

    <span data-ttu-id="d8ac1-142">De prijs en de regelbedragen worden weergegeven met of zonder btw, afhankelijk van wat u hebt geselecteerd in het veld **Prijzen inclusief btw** op de klantenkaart.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-142">The price and line amounts are with or without sales tax, depending on what you selected in the **Prices Including Tax** field on the customer card.</span></span>  
12. <span data-ttu-id="d8ac1-143">Als u een korting wilt geven, kunt u een percentage invoeren in het veld **Regelkorting %**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-143">If you want to give a discount, enter a percentage in the **Line Discount %** field.</span></span> <span data-ttu-id="d8ac1-144">De waarde in het veld **Regelbedrag** wordt dienovereenkomstig bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-144">The value in the **Line Amount** field updates accordingly.</span></span>  

    <span data-ttu-id="d8ac1-145">Als u speciale artikelprijzen hebt ingesteld op het sneltabblad **Verkoopprijzen en verkoopregelkortingen** op de klantenkaart of de artikelkaart, worden de prijs en het bedrag op de offerteregel automatisch bijgewerkt als aan de overeengekomen prijscriteria wordt voldaan.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-145">If special item prices are set up on the **Sales Prices and Sales Line Discounts** FastTab on the customer or item card, the price and amount on the sales line automatically update if the price criteria is met.</span></span> <span data-ttu-id="d8ac1-146">Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="d8ac1-146">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>  
13. <span data-ttu-id="d8ac1-147">Herhaal stap 9 t/m 12 voor elk product dat u aan de klant wilt aanbieden.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-147">Repeat steps 9 through 12 for every product you want to offer the customer.</span></span>  

    <span data-ttu-id="d8ac1-148">De totalen onder de regels worden automatisch berekend wanneer u regels maakt of wijzigt.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-148">The totals under the lines are automatically calculated as you create or modify lines.</span></span>  
14. <span data-ttu-id="d8ac1-149">In het veld **Kortingsbedrag op factuur** voert u een bedrag in dat moet worden afgetrokken van de waarde in het veld **Totaal incl. btw**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-149">In the **Invoice Discount Amount** field, enter an amount that should be deducted from the value shown in the **Total Incl. Tax** field.</span></span>

    <span data-ttu-id="d8ac1-150">Als u factuurkortingen voor de klant hebt opgegeven, wordt het opgegeven percentage automatisch ingevoegd in het veld **Factuurkorting %**als aan de voorwaarden wordt voldaan, en het gerelateerde bedrag wordt ingevoegd in het veld **Factuurkortingsbedrag excl. btw** .</span><span class="sxs-lookup"><span data-stu-id="d8ac1-150">If you have set up invoice discounts for the customer, then the specified percentage value is automatically inserted in the **Invoice Discount %** field if the criteria are met, and the related amount is inserted in the **Inv. Discount Amount Excl. Tax** field.</span></span> <span data-ttu-id="d8ac1-151">Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).</span><span class="sxs-lookup"><span data-stu-id="d8ac1-151">For more information, see [Record Sales Price, Discount, and Payment Agreements](sales-how-record-sales-price-discount-payment-agreements.md).</span></span>
15. <span data-ttu-id="d8ac1-152">Wanneer de verkoopofferteregels zijn ingevuld, kiest u de actie **Verzenden via e-mail**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-152">When the sales quote lines are completed, choose the **Send by Email** action.</span></span>
16. <span data-ttu-id="d8ac1-153">Vul in het venster **E-mail verzenden** eventuele overige velden in en controleer de ingesloten verkoopofferte.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-153">In the **Send Email** window, fill in any remaining fields and review the embedded sales quote.</span></span> <span data-ttu-id="d8ac1-154">Zie [Documenten per e-mail verzenden](ui-how-send-documents-email.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-154">For more information, see [Send Documents by Email](ui-how-send-documents-email.md).</span></span>
17. <span data-ttu-id="d8ac1-155">Als de klant de offerte accepteert, kiest u de actie **Factuur maken** of de actie **Order maken**.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-155">If the customer accepts the quote, choose the **Make Invoice** or the **Make Order** action.</span></span>

<span data-ttu-id="d8ac1-156">De verkoopofferte wordt verwijderd uit de database.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-156">The sales quote is removed from the database.</span></span> <span data-ttu-id="d8ac1-157">Een verkoopfactuur of een verkooporder wordt gemaakt op basis van de informatie in de verkoopofferte waarin u de verkoop kunt verwerken.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-157">A sales invoice or a sales order is created based on the information in the sales quote in which you can process the sale.</span></span> <span data-ttu-id="d8ac1-158">Op de verkoopfactuur of verkooporder vermeldt het veld **Offertenr.** het nummer van de verkoopofferte van waaruit het is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-158">In the **Quote No.** field on the sales invoice or sales order, you can see the number of the sales quote that it was made from.</span></span> <span data-ttu-id="d8ac1-159">Zie [Verkopen factureren](sales-how-invoice-sales.md) of [Producten verkopen](sales-how-sell-products.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d8ac1-159">For more information, see [Invoice Sales](sales-how-invoice-sales.md) or [Sell Products](sales-how-sell-products.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d8ac1-160">Zie ook</span><span class="sxs-lookup"><span data-stu-id="d8ac1-160">See Also</span></span>
[<span data-ttu-id="d8ac1-161">Verkoop</span><span class="sxs-lookup"><span data-stu-id="d8ac1-161">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="d8ac1-162">Verkopen instellen</span><span class="sxs-lookup"><span data-stu-id="d8ac1-162">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="d8ac1-163">Documenten per e-mail verzenden</span><span class="sxs-lookup"><span data-stu-id="d8ac1-163">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="d8ac1-164">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="d8ac1-164">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
