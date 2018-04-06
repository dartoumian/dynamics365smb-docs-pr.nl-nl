---
title: 'Procedure: artikelposten verwijderen en opnieuw toepassen | Microsoft Docs'
description: U kunt bepaalde artikelvereffeningsposten die automatisch worden gemaakt tijdens voorraadtransacties inzien en handmatig wijzigen.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 89fa84f814f3d7f53a842b1d675bf8143416b4d5
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="remove-and-reapply-item-ledger-entries"></a><span data-ttu-id="9847e-103">Artikelposten verwijderen en opnieuw toepassen</span><span class="sxs-lookup"><span data-stu-id="9847e-103">Remove and Reapply Item Ledger Entries</span></span>
<span data-ttu-id="9847e-104">U kunt in het venster **Vereffeningsvoorstel** bepaalde artikelvereffeningsposten die automatisch worden gemaakt tijdens voorraadtransacties inzien en handmatig wijzigen.</span><span class="sxs-lookup"><span data-stu-id="9847e-104">In the **Application Worksheet** window, you can view and manually change certain item application entries that are created automatically during inventory transactions.</span></span>  

<span data-ttu-id="9847e-105">Wanneer u een transactie boekt waarbij artikelen naar of uit voorraad worden verplaatst, wordt een artikelvereffening gemaakt tussen elke voorraadtoename en voorraadafname.</span><span class="sxs-lookup"><span data-stu-id="9847e-105">When you post a transaction where items are moved in or out of inventory, an item application is created between each inventory increase and inventory decrease.</span></span> <span data-ttu-id="9847e-106">Deze vereffeningen bepalen de kostenstroom van de goederen die in de voorraad zijn opgenomen naar de kosten die uit de voorraad worden gehaald.</span><span class="sxs-lookup"><span data-stu-id="9847e-106">These applications determine the flow of costs from the goods that are received in inventory to the cost of goods going out of inventory.</span></span> <span data-ttu-id="9847e-107">Vanwege de manier waarop de kostprijs wordt berekend, kan een onjuiste artikelvereffening leiden tot onjuiste gemiddelde kosten en tot een onjuiste kostprijs.</span><span class="sxs-lookup"><span data-stu-id="9847e-107">Because of the way the unit cost is calculated, an incorrect item application could lead to a skewed average cost and a skewed unit cost.</span></span> <span data-ttu-id="9847e-108">Zie Ontwerpdetails: artikelvereffening voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="9847e-108">For more information, see Design Details: Item Application.</span></span>

<span data-ttu-id="9847e-109">In de volgende scenario's moet u mogelijk een vereffening ongedaan maken of artikelposten opnieuw toepassen:</span><span class="sxs-lookup"><span data-stu-id="9847e-109">The following scenarios might require that you undo an application or reapply item ledger entries:</span></span>

- <span data-ttu-id="9847e-110">U bent vergeten een vaste vereffening te maken.</span><span class="sxs-lookup"><span data-stu-id="9847e-110">You have forgotten to make a fixed application.</span></span>
- <span data-ttu-id="9847e-111">U hebt een onjuiste vaste vereffening uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="9847e-111">You have made an incorrect fixed application.</span></span>
- <span data-ttu-id="9847e-112">U moet een artikel retourneren waarmee al een verkoop is vereffend.</span><span class="sxs-lookup"><span data-stu-id="9847e-112">You have to return an item to which a sale has already been applied.</span></span>

<span data-ttu-id="9847e-113">Gebruik indien mogelijk een document om een artikelpost opnieuw toe te passen.</span><span class="sxs-lookup"><span data-stu-id="9847e-113">If possible, use a document to reapply an item ledger entry.</span></span> <span data-ttu-id="9847e-114">Als u bijvoorbeeld een inkoopretour moet maken van een artikel dat al is vereffend met een verkoop, voert u de vereffening opnieuw uit door het inkoopretourdocument te maken en te boeken met de juiste vereffening in het veld **Vereffeningsnr. artikelpost** op de inkoopretourregel.</span><span class="sxs-lookup"><span data-stu-id="9847e-114">For example, if you must make a purchase return of an item to which a sale has already been applied, you can reapply by creating and posting the purchase return document by using the correct application in the **Appl.-to Item Entry** field on the purchase return line.</span></span> <span data-ttu-id="9847e-115">Dit gaat vooral gemakkelijk met de functie **Geboekte documentregels ophalen voor tegenboeking** of **Document kopiëren** in het inkoopretourdocument.</span><span class="sxs-lookup"><span data-stu-id="9847e-115">You can use the **Get Posted Document Lines to Reverse** function or the **Copy Document** function in the purchase return document to make this easier.</span></span> <span data-ttu-id="9847e-116">Wanneer u het document boekt, wordt de artikelpost automatisch opnieuw toegepast.</span><span class="sxs-lookup"><span data-stu-id="9847e-116">When you post the document, the item ledger entry is automatically reapplied.</span></span> <span data-ttu-id="9847e-117">Zie voor meer informatie [Inkoopretouren of annuleringen verwerken](purchasing-how-process-purchase-returns-cancellations.md).</span><span class="sxs-lookup"><span data-stu-id="9847e-117">For more information, see [Process Purchase Returns or Cancellations](purchasing-how-process-purchase-returns-cancellations.md).</span></span>

<span data-ttu-id="9847e-118">Als het niet mogelijk is om een document te gebruiken voor het opnieuw uitvoeren van een vereffening, als u bijvoorbeeld een vaste vereffening moet corrigeren, gebruikt u het venster **Vereffeningsvoorstel** om een vereffening te corrigeren.</span><span class="sxs-lookup"><span data-stu-id="9847e-118">If you cannot use a document to reapply, such as when you have to correct a fixed application, then use the **Application Worksheet** window to correct an application.</span></span>

> [!Warning]  
> <span data-ttu-id="9847e-119">Houd het volgende in gedachten wanneer u met het toepassingsvoorstel werkt:</span><span class="sxs-lookup"><span data-stu-id="9847e-119">The following are important considerations to remember when you are working with the application worksheet:</span></span>
    - <span data-ttu-id="9847e-120">U moet het opnieuw uitvoeren van een vereffening voor vereffeningsposten niet langere tijd uitstellen, omdat andere gebruikers de artikelen niet kunnen verwerken totdat u de vereffeningsposten opnieuw vereffent of het venster **Vereffeningsvoorstel** sluit.</span><span class="sxs-lookup"><span data-stu-id="9847e-120">You should not leave application entries unapplied for long periods of time because other users cannot process the items until you reapply the application entries or close the **Application Worksheet** window.</span></span> <span data-ttu-id="9847e-121">Gebruikers die acties willen uitvoeren voor een vereffeningspost waarvan de vereffening handmatig ongedaan is gemaakt, ontvangen het volgende foutmelding: "U kunt deze handeling niet uitvoeren omdat de posten voor artikel XXX niet vereffend zijn in het vereffeningsvoorstel door gebruiker XXX."</span><span class="sxs-lookup"><span data-stu-id="9847e-121">Users who try to perform actions that involve a manually unapplied application entry receive the following error message: “You cannot perform this action because entries for item XXX are unapplied in the Application Worksheet by user XXX.”</span></span>
    - <span data-ttu-id="9847e-122">U moet artikelposten alleen buiten de gebruikelijke werktijden opnieuw vereffenen. Zo voorkomt u eventuele conflicten met andere gebruikers die transacties voor dezelfde artikelen boeken.</span><span class="sxs-lookup"><span data-stu-id="9847e-122">You should only reapply item ledger entries during nonworking hours to avoid conflicts with other users who are posting transactions with the same items.</span></span>
    - <span data-ttu-id="9847e-123">Wanneer u het vereffeningsvoorstel sluit, voert [!INCLUDE[d365fin](includes/d365fin_md.md)] een controle uit om ervoor te zorgen dat alle posten zijn toegepast.</span><span class="sxs-lookup"><span data-stu-id="9847e-123">When you close the application worksheet, [!INCLUDE[d365fin](includes/d365fin_md.md)] performs a check to make sure that all entries are applied.</span></span> <span data-ttu-id="9847e-124">Als u bijvoorbeeld een aantalvereffening verwijdert en geen nieuwe vereffening maakt, zal bij het sluiten van het vereffeningsvoorstel alsnog een nieuwe vereffening worden aangemaakt.</span><span class="sxs-lookup"><span data-stu-id="9847e-124">For example, if you remove a quantity application but do not create a new application, and then you close the application worksheet, a new application is created.</span></span> <span data-ttu-id="9847e-125">Zo blijven de kosten intact.</span><span class="sxs-lookup"><span data-stu-id="9847e-125">This helps keep the cost intact.</span></span> <span data-ttu-id="9847e-126">Als u echter een vaste vereffening verwijdert, wordt niet automatisch een nieuwe vaste vereffening gemaakt bij het sluiten van het voorstel.</span><span class="sxs-lookup"><span data-stu-id="9847e-126">However, if you remove a fixed application, a new fixed application is not automatically created when you close the worksheet.</span></span> <span data-ttu-id="9847e-127">U moet dan zelf een nieuwe vereffening aanmaken in het voorstel.</span><span class="sxs-lookup"><span data-stu-id="9847e-127">You must do this manually by creating a new application in the worksheet.</span></span>
    - <span data-ttu-id="9847e-128">U kunt in het toepassingsvoorstel vereffeningen uit meerdere posten tegelijk verwijderen.</span><span class="sxs-lookup"><span data-stu-id="9847e-128">It is possible to remove applications from more than one entry at a time in the application worksheet.</span></span> <span data-ttu-id="9847e-129">Aangezien het vereffenen van posten echter invloed heeft op de posten die beschikbaar zijn voor vereffening, kunt u geen vereffening maken voor meerdere posten tegelijk.</span><span class="sxs-lookup"><span data-stu-id="9847e-129">However, because applying entries affects the set of entries that are available for application, you cannot create an application for more than one entry at a time.</span></span>
    - <span data-ttu-id="9847e-130">Het toepassingsvoorstel kan onder de volgende omstandigheden geen vereffening maken: als er onvoldoende aantallen in voorraad zijn om te vereffenen, kan het toepassingsvoorstel geen vereffening maken wanneer u een negatieve voorraadmutatiepost zonder artikeltraceringsinformatie probeert te vereffenen met een positieve voorraadmutatiepost met artikeltraceringsinformatie.</span><span class="sxs-lookup"><span data-stu-id="9847e-130">The application worksheet cannot make an application in the following situation: If there is not enough quantity on stock to apply, the application worksheet cannot make an application when you are trying to apply an inventory decrease entry without item tracking information to an inventory increase entry with item tracking information.</span></span>

## <a name="to-remove-an-item-application-by-using-the-application-worksheet"></a><span data-ttu-id="9847e-131">Een artikelvereffening verwijderen met het Vereffeningsvoorstel</span><span class="sxs-lookup"><span data-stu-id="9847e-131">To remove an item application by using the Application Worksheet</span></span>  
1.  <span data-ttu-id="9847e-132">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vereffeningsvoorstel** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9847e-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Application Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9847e-133">Het venster **Vereffeningsvoorstel** wordt geopend en toont bestaande artikelposten voor alle items.</span><span class="sxs-lookup"><span data-stu-id="9847e-133">The **Application Worksheet** window opens displaying existing item ledger entries for all items.</span></span>  
3.  <span data-ttu-id="9847e-134">Voer filters in op het sneltabblad **Algemeen** om de artikelpost waarvoor u de vereffening wilt wijzigen makkelijker te kunnen vinden.</span><span class="sxs-lookup"><span data-stu-id="9847e-134">Enter filters on the **General** FastTab to make it easier to find the item ledger entry for which you want to change the application.</span></span>  
4.  <span data-ttu-id="9847e-135">Selecteer de artikelpost en kies de actie **Vereffende posten**.</span><span class="sxs-lookup"><span data-stu-id="9847e-135">Select the item ledger entry, and then choose the **Applied Entries** action.</span></span> <span data-ttu-id="9847e-136">Het venster **Vereffende posten weergeven - Vereffende posten** wordt geopend, met daarin de artikelpost of de artikelposten die met de geselecteerde post zijn vereffend.</span><span class="sxs-lookup"><span data-stu-id="9847e-136">The **View Applied Entries – Applied Entries** window opens to show the item ledger entry or entries that are currently applied to the selected entry.</span></span>  
5.  <span data-ttu-id="9847e-137">Selecteer de artikelpost waarvoor u de vereffening wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="9847e-137">Select the item ledger entry for which you want to remove the application.</span></span>  
6.  <span data-ttu-id="9847e-138">Kies de actie **Vereffening verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="9847e-138">Choose the **Remove Application** action.</span></span> <span data-ttu-id="9847e-139">De artikelvereffeningspost die de twee artikelposten koppelt, wordt dan verwijderd en naar het venster **Vereffende posten weergeven - Niet-vereffende posten** verplaatst.</span><span class="sxs-lookup"><span data-stu-id="9847e-139">This removes the item application entry that links the two item ledger entries and moves it to the **View Applied Entries – Unapplied Entries** window.</span></span>  
7.  <span data-ttu-id="9847e-140">Sluit het venster **Vereffende posten weergeven - Vereffende posten**.</span><span class="sxs-lookup"><span data-stu-id="9847e-140">Close the **View Applied Entries – Applied Entries** window.</span></span>  

 <span data-ttu-id="9847e-141">Het veld **Resterend aantal** van de twee artikelposten worden verhoogd met het niet-vereffende aantal.</span><span class="sxs-lookup"><span data-stu-id="9847e-141">The **Remaining Quantity** field of the two item ledger entries are increased by the quantity that has been unapplied.</span></span> <span data-ttu-id="9847e-142">De verwijderde artikelpost kan nu opnieuw worden vereffend in het venster **Vereffende posten weergeven - Niet-vereffende posten**.</span><span class="sxs-lookup"><span data-stu-id="9847e-142">The removed item ledger entry is now available for reapplication in the **View Applied Entries – Unapplied Entries** window.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="9847e-143">U moet het opnieuw uitvoeren van een vereffening voor vereffeningsposten niet langere tijd uitstellen, omdat andere gebruikers de betrokken artikelen niet kunnen verwerken totdat u de vereffeningsposten opnieuw vereffent of het venster **Vereffeningsvoorstel** sluit.</span><span class="sxs-lookup"><span data-stu-id="9847e-143">You should not leave application entries unapplied for longer periods of time because other users cannot process the affected items until you reapply the application entries or close the **Application Worksheet** window.</span></span> <span data-ttu-id="9847e-144">De volgende foutmelding wordt weergegeven als u probeert bewerkingen uit te voeren waar een handmatig niet-vereffende vereffeningspost in is opgenomen:</span><span class="sxs-lookup"><span data-stu-id="9847e-144">The following error message is displayed if you try to perform actions that involve a manually unapplied application entry:</span></span>  
>   
>  <span data-ttu-id="9847e-145">**U kunt deze handeling niet uitvoeren omdat posten voor artikel <item> niet vereffend zijn in het Vereffeningsvoorstel door gebruiker <user>.**</span><span class="sxs-lookup"><span data-stu-id="9847e-145">**You cannot perform this action because entries for item <item> are unapplied in the Application Worksheet by user <user>.**</span></span>  

## <a name="to-reapply-an-item-application-by-using-the-application-worksheet"></a><span data-ttu-id="9847e-146">Een artikelvereffening opnieuw vereffenen met het Vereffeningsvoorstel</span><span class="sxs-lookup"><span data-stu-id="9847e-146">To reapply an item application by using the Application Worksheet</span></span>  
1.  <span data-ttu-id="9847e-147">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vereffeningsvoorstel** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9847e-147">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Application Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="9847e-148">Het venster **Vereffeningsvoorstel** wordt geopend en toont bestaande artikelposten voor alle items.</span><span class="sxs-lookup"><span data-stu-id="9847e-148">The **Application Worksheet** window opens displaying existing item ledger entries for all items.</span></span>  
3.  <span data-ttu-id="9847e-149">Als u posten opnieuw wilt vereffenen die zijn verwijderd na het openen van het voorstel, selecteert u de artikelpost die u opnieuw wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="9847e-149">To reapply entries that were removed since the worksheet was opened, select the item ledger entry that you want to reapply.</span></span> <span data-ttu-id="9847e-150">Kies op het tabblad **Acties** in de groep **Functies** de optie **Opnieuw vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="9847e-150">On the **Actions** tab, in the **Functions** group, choose **Reapply**.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9847e-151">Deze vereffening van het oorspronkelijke aantal gebeurt ook automatisch wanneer u het venster **Vereffeningsvoorstel** sluit.</span><span class="sxs-lookup"><span data-stu-id="9847e-151">This reapplication to the original balance also occurs automatically when you close the **Application Worksheet** window.</span></span>  
4.  <span data-ttu-id="9847e-152">Selecteer om een beschikbare open artikelpost op een andere post te vereffenen de artikelpost die u wilt vereffenen.</span><span class="sxs-lookup"><span data-stu-id="9847e-152">To apply an available open item ledger entry to another entry, select the item ledger entry that you want to apply.</span></span> <span data-ttu-id="9847e-153">Kies de actie **Niet-toegepaste posten**.</span><span class="sxs-lookup"><span data-stu-id="9847e-153">Choose the **Unapplied Entries** action.</span></span> <span data-ttu-id="9847e-154">Het venster **Vereffende posten weergeven - Niet-vereffende posten** opent.</span><span class="sxs-lookup"><span data-stu-id="9847e-154">The **View Applied Entries – Unapplied Entries** window opens.</span></span>  
5.  <span data-ttu-id="9847e-155">Selecteer een of meer artikelposten die u wilt vereffenen met de post die is geselecteerd in het venster **Vereffeningsvoorstel** en klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="9847e-155">Select one or more item ledger entries that you want to apply to the entry selected in the **Application Worksheet** window, and then choose the **OK** button.</span></span>  

     <span data-ttu-id="9847e-156">Er wordt een artikelvereffeningspost gemaakt tussen de twee artikelposten.</span><span class="sxs-lookup"><span data-stu-id="9847e-156">An item application entry is created between the two item ledger entries.</span></span> <span data-ttu-id="9847e-157">De velden **Resterend aantal** van de twee posten worden gereduceerd met het vereffende aantal.</span><span class="sxs-lookup"><span data-stu-id="9847e-157">The **Remaining Quantity** fields of the two entries are reduced by the applied quantity.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9847e-158">Als u ervoor hebt gekozen een vereffening uit te voeren die tijdens het herwaarderen van de kosten tot een oneindige herhaling zou leiden, wordt de door u voorgestelde vereffening niet uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="9847e-158">If you have chosen to make an application that would create an infinite loop in the cost adjustment process, then the application that you proposed is not made.</span></span> <span data-ttu-id="9847e-159">Dit kan voorkomen wanneer de originele posten negatieve voorraad hebben veroorzaakt.</span><span class="sxs-lookup"><span data-stu-id="9847e-159">This can occur when the original entries created negative stock.</span></span> <span data-ttu-id="9847e-160">De vereffening wordt niet uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="9847e-160">The application is not made.</span></span> <span data-ttu-id="9847e-161">Daarom moet u een andere post selecteren voor de vereffening.</span><span class="sxs-lookup"><span data-stu-id="9847e-161">Therefore, you must select a different entry for the application.</span></span>  
6.  <span data-ttu-id="9847e-162">Als het veld **Automatische kostenwaardering** in de **Voorraadinstelling** is ingesteld op **Altijd**, voert het programma de batchverwerking voor het herwaarderen van de kosten automatisch uit nadat u een vereffening opnieuw hebt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="9847e-162">If the **Automatic Cost Adjustment** field in the **Inventory Setup** is set to **Always**, then the cost adjustment batch job is automatically run after you make a reapplication.</span></span> <span data-ttu-id="9847e-163">Anders voert u de batchverwerking **Kostprijs herwaarderen - Artikelposten** uit om er zeker van zijn dat alle kosten up-to-date zijn.</span><span class="sxs-lookup"><span data-stu-id="9847e-163">Otherwise, run the **Adjust Cost - Item Entries** batch job to make sure that all costs are up to date.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9847e-164">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9847e-164">See Also</span></span>  
[<span data-ttu-id="9847e-165">Open artikelposten die uit een vaste vereffening in het artikeldagboek voortkomen sluiten</span><span class="sxs-lookup"><span data-stu-id="9847e-165">Close Open Item Ledger Entries Resulting from Fixed Application in the Item Journal</span></span>](finance-how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal.md)  
 [<span data-ttu-id="9847e-166">Inkoopretouren of annuleringen verwerken</span><span class="sxs-lookup"><span data-stu-id="9847e-166">Process Purchase Returns or Cancellations</span></span>](purchasing-how-process-purchase-returns-cancellations.md)  
 <span data-ttu-id="9847e-167">[Voorraadkosten beheren](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="9847e-167">[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
 [<span data-ttu-id="9847e-168">Ontwerpdetails: Artikelvereffening</span><span class="sxs-lookup"><span data-stu-id="9847e-168">Design Details: Item Application</span></span>](design-details-item-application.md)  
 <span data-ttu-id="9847e-169">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9847e-169">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
