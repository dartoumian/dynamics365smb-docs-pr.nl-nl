---
title: Artikelen opslaan met magazijnopslag | Microsoft Docs
description: Wanneer voor de vestiging magazijnopslag- en -ontvangstverwerking is vereist, beheert u de opslag van artikelen met de functie voor magazijnopslagdocumenten.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/31/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: bf7b58fad1aa587079b51b505e9d757bb66f39c9
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="put-items-away-with-warehouse-put-aways"></a><span data-ttu-id="b8a53-103">Artikelen opslaan met magazijnopslag</span><span class="sxs-lookup"><span data-stu-id="b8a53-103">Put Items Away with Warehouse Put-aways</span></span>
<span data-ttu-id="b8a53-104">Wanneer voor de vestiging magazijnopslag- en -ontvangstverwerking is vereist, beheert u de opslag van artikelen met de functie voor magazijnopslagdocumenten.</span><span class="sxs-lookup"><span data-stu-id="b8a53-104">When your location is set up to require warehouse put-away processing and warehouse receive processing, you use the warehouse put-away documents function to control the putting away of items.</span></span>  

<span data-ttu-id="b8a53-105">Als u een magazijnontvangst boekt, worden de brondocumenten zoals inkooporder, inkomende transferorder of verkoopretourorder bijgewerkt, de ontvangen aantallen geboekt in de artikelposten en de regels over de ontvangen artikelen naar de opslagfunctie van het magazijn verzonden.</span><span class="sxs-lookup"><span data-stu-id="b8a53-105">When you post a warehouse receipt, the source documents, such as purchase, inbound transfer, or sales return orders, are updated, the quantity received is posted to the item ledger, and the lines about the items received are sent to the put-away function in the warehouse.</span></span> <span data-ttu-id="b8a53-106">Als u met interne opslag en pick werkt, kunnen ook opslagregels worden gegenereerd door de interne opslag.</span><span class="sxs-lookup"><span data-stu-id="b8a53-106">If you have internal put-away and pick, the internal put-away can also create lines for put-away.</span></span>  

<span data-ttu-id="b8a53-107">Afhankelijk van de magazijninstellingen worden de regels beschikbaar gemaakt in het opslagvoorstel of worden direct opslaginstructies gemaakt.</span><span class="sxs-lookup"><span data-stu-id="b8a53-107">Depending on the warehouse setup, the lines are either made available to the put-away worksheet or used to generate put-away instructions immediately.</span></span> <span data-ttu-id="b8a53-108">Zie [Opslag plannen in voorstellen](warehouse-how-to-plan-put-aways-in-worksheets.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b8a53-108">For more information, see [Plan Put-aways in Worksheets](warehouse-how-to-plan-put-aways-in-worksheets.md).</span></span>  

<span data-ttu-id="b8a53-109">Naast de standaard manieren waarop magazijnopslag gemaakt kan worden die in dit onderwerp worden beschreven, kunt u opslag maken vanuit de bijbehorende geboekte magazijnontvangst.</span><span class="sxs-lookup"><span data-stu-id="b8a53-109">In addition to the standard ways to create warehouse put-aways that are described in this topic, you can create the put-away from the related posted warehouse receipt.</span></span> <span data-ttu-id="b8a53-110">Dit is nuttig als u opslagregels hebt verwijderd of als u gestuurde opslag en pick gebruikt en het opslagwerkblad niet wilt gebruiken omdat u opslaginstructies (opnieuw) kunt maken van de geboekte ontvangstregels.</span><span class="sxs-lookup"><span data-stu-id="b8a53-110">This is useful if you have deleted put-away lines, or if you use directed put-away and pick and have decided not to use the put-away worksheet, because you can create or recreate put-away instructions from the posted receipt lines.</span></span>  

## <a name="to-put-items-away-without-directed-put-away-and-pick"></a><span data-ttu-id="b8a53-111">Artikelen opslaan zonder gestuurde opslag en pick</span><span class="sxs-lookup"><span data-stu-id="b8a53-111">To put items away without directed put-away and pick</span></span>  
1.  <span data-ttu-id="b8a53-112">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnopslag** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="b8a53-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Put-aways**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b8a53-113">Open de magazijnopslag die gereed is om te verwerken.</span><span class="sxs-lookup"><span data-stu-id="b8a53-113">Open the warehouse put-away that is ready to handle.</span></span>  

    <span data-ttu-id="b8a53-114">U kunt de opslagregels op grond van diverse criteria sorteren, bijvoorbeeld op artikel, schapnummer of vervaldatum en op deze manier het opslagproces optimaliseren.</span><span class="sxs-lookup"><span data-stu-id="b8a53-114">You can sort the put-away lines by various criteria, for example, by item, shelf number, or due date, and thereby optimize the put-away process.</span></span>  
3.  <span data-ttu-id="b8a53-115">Voer op elke regel het aantal dat u wilt opslaan in het veld **Te verwerken aantal** in.</span><span class="sxs-lookup"><span data-stu-id="b8a53-115">On each line, in the **Qty. to Handle** field, enter the quantity you want to put away.</span></span>  
4.  <span data-ttu-id="b8a53-116">Als u de opslag van artikelen hebt voltooid, kiest u de actie **Opslag registreren** om de voltooiing van de activiteit te registreren en de artikelen beschikbaar te maken voor pickacties.</span><span class="sxs-lookup"><span data-stu-id="b8a53-116">After you have completed putting the items away, choose the **Register Put-away** action to record the completion of the activity and make the items available for picking.</span></span>  

## <a name="to-put-items-away-with-directed-put-away-and-pick"></a><span data-ttu-id="b8a53-117">Artikelen opslaan met gestuurde opslag en pick</span><span class="sxs-lookup"><span data-stu-id="b8a53-117">To put items away with directed put-away and pick</span></span>  
1.  <span data-ttu-id="b8a53-118">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnopslag** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="b8a53-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Put-aways**, and then choose the related link.</span></span>
    <span data-ttu-id="b8a53-119">Als er opslaginstructies zijn gemaakt, wordt er een magazijnopslag weergegeven.</span><span class="sxs-lookup"><span data-stu-id="b8a53-119">If put-away instructions have been created, a warehouse put-away is visible.</span></span>  
2.  <span data-ttu-id="b8a53-120">Open de magazijnopslag waaraan u wilt werken.</span><span class="sxs-lookup"><span data-stu-id="b8a53-120">Open the warehouse put-away that you want to work on.</span></span>  
3.  <span data-ttu-id="b8a53-121">Als voor het magazijn een gebruikers-id is vereist, voert u deze eerst in op het sneltabblad **Algemeen**. Daarna kunt u de gewenste opslag bewerken.</span><span class="sxs-lookup"><span data-stu-id="b8a53-121">If your warehouse requires, enter your user ID on the **General** FastTab when you begin work on a particular put-away.</span></span>  
4.  <span data-ttu-id="b8a53-122">Voer de Nemen- en Plaatsen-acties uit in het veld **Actiesoort** op de regels.</span><span class="sxs-lookup"><span data-stu-id="b8a53-122">Perform the take and place actions indicated in the **Action Type** field on the lines.</span></span>  

    <span data-ttu-id="b8a53-123">Elke ontvangstregel is in de magazijnopslag omgezet in ten minste twee regels:</span><span class="sxs-lookup"><span data-stu-id="b8a53-123">Note that each receipt line has become at least two lines in the warehouse put-away:</span></span>  

    -   <span data-ttu-id="b8a53-124">De eerste regel met **Nemen** in het veld **actiesoort** geeft aan waar de artikelen zich in het ontvangstgebied bevinden.</span><span class="sxs-lookup"><span data-stu-id="b8a53-124">The first line, with **Take** in the **Action Type** field, indicates where the items are located in the receiving area.</span></span> <span data-ttu-id="b8a53-125">U kunt de zone en de opslaglocatie op deze regel niet wijzigen.</span><span class="sxs-lookup"><span data-stu-id="b8a53-125">You cannot change the zone and bin field on this line.</span></span>  
    -   <span data-ttu-id="b8a53-126">De volgende regel met **Plaatsen als** in het veld **actiesoort** geeft aan waar u de artikelen in de magazijnopslag moet plaatsen.</span><span class="sxs-lookup"><span data-stu-id="b8a53-126">The next line, with **Place** in the **Action Type** field, shows where you must place the items in warehouse storage.</span></span> <span data-ttu-id="b8a53-127">Als er een groot aantal artikelen via één ontvangstregel het magazijn is binnengekomen, moeten de artikelen mogelijk op verschillende opslaglocaties worden opgeslagen en wordt er een Plaatsen-regel voor elke opslaglocatie weergegeven.</span><span class="sxs-lookup"><span data-stu-id="b8a53-127">If the warehouse has received a large number of items on one receipt line, they may have to be put away in several bins, so there is a Place line for each bin.</span></span>  

        <span data-ttu-id="b8a53-128">Als de Nemen- en Plaatsen-regels op de ontvangstregels niet opeenvolgend worden weergegeven, kunt u de regels sorteren door **Artikel** te selecteren in het veld **Sorteringsmethode** op het sneltabblad **Algemeen**.</span><span class="sxs-lookup"><span data-stu-id="b8a53-128">If the Take and Place lines for each receipt line do not immediately follow one another, and you want them to do so, you can sort the lines by selecting **Item** in the **Sorting Method** field on the **General** FastTab.</span></span>  

        <span data-ttu-id="b8a53-129">Als de fysieke indeling van het magazijn en de rangorde van opslaglocaties met elkaar overeenkomen, kunt u de sorteermethode **Opslaglocatievolgorde** gebruiken om een opslag voor te bereiden waarin uw rondgang door het magazijn zo efficiënt mogelijk verloopt.</span><span class="sxs-lookup"><span data-stu-id="b8a53-129">If the physical layout of the warehouse reflects the bin rankings, you can use the **Bin Ranking** sorting method to prepare a put-away round that will minimize your steps through the warehouse.</span></span>  

5.  <span data-ttu-id="b8a53-130">Als u alle artikelen volgens de instructies op de opslaglocaties hebt geplaatst, kiest u de actie **Opslag registreren**.</span><span class="sxs-lookup"><span data-stu-id="b8a53-130">When you have placed all the items in bins as instructed, choose the **Register Put-away** action.</span></span>  

<span data-ttu-id="b8a53-131">Op locaties die zijn ingesteld voor gestuurde opslag en pick, zijn de volgende instellingen vereisten voor bovenstaande procedure:</span><span class="sxs-lookup"><span data-stu-id="b8a53-131">At locations that are set up to use directed put-away and pick, the following settings are prerequisites for the procedure above:</span></span>  

- <span data-ttu-id="b8a53-132">Er wordt een opslagsjablonen ingesteld.</span><span class="sxs-lookup"><span data-stu-id="b8a53-132">A put-away template is set up.</span></span> <span data-ttu-id="b8a53-133">Zie voor meer informatie [Opslagsjablonen instellen](warehouse-how-to-set-up-put-away-templates.md).</span><span class="sxs-lookup"><span data-stu-id="b8a53-133">For more information, see [Set Up Put-away Templates](warehouse-how-to-set-up-put-away-templates.md).</span></span>  
- <span data-ttu-id="b8a53-134">Het gewicht, het volume en de speciale opslagvereisten van het artikel of de SKU worden opgegeven.</span><span class="sxs-lookup"><span data-stu-id="b8a53-134">The weight, cubage, and special storage requirements of the item or stockkeeping unit are defined.</span></span> <span data-ttu-id="b8a53-135">Zie voor meer informatie Brutogewicht.</span><span class="sxs-lookup"><span data-stu-id="b8a53-135">For more information, see Gross Weight.</span></span>  
- <span data-ttu-id="b8a53-136">De capaciteit, de soort opslaglocatie en de volgorde van de opslaglocaties. Zie Opslaglocatievolgorde voor meer informatie .</span><span class="sxs-lookup"><span data-stu-id="b8a53-136">The capacity, bin type, and bin ranking of the bins. For more information, see Bin Ranking.</span></span>  

<span data-ttu-id="b8a53-137">De opslaglocatievolgorde wordt gebruikt wanneer meerdere opslaglocaties voldoen aan de opslagsjablooncriteria.</span><span class="sxs-lookup"><span data-stu-id="b8a53-137">The bin ranking is taken into consideration when more than one bin matches put-away template criteria.</span></span> <span data-ttu-id="b8a53-138">Als meerdere opslaglocaties voldoen aan de criteria van de opslagsjabloon en dezelfde rang in de opslaglocatievolgorde hebben, wordt de opslaglocatie met het hoogste opslaglocatienummer gebruikt.</span><span class="sxs-lookup"><span data-stu-id="b8a53-138">If both the put-away template criteria and the bin ranking are the same for more than one bin, the bin with the highest number is selected.</span></span>

## <a name="to-create-a-put-away-from-a-posted-receipt"></a><span data-ttu-id="b8a53-139">Een magazijnopslag maken vanuit een geboekte ontvangst</span><span class="sxs-lookup"><span data-stu-id="b8a53-139">To create a put-away from a posted receipt</span></span>  
 <span data-ttu-id="b8a53-140">Als bij uw vestiging zowel opslagverwerking als ontvangstverwerking wordt gebruikt en u opslagregels hebt verwijderd, of als u gestuurde opslag en pick gebruikt en het opslagwerkblad niet wilt gebruiken, kunt u opslaginstructies (opnieuw) maken voor de geboekte ontvangstregels.</span><span class="sxs-lookup"><span data-stu-id="b8a53-140">If your location uses both put-away processing and receive processing and you have deleted put-away lines, or if you use directed put-away and pick and have decided not to use the put-away worksheet, you can create or recreate put-away instructions for the posted receipt lines.</span></span>

1.  <span data-ttu-id="b8a53-141">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Geboekte magazijnontvangsten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="b8a53-141">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Whse. Receipts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b8a53-142">Selecteer een geboekte ontvangst die mogelijk moet worden opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="b8a53-142">Select a posted receipt that might need to be put away.</span></span>  
3.  <span data-ttu-id="b8a53-143">Kies de actie **Kaart**.</span><span class="sxs-lookup"><span data-stu-id="b8a53-143">Choose the **Card** action.</span></span>  

    <span data-ttu-id="b8a53-144">Als het veld **Documentstatus** leeg is, is de ontvangst nog niet opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="b8a53-144">If the **Document Status** field is blank, the receipt has not been put away at all.</span></span> <span data-ttu-id="b8a53-145">Anders geeft het veld aan dat de ontvangst gedeeltelijk opslaan of volledig opslaan betreft.</span><span class="sxs-lookup"><span data-stu-id="b8a53-145">Otherwise, the field indicates the receipt is partially put-away or completely put-away.</span></span>  

4.  <span data-ttu-id="b8a53-146">Als de ontvangst gedeeltelijk is opgeslagen of nog niet is opgeslagen, kiest u de actie **Opslag maken**.</span><span class="sxs-lookup"><span data-stu-id="b8a53-146">If the receipt is partially put away or not put away at all, choose the **Create Put-away** action.</span></span>  
5.  <span data-ttu-id="b8a53-147">Vul het aanvraagvenster voor de batchverwerking in om de opslaginstructies te maken en klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="b8a53-147">Fill in the batch job request window to create the put-away, and then choose the **OK** button.</span></span>   

## <a name="see-also"></a><span data-ttu-id="b8a53-148">Zie ook</span><span class="sxs-lookup"><span data-stu-id="b8a53-148">See Also</span></span>  
[<span data-ttu-id="b8a53-149">Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="b8a53-149">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="b8a53-150">Voorraad</span><span class="sxs-lookup"><span data-stu-id="b8a53-150">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="b8a53-151">[Magazijnbeheer instellen](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="b8a53-151">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="b8a53-152">[Assemblagebeheer](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="b8a53-152">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="b8a53-153">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="b8a53-153">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="b8a53-154">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="b8a53-154">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
