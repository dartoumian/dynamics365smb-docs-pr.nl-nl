---
title: Picks plannen in het voorstel | Microsoft Docs
description: Als voor het magazijn zowel pick- als verzendingsverwerking is vereist, hebt u de keuze om van de regels op verzenddocumenten niet automatisch pickinstructies te maken, maar de regels beschikbaar te stellen in het pickvoorstel.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 073cc86b9df5845fbce18804756f980649f94081
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="plan-picks-in-worksheets"></a><span data-ttu-id="0f3c2-103">Picks plannen in het voorstel</span><span class="sxs-lookup"><span data-stu-id="0f3c2-103">Plan Picks in Worksheets</span></span>
<span data-ttu-id="0f3c2-104">Als voor het magazijn zowel pick- als verzendingsverwerking is vereist, hebt u de keuze om van de regels op verzenddocumenten niet automatisch pickinstructies te maken, maar de regels beschikbaar te stellen in het pickvoorstel.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-104">If your warehouse is set up to require both pick and shipment processing, the warehouse can choose to operate so that the lines on shipment documents are not automatically transformed into pick instructions, but are made available instead to the pick worksheet.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0f3c2-105">Als de pickinstructies voor het magazijn al zijn gemaakt maar u ze wilt combineren tot één efficiënte pickinstructie, moet u de afzonderlijke magazijnpicks verwijderen.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-105">If warehouse pick instructions have already been created, and you would like to combine them into one efficient pick instruction, then you must delete the individual warehouse picks.</span></span> <span data-ttu-id="0f3c2-106">De te picken regels kunnen nu in het voorstel worden geplaatst.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-106">The lines to be picked can now be listed in the worksheet.</span></span>  

<span data-ttu-id="0f3c2-107">In het pickvoorstel kunt u picklijsten instellen voor werknemers. Deze picklijsten beperken de tijd die de werknemer nodig heeft om zich te verplaatsen voor het picken van artikelen in het magazijn.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-107">In the pick worksheet, you can set up pick lists for employees that minimize the time the employee has to move about the warehouse picking items.</span></span> <span data-ttu-id="0f3c2-108">Er zijn velden die informatie over de beschikbare aantal artikelen in de cross-dockopslaglocaties bevatten. Dit is handig bij cross-dockgevallen om de werkopdrachten te plannen, omdat het programma altijd een pick voorstelt van een cross-dockopslaglocatie vóór een andere opslaglocatie, onafhankelijk van de eenheid.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-108">There are fields that contain information about the quantities of items available in the cross-dock bins. This is useful in cross docking situations to plan your work assignments, because the program will always propose a pick from a cross-dock bin before any other bin, regardless of the unit of measure.</span></span> <span data-ttu-id="0f3c2-109">De regels in het voorstel kunnen afkomstig zijn uit een aantal brondocumenten en worden gesorteerd op artikel, schapnummer, brondocument, vervaldatum of verzendadres.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-109">The lines in the worksheet can come from a number of source documents and be sorted by item, shelf number, source document, due date, or ship-to address.</span></span>  

<span data-ttu-id="0f3c2-110">Bij een sortering op vervaldatum hebt u de keuze om de regels die geen directe aandacht behoeven uit het voorstel te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-110">If you sort by due date, you can choose to delete from the worksheet all lines except those that need immediate attention.</span></span> <span data-ttu-id="0f3c2-111">De minder urgente regels worden niet feitelijk verwijderd, maar alleen teruggestuurd naar de **pickselectie**.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-111">The less urgent lines are not deleted as such, but just sent back to the **Pick Selection** worksheet.</span></span> <span data-ttu-id="0f3c2-112">Als u de pick maakt, zijn de regels al gesorteerd op vervaldatum en kunt u de pick vervolgens toewijzen aan een bepaalde werknemer.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-112">When you create the pick, the lines have already been sorted by due date, and you can choose to assign the pick to a particular employee.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="0f3c2-113">Het picken voor magazijnverzending van artikelen die worden samengesteld voor de verkooporder die wordt verzonden volgt dezelfde stappen als gewone magazijnpicks voor verzending, zoals beschreven in dit onderwerp.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-113">Picking for warehouse shipment of items that are assembled to the sales order being shipped follows the same steps as for regular warehouse picks for shipment, as described in this topic.</span></span> <span data-ttu-id="0f3c2-114">Het aantal pickregels per te verzenden aantal is mogelijk echter veel-op-één omdat u de componenten pickt, niet het assemblageartikel.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-114">However, the number of pick lines per quantity to ship may be many to one because you pick the components, not the assembly item.</span></span>  
>   
>  <span data-ttu-id="0f3c2-115">De magazijnpickregels zijn gemaakt voor de waarde in het veld **Resterend aantal** op de regels van de assemblage die is gekoppeld aan de verkooporderregel die wordt verzonden.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-115">The warehouse pick lines are created for the value in the **Remaining Quantity** field on the lines of the assembly order that is linked to the sales order line that is being shipped.</span></span> <span data-ttu-id="0f3c2-116">Dit zorgt ervoor dat alle onderdelen in één actie worden gepickt.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-116">This ensures that all components are picked in one action.</span></span>  
>   
>  <span data-ttu-id="0f3c2-117">Zie de sectie Op-order-assembleren-artikelen in magazijnverzendingen afhandelen in Magazijnverzending voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-117">For more information, see “Handling Assemble-to-Order Items in Warehouse Shipments” in Warehouse Shipment.</span></span>  
>   
>  <span data-ttu-id="0f3c2-118">Zie [Picken voor assemblage of productie in geavanceerde magazijnconfiguraties](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md) voor informatie over het picken van onderdelen voor assemblageorders in het algemeen, met inbegrip van situaties waar de assemblage niet voor een verkoopverzending is.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-118">For information about picking components for assembly orders generally, including situations where the assembly item is not due on a sales shipment, see [Pick for Assembly or Production in Advanced Warehouse Configurations](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md).</span></span>  

## <a name="to-plan-picks-in-the-worksheet"></a><span data-ttu-id="0f3c2-119">U kunt als volgt picks plannen in het voorstel</span><span class="sxs-lookup"><span data-stu-id="0f3c2-119">To plan picks in the worksheet</span></span>  
1.  <span data-ttu-id="0f3c2-120">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Pickvoorstel** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-120">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Pick Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="0f3c2-121">Kies de actie **Magazijndocumenten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-121">Choose the **Get Whse. Documents** action.</span></span>  
3.  <span data-ttu-id="0f3c2-122">Selecteer de verzendingen waarvoor u een pick wilt voorbereiden.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-122">Select the shipments for which you want to prepare a pick.</span></span> <span data-ttu-id="0f3c2-123">Hoewel u de regels nog in beperkte mate kunt sorteren, zal de sortering niet meer worden overgenomen op de pickinstructie.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-123">You can now sort the lines to some degree, but the sorting you do here will not be carried through to the pick instruction.</span></span> <span data-ttu-id="0f3c2-124">U kunt ook bepaalde regels verwijderen om een nog efficiëntere pick te maken.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-124">You can also delete some of the lines to make a more effective pick.</span></span> <span data-ttu-id="0f3c2-125">Als er bijvoorbeeld regels zijn met artikelen die in cross-docklocaties zijn geplaatst, kunt u een pick maken voor alle regels die verbonden zijn aan deze regels.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-125">For instance, if there are a number of lines with items in cross-dock bins, you might want to create a pick for all the lines associated with these lines.</span></span> <span data-ttu-id="0f3c2-126">De cross-dockartikelen worden dan verzonden, samen met de andere artikelen in de verzending, en in de cross-docklocaties komt ruimte vrij voor andere binnenkomende artikelen.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-126">The cross-docked items will be shipped, along with the other items on the shipments, and the cross-dock bins will have space for more incoming items.</span></span>  
4.  <span data-ttu-id="0f3c2-127">Kies de actie **Pick maken** en vul het aanvraagvenster **Pick maken** in.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-127">Choose the **Create Pick** action, and fill in the **Create Pick** request window.</span></span> <span data-ttu-id="0f3c2-128">De nieuwe pickregels worden gesorteerd volgens de methode die u hier kiest.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-128">The sorting you request here will order the pick lines you create.</span></span> <span data-ttu-id="0f3c2-129">Stel dat u voor elke zone één pick maakt, dan kunt u de regels binnen elke pick sorteren op rangorde van opslaglocatie.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-129">For example, you can create one pick for each zone and sort the lines by bin ranking within each pick.</span></span>  
5.  <span data-ttu-id="0f3c2-130">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Magazijnpicks** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-130">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Picks**, and then choose the related link.</span></span> <span data-ttu-id="0f3c2-131">Het venster **Picks** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-131">The **Picks** window opens.</span></span>  
6.  <span data-ttu-id="0f3c2-132">U kunt de pickopdracht die u hebt gemaakt nu opzoeken door op Pick, Overzicht te klikken en de pick met het hoogste nummer te selecteren.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-132">You can now find the pick assignment you just created by selecting the pick with the highest number.</span></span>  
7.  <span data-ttu-id="0f3c2-133">U kunt indien nodig de toegewezen gebruikers-id en sortering van de regels van de pick nog wijzigen.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-133">In the pick, you can still alter, if necessary, the assigned user ID and the way the lines are sorted.</span></span>  
8.  <span data-ttu-id="0f3c2-134">Kies de actie **Afdrukken** om de pickinstructies af te drukken.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-134">Choose the **Print** action to print the pick instructions.</span></span>  
9. <span data-ttu-id="0f3c2-135">Als u de pick hebt uitgevoerd, kiest u de actie **Registreren**.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-135">After you have performed the pick, choose the **Register** action.</span></span>  

<span data-ttu-id="0f3c2-136">Als de nummering van opslaglocaties een weerspiegeling vormt van de fysieke indeling van het magazijn en u hebt de regels gesorteerd op opslaglocatie, kan de picker in één rondgang door het magazijn artikelen voor verschillende verzendingen tegelijk picken.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-136">If the bins have been numbered in a way that mirrors the physical layout of the warehouse, the lines sorted by bin code allow the picker to pick for a number of shipments in one round of the warehouse.</span></span> <span data-ttu-id="0f3c2-137">De medewerker haalt uit elke opslaglocatie per verzendregel het vereiste aantal artikelen en plaatst deze bij de overige artikelen voor een bepaalde verzending.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-137">The worker takes the required number of items for each shipment line out of each bin and places them along with the other items for the particular shipment.</span></span> <span data-ttu-id="0f3c2-138">De picker kan zo veel tijd besparen omdat hij of zij slechts één keer naar de opslaglocatie hoeft te gaan om voor verschillende verzendingen te picken.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-138">A picker can save a great deal of time by picking for several shipments in one visit to a bin.</span></span>  

<span data-ttu-id="0f3c2-139">De rangorde van opslaglocaties is een andere effectieve sorteeroptie, zeker als het magazijn fysiek gezien meer op rangorde van opslaglocatie is ingedeeld dan op opslaglocatie.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-139">Another effective sorting option is bin ranking, if the physical layout of the warehouse is more according to bin ranking than bin code.</span></span>  

<span data-ttu-id="0f3c2-140">U kunt in het pickvoorstel ook op verzendadres sorteren, zodat u de orders voor verre klanten het eerst kunt samenstellen en verzenden.</span><span class="sxs-lookup"><span data-stu-id="0f3c2-140">In the pick worksheet, you can also sort by ship-to address, enabling you to assemble and ship the orders to far-away customers first.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0f3c2-141">Zie ook</span><span class="sxs-lookup"><span data-stu-id="0f3c2-141">See Also</span></span>
[<span data-ttu-id="0f3c2-142">Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="0f3c2-142">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="0f3c2-143">Voorraad</span><span class="sxs-lookup"><span data-stu-id="0f3c2-143">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="0f3c2-144">[Magazijnbeheer instellen](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="0f3c2-144">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="0f3c2-145">[Assemblagebeheer](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="0f3c2-145">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="0f3c2-146">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="0f3c2-146">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="0f3c2-147">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0f3c2-147">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
