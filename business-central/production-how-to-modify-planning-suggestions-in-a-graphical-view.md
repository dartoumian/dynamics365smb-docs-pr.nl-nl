---
title: Planningsuggesties in een grafische weergave wijzigen | Microsoft Docs
description: Een typische planningsactiviteit is het wijzigen of toevoegen van planningsvoorstelregels om de voorgestelde voorzieningsorders te wijzigen voordat u ze vastlegt door de functie **Planningsboodschap uitvoeren** uit te voeren. In plaats van dit in het planningsvoorstel te doen, kunt u ook een grafische weergave gebruiken.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f005baaeed8a3469258db5f2cde594291b384ba2
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="modify-planning-suggestions-in-a-graphical-view"></a><span data-ttu-id="c2d50-104">Planningsuggesties in een grafische weergave wijzigen</span><span class="sxs-lookup"><span data-stu-id="c2d50-104">Modify Planning Suggestions in a Graphical View</span></span>
<span data-ttu-id="c2d50-105">Een typische planningsactiviteit is het wijzigen of toevoegen van planningsvoorstelregels om de voorgestelde voorzieningsorders te wijzigen voordat u ze vastlegt door de functie **Planningsboodschap uitvoeren** uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="c2d50-105">A typical planning activity is to change or add planning worksheet lines to modify the suggested supply orders before you commit them by running the **Carry out Action Message** function.</span></span> <span data-ttu-id="c2d50-106">In plaats van dit in het planningsvoorstel te doen, kunt u ook een grafische weergave gebruiken.</span><span class="sxs-lookup"><span data-stu-id="c2d50-106">An alternative to doing this in the planning worksheet is to use a graphical view.</span></span>

<span data-ttu-id="c2d50-107">In het venster **Artikelbeschikbaarheid per tijdlijn** kunt u bepaalde aanvulorders en suggesties wijzigen door elementen langs de x-as te slepen om het aantal te wijzigen of langs de y-as te slepen om de vervaldatum te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-107">In the **Item Availability by Timeline** window, you can modify certain supply orders and suggestions by dragging elements on the x-axis to change quantity or dragging elements on the y-axis to change due date.</span></span>  

 <span data-ttu-id="c2d50-108">In het venster **Artikelbeschikbaarheid per tijdlijn** en het venster **Planningsvoorstel** kunt u de volgende wijzigingen aanbrengen:</span><span class="sxs-lookup"><span data-stu-id="c2d50-108">In the **Item Availability by Timeline** window and the **Planning Worksheet** window you can make the following changes:</span></span>  

-   <span data-ttu-id="c2d50-109">Een voorgestelde voorzieningsorder die alleen als een planningsregel bestaat wijzigen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-109">Modify a suggested supply order that only exists as a planning line.</span></span>  
-   <span data-ttu-id="c2d50-110">Een bestaande voorzieningsorder die het planningssysteem voorstelt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-110">Modify an existing supply order that the planning system suggests to change.</span></span>  
-   <span data-ttu-id="c2d50-111">Een nieuwe voorgestelde voorzieningsorder maken en wijzigen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-111">Create a new suggested supply order and modify it.</span></span>  

<span data-ttu-id="c2d50-112">Zie voor meer informatie over de typen planningsregels die worden weergegeven het veld Omschrijving op het sneltabblad **Gebeurteniswijzigingen**.</span><span class="sxs-lookup"><span data-stu-id="c2d50-112">For more information about the planning line types that are shown, see the Description field on the **Event Changes** FastTab.</span></span>  

<span data-ttu-id="c2d50-113">Wanneer u **Wijzigingen opslaan** kiest in het venster **Artikelbeschikbaarheid per tijdlijn**, worden de wijzigingen die u hebt aangebracht gekopieerd naar de planning of het inkoopvoorstel.</span><span class="sxs-lookup"><span data-stu-id="c2d50-113">When you choose **Save Changes** in the **Item Availability by Timeline** window, the modifications that you have made are copied to the planning or requisition worksheet.</span></span> <span data-ttu-id="c2d50-114">U kunt ze nu implementeren met de functie **Planningsboodschap uitvoeren - Plan**.</span><span class="sxs-lookup"><span data-stu-id="c2d50-114">You can now implement them using the **Carry Out Action Msg.-Plan.** function.</span></span>  

<span data-ttu-id="c2d50-115">De volgende procedure laat zien hoe u voorzieningsvoorstellen kunt wijzigen door slepen en neerzetten.</span><span class="sxs-lookup"><span data-stu-id="c2d50-115">The following procedure shows how to modify supply suggestions by drag and drop.</span></span> <span data-ttu-id="c2d50-116">Als alternatief kunt u de velden **Vervaldatum** en **Aantal** wijzigen op het sneltabblad **Event Changes** en de wijzigingen direct grafisch zien in het tabblad **Timeline** van het venster **Planningsvoorstel**.</span><span class="sxs-lookup"><span data-stu-id="c2d50-116">As an alternative, you can change the **Due Date** and **Quantity** fields on the **Event Changes** FastTab and immediately see the changes graphically on the **Timeline** FastTab in the **Planning Worksheet** window.</span></span>  

## <a name="to-modify-suggested-supply-orders-in-the-graphical-view"></a><span data-ttu-id="c2d50-117">Voorgestelde voorzieningsorders in de grafische weergave wijzigen</span><span class="sxs-lookup"><span data-stu-id="c2d50-117">To modify suggested supply orders in the graphical view</span></span>  
1.  <span data-ttu-id="c2d50-118">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelbeschikbaarheid per tijdlijn** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c2d50-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Availability by Timeline**, and then choose the related link.</span></span>  

    <span data-ttu-id="c2d50-119">Het venster **Artikelbeschikbaarheid per tijdlijn** wordt geopend met het artikelnummer, de vestiging en de variant van het artikel op de geselecteerde planningsregel vooraf ingevuld op de velden op het sneltabblad **Opties**.</span><span class="sxs-lookup"><span data-stu-id="c2d50-119">The **Item Availability by Timeline** window opens with the item number, location, and variant of the item on the selected planning line prefilled in the **Options** FastTab.</span></span> <span data-ttu-id="c2d50-120">Het sneltabblad **Tijdlijn** toont een grafische weergave van de verwachte voorraad van het artikel, inclusief planningsvoorstellen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-120">The **Timeline** FastTab shows a graphical representation of the item’s projected inventory, including planning suggestions.</span></span>  

2.  <span data-ttu-id="c2d50-121">Zorg ervoor dat het veld **Planningsvoorstellen opnemen** is geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-121">Make sure that the **Include Planning Suggestions** field is selected.</span></span>  
3.  <span data-ttu-id="c2d50-122">Zoek de voorgestelde voorzieningsorder die u wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-122">Find the suggested supply order that you want to modify.</span></span> <span data-ttu-id="c2d50-123">U kunt de aanpasbare elementen vinden door de groene cirkel en een pictogram van de schijf.</span><span class="sxs-lookup"><span data-stu-id="c2d50-123">You can identify modifiable elements by the green circle and the disk icon.</span></span> <span data-ttu-id="c2d50-124">Zie voor meer informatie over de verschillende symbolen de sectie Symbolen en pictogrammen op het sneltabblad Tijdlijn.</span><span class="sxs-lookup"><span data-stu-id="c2d50-124">For more information about the different symbols, see the "Symbols and Icons on the Timeline FastTab" section.</span></span>  
4.  <span data-ttu-id="c2d50-125">Plaats de aanwijzer op de groene cirkel totdat deze vergroot en de aanwijzer verandert in het Verplaatsen-symbool (vier pijltjes).</span><span class="sxs-lookup"><span data-stu-id="c2d50-125">Place the pointer over the green circle until it enlarges and the pointer changes to Move shape (four arrows).</span></span>  
5.  <span data-ttu-id="c2d50-126">Houd de muisknop ingedrukt terwijl u de aanwijzer omhoog of omlaag sleept om het aantal aan te passen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-126">Press and hold the mouse button while you drag the pointer up or down to modify the quantity.</span></span> <span data-ttu-id="c2d50-127">Houd de muisknop ingedrukt terwijl u de aanwijzer naar links of rechts sleept om de vervaldatum aan te passen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-127">Press and hold the mouse button while you drag the pointer left or right to modify the due date.</span></span>  
6.  <span data-ttu-id="c2d50-128">Naast het verplaatsen van elementen door slepen en neerzetten, kunt u planningsvoorstellen aanpassen door een aantal functies in het vervolgkeuzemenu te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="c2d50-128">In addition to moving elements by drag and drop, you can modify planning suggestions by using a number of drop-down menu functions.</span></span> <span data-ttu-id="c2d50-129">Open het vervolgkeuzemenu voor de groene cirkel van een voorgesteld voorzieningselement en selecteer een van de volgende functies</span><span class="sxs-lookup"><span data-stu-id="c2d50-129">Access the drop-down menu for the green circle of a suggested supply element and select one the following functions</span></span>  

    |<span data-ttu-id="c2d50-130">Functie</span><span class="sxs-lookup"><span data-stu-id="c2d50-130">Function</span></span>|<span data-ttu-id="c2d50-131">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="c2d50-131">Description</span></span>|  
    |--------------|---------------------------------------|  
    |<span data-ttu-id="c2d50-132">**Nieuwe voorraad maken**</span><span class="sxs-lookup"><span data-stu-id="c2d50-132">**Create New Supply**</span></span>|<span data-ttu-id="c2d50-133">Hiermee wordt een nieuw element gemaakt op het punt waar u het vervolgkeuzemenu opent. Dit vertegenwoordigt een nieuwe voorgestelde aanvulorder.</span><span class="sxs-lookup"><span data-stu-id="c2d50-133">Creates a new element point where you access the drop-down menu, which represents a new suggested supply order.</span></span> <span data-ttu-id="c2d50-134">Het wordt een nieuwe regel in het planningsvoorstel wanneer u **Wijzigingen opslaan** kiest.</span><span class="sxs-lookup"><span data-stu-id="c2d50-134">It becomes a new line in the planning worksheet when you choose **Save Changes**.</span></span><br /><br /> <span data-ttu-id="c2d50-135">**OPMERKING:** als het veld **Vestigingsfilter** of **Variantfilter** op het tabblad **Options** leeg is of meer dan één filterwaarde bevat, wordt de nieuwe voorziening gemaakt en later opgeslagen naar het plannings- of inkoopvoorstel met de volgende codes:</span><span class="sxs-lookup"><span data-stu-id="c2d50-135">**NOTE:** If the **Location Filter** or **Variant Filter** fields on the **Options** FastTab are empty or have more than one filter value, then the new supply is created and later saved to the planning or requisition worksheet with the following codes:</span></span><br /><br /> <span data-ttu-id="c2d50-136">\* Als het filterveld leeg is, wordt de nieuwe voorziening gemaakt zonder een vestigings- of variantcode.</span><span class="sxs-lookup"><span data-stu-id="c2d50-136">\* If the filter field is empty, then the new supply is created without a location or variant code.</span></span><br /><br /> <span data-ttu-id="c2d50-137">\* Als er meer dan één filterwaarde is gedefinieerd, wordt de nieuwe voorziening gemaakt voor de eerste filterwaarde volgens de sorteermethode.</span><span class="sxs-lookup"><span data-stu-id="c2d50-137">\* If more than one filter value is defined, then the new supply is created for the first filter value according to the sorting method.</span></span><br /><br /> <span data-ttu-id="c2d50-138">Als u een andere variant- of vestigingscode wilt, moet u dat handmatig wijzigen op de nieuwe planningsregel.</span><span class="sxs-lookup"><span data-stu-id="c2d50-138">If you want another variant or location code, then you must manually change it on the new planning line.</span></span>|  
    |<span data-ttu-id="c2d50-139">**Voorziening automatisch aanpassen**</span><span class="sxs-lookup"><span data-stu-id="c2d50-139">**Auto-Adjust Supply**</span></span>|<span data-ttu-id="c2d50-140">Optimaliseert een nieuwe voorziening die u in de grafiek hebt gemaakt door ervoor te zorgen dat deze resulteert in nul-voorraad voor de volgende voorziening.</span><span class="sxs-lookup"><span data-stu-id="c2d50-140">Optimizes a new supply that you have created in the graph by making sure that it results in zero inventory before the next supply.</span></span>|  
    |<span data-ttu-id="c2d50-141">**Voorziening verwijderen**</span><span class="sxs-lookup"><span data-stu-id="c2d50-141">**Delete Supply**</span></span>|<span data-ttu-id="c2d50-142">Hiermee verwijdert u het element in het sneltabblad **Tijdlijn** en verwijdert u de planningsregel wanneer u **Wijzigingen opslaan** kiest.</span><span class="sxs-lookup"><span data-stu-id="c2d50-142">Deletes the element in the **Timeline** FastTab and deletes the planning line when you choose **Save Changes**.</span></span> <span data-ttu-id="c2d50-143">Het pictogram verandert in een schijf met een rood kruis wanneer de voorziening is verwijderd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-143">The icon changes to a disk that has a red cross when the supply has been deleted.</span></span><br /><br /> <span data-ttu-id="c2d50-144">**OPMERKING:** u kunt alleen een voorziening van het type planningsboodschap **Nieuw** verwijderen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-144">**NOTE:** You can only delete a supply of action message type **New**.</span></span> <span data-ttu-id="c2d50-145">Nadat u **Wijzigingen opslaan** kiest, moet u handmatig de betreffende planningsregel verwijderen in het plannings- of inkoopvoorstel.</span><span class="sxs-lookup"><span data-stu-id="c2d50-145">After you choose **Save Changes**, you must manually delete the planning line in question in the planning or requisition worksheet.</span></span>|  

7.  <span data-ttu-id="c2d50-146">Kies de actie **Opnieuw laden** als u alle wijzigingen wilt terugdraaien die u hebt aangebracht nadat u het venster **Artikelbeschikbaarheid per tijdlijn** voor het laatst hebt geopend of **Opnieuw laden** hebt geselecteerd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-146">Choose the **Reload** action if you want to reset all the changes that you have made after you last opened the **Item Availability by Timeline** window or selected **Reload**.</span></span>  
8. <span data-ttu-id="c2d50-147">Wanneer de elementen zijn geplaatst waar u ze wilt in het schema, klikt u op **Wijzigingen opslaan** om het aangepaste aantal en de datumwijzigingen te kopiëren naar de plannings- of inkoopregels die de grafische elementen weergeven.</span><span class="sxs-lookup"><span data-stu-id="c2d50-147">When the elements are placed where you want them in the diagram, choose **Save Changes** to copy modified quantity and date changes to the planning or requisition lines that represent the graphical elements.</span></span>  

<span data-ttu-id="c2d50-148">Om de wijzigingen in het voorzieningsplan te implementeren, moet u de resulterende planningsboodschappen van het plannings- of inkoopvoorstel opvolgen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-148">To implement the supply plan changes, you must follow the resulting action messages from the planning or requisition worksheet.</span></span> <span data-ttu-id="c2d50-149">Zie voor meer informatie Planningsboodschap uitvoeren - Plan.</span><span class="sxs-lookup"><span data-stu-id="c2d50-149">For more information, see Carry Out Action Msg.-Plan..</span></span>

## <a name="symbols-and-icons-on-the-timeline-fasttab"></a><span data-ttu-id="c2d50-150">Symbolen en pictogrammen op het sneltabblad Tijdlijn</span><span class="sxs-lookup"><span data-stu-id="c2d50-150">Symbols and Icons on the Timeline FastTab</span></span>
 |<span data-ttu-id="c2d50-151">Symbool/pictogram</span><span class="sxs-lookup"><span data-stu-id="c2d50-151">Symbol/Icon</span></span>|<span data-ttu-id="c2d50-152">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="c2d50-152">Description</span></span>|  
 |------------------|---------------------------------------|  
 |<span data-ttu-id="c2d50-153">Zwart kruis</span><span class="sxs-lookup"><span data-stu-id="c2d50-153">Black cross</span></span>|<span data-ttu-id="c2d50-154">Orders (zowel vraag als aanbod).</span><span class="sxs-lookup"><span data-stu-id="c2d50-154">Orders (both supply and demand).</span></span><br /><br /> <span data-ttu-id="c2d50-155">-   Kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-155">-   Cannot be modified.</span></span><br /><span data-ttu-id="c2d50-156">-   Zichtbaar wanneer het veld **Geplande voorraad weergeven** is geselecteerd (oranje grafiek).</span><span class="sxs-lookup"><span data-stu-id="c2d50-156">-   Visible when the **Show Projected Inventory** field is selected (orange graph).</span></span>|  
 |<span data-ttu-id="c2d50-157">Rode cirkel</span><span class="sxs-lookup"><span data-stu-id="c2d50-157">Red circle</span></span>|<span data-ttu-id="c2d50-158">Bestaande voorzieningsorders die geen deel uitmaken van planningsvoorstellen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-158">Existing supply orders that are not in planning suggestions.</span></span><br /><br /> <span data-ttu-id="c2d50-159">-   Kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-159">-   Cannot be modified.</span></span><br /><span data-ttu-id="c2d50-160">-   Zichtbaar wanneer het veld **Geplande voorraad weergeven** is geselecteerd (oranje grafiek).</span><span class="sxs-lookup"><span data-stu-id="c2d50-160">-   Visible when the **Show Projected Inventory** field is selected (orange graph).</span></span>|  
 |<span data-ttu-id="c2d50-161">Gele ster</span><span class="sxs-lookup"><span data-stu-id="c2d50-161">Yellow star</span></span>|<span data-ttu-id="c2d50-162">Vraag voorspellen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-162">Forecast demand.</span></span><br /><br /> <span data-ttu-id="c2d50-163">-   Kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-163">-   Cannot be modified.</span></span><br /><span data-ttu-id="c2d50-164">-   Zichtbaar wanneer het veld **Prognosenaam** een waarde bevat.</span><span class="sxs-lookup"><span data-stu-id="c2d50-164">-   Visible when the **Forecast Name** field has a value.</span></span><br /><br /> <span data-ttu-id="c2d50-165">Wanneer zowel het veld **Geplande voorraad weergeven** als het veld **Planningsuggesties opnemen** is geselecteerd, heeft elke gele ster een gekoppelde tegenhanger in de tegenovergestelde grafiek.</span><span class="sxs-lookup"><span data-stu-id="c2d50-165">When both the **Show Projected Inventory** and the **Include Planning Suggestions** fields are selected, then each yellow star has a linked counterpart in the opposite graph.</span></span> <span data-ttu-id="c2d50-166">Dit illustreert hoe een voorgesteld aanbod voldoet aan de geprognosticeerde vraag.</span><span class="sxs-lookup"><span data-stu-id="c2d50-166">This illustrates how a suggested supply fulfills the forecasted demand.</span></span>|  
 |<span data-ttu-id="c2d50-167">Groene cirkel met een pictogram in de vorm van een schijf met een rood kruis</span><span class="sxs-lookup"><span data-stu-id="c2d50-167">Green circle with an icon shaped as a disk that has a red cross</span></span>|<span data-ttu-id="c2d50-168">Voorgestelde voorzieningsorder met planningsboodschap *Annuleren*.</span><span class="sxs-lookup"><span data-stu-id="c2d50-168">Suggested supply order with action message *Cancel*.</span></span><br /><br /> <span data-ttu-id="c2d50-169">-   Kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-169">-   Cannot be modified.</span></span><br /><span data-ttu-id="c2d50-170">-   Zichtbaar wanneer het veld **Planningsuggesties opnemen** is geselecteerd (groene grafiek).</span><span class="sxs-lookup"><span data-stu-id="c2d50-170">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span></span>|  
 |<span data-ttu-id="c2d50-171">Groene cirkel met een pictogram in de vorm van een schijf met een ster</span><span class="sxs-lookup"><span data-stu-id="c2d50-171">Green circle with an icon shaped as a disk that has a star</span></span>|<span data-ttu-id="c2d50-172">Voorgestelde voorzieningsorders met planningsboodschap *Nieuw*.</span><span class="sxs-lookup"><span data-stu-id="c2d50-172">Suggested supply orders with action message *New*.</span></span><br /><br /> <span data-ttu-id="c2d50-173">-   Kan worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-173">-   Can be modified.</span></span><br /><span data-ttu-id="c2d50-174">-   Zichtbaar wanneer het veld **Planningsuggesties opnemen** is geselecteerd (groene grafiek).</span><span class="sxs-lookup"><span data-stu-id="c2d50-174">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span></span>|  
 |<span data-ttu-id="c2d50-175">Groene cirkel met een pictogram in de vorm van een schijf met een of twee pijlen</span><span class="sxs-lookup"><span data-stu-id="c2d50-175">Green circle with an icon shaped as a disk that has one or two arrows</span></span>|<span data-ttu-id="c2d50-176">Voorgestelde voorzieningenorders met planningsboodschap *Herplannen*, *Aantal wijzigingen* of *Herplannen en aantal wijzigingen*</span><span class="sxs-lookup"><span data-stu-id="c2d50-176">Suggested supply orders with action message *Reschedule*, *Change Qty.*, or *Resched. and Chg. Qty.*</span></span><br /><br /> <span data-ttu-id="c2d50-177">-   Kan worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-177">-   Can be modified.</span></span><br /><span data-ttu-id="c2d50-178">-   Zichtbaar wanneer het veld **Planningsuggesties opnemen** is geselecteerd (groene grafiek).</span><span class="sxs-lookup"><span data-stu-id="c2d50-178">-   Visible when the **Include Planning Suggestions** field is selected (green graph).</span></span><br /><br /> <span data-ttu-id="c2d50-179">De pijlen geven de richting van de planningsuggestie aan.</span><span class="sxs-lookup"><span data-stu-id="c2d50-179">The arrows reflect the direction of the planning suggestion.</span></span> <span data-ttu-id="c2d50-180">Bijvoorbeeld een pijl-links samen met een pijl-omhoog geeft een planningsboodschap *Herplannen en Aantal wijzigen* aan die uit een achterwaartse herplanning en een toename van het aantal bestaat.</span><span class="sxs-lookup"><span data-stu-id="c2d50-180">For example, a left arrow together with an up arrow reflects a *Resched. and Chg. Qty.* action message that consists of a backward rescheduling and a quantity increase.</span></span>|  

<span data-ttu-id="c2d50-181">Wanneer u het vervolgkeuzemenu voor het sneltabblad **Tijdlijn** opent, worden de volgende functies weergegeven, afhankelijk van wat u kiest</span><span class="sxs-lookup"><span data-stu-id="c2d50-181">When you access the drop-down menu for the **Timeline** FastTab, the following functions appear depending what you choose</span></span>  

 |<span data-ttu-id="c2d50-182">Functie</span><span class="sxs-lookup"><span data-stu-id="c2d50-182">Function</span></span>|<span data-ttu-id="c2d50-183">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="c2d50-183">Description</span></span>|  
 |--------------|---------------------------------------|  
 |<span data-ttu-id="c2d50-184">**Nieuwe voorraad maken**</span><span class="sxs-lookup"><span data-stu-id="c2d50-184">**Create New Supply**</span></span>|<span data-ttu-id="c2d50-185">Hiermee wordt een nieuw element gemaakt op het punt waar u het vervolgkeuzemenu opent. Dit vertegenwoordigt een nieuwe voorgestelde aanvulorder.</span><span class="sxs-lookup"><span data-stu-id="c2d50-185">Creates a new element on the point where you access the drop-down menu, which represents a new suggested supply order.</span></span> <span data-ttu-id="c2d50-186">Het wordt een nieuwe regel in het planningsvoorstel wanneer u **Wijzigingen opslaan** kiest op het tabblad **Verwerken**.</span><span class="sxs-lookup"><span data-stu-id="c2d50-186">It becomes a new line in the planning worksheet when you choose **Save Changes** on the **Process** tab.</span></span><br /><br /> <span data-ttu-id="c2d50-187">Filterwaarden die worden gedefinieerd in het veld **Vestigingsfilter** of **Variantfilter** op het sneltabblad **Opties**, worden toegepast op de nieuwe voorzieningenorder.</span><span class="sxs-lookup"><span data-stu-id="c2d50-187">Any filter values that are defined in the **Location Filter** or **Variant Filter** fields on the **Options** FastTab will be applied to the new supply order.</span></span> <span data-ttu-id="c2d50-188">**Opmerking:** als de filtervelden leeg zijn of meer dan één filterwaarde bevatten, wordt de nieuwe voorzieningsorder gemaakt met behulp van de volgende codes:</span><span class="sxs-lookup"><span data-stu-id="c2d50-188">**Note:**  If the filter fields are empty or have more than one filter value, then the new supply order is created by using the following codes:</span></span> <ul><li><span data-ttu-id="c2d50-189">Als het filterveld leeg is, wordt de nieuwe voorziening gemaakt zonder een vestigings- of variantcode.</span><span class="sxs-lookup"><span data-stu-id="c2d50-189">If the filter field is empty, then the new supply is created without a location or variant code.</span></span></li><li><span data-ttu-id="c2d50-190">Als er meer dan één filterwaarde is gedefinieerd, wordt de nieuwe voorziening gemaakt met behulp van de eerste filterwaarde op basis van de sorteervolgorde.</span><span class="sxs-lookup"><span data-stu-id="c2d50-190">If more than one filter value is defined, then the new supply is created by using the first filter value according to the sorting order.</span></span></li></ul> <span data-ttu-id="c2d50-191">Als u een andere variant- of vestigingscode wilt in de nieuwe voorzieningsorder, moet u deze handmatig wijzigen op de nieuwe planningsregel.</span><span class="sxs-lookup"><span data-stu-id="c2d50-191">If you want another variant or location code in the new supply order, then you must manually change it on the new planning line.</span></span>|  
 |<span data-ttu-id="c2d50-192">**Voorziening automatisch aanpassen**</span><span class="sxs-lookup"><span data-stu-id="c2d50-192">**Auto-Adjust Supply**</span></span>|<span data-ttu-id="c2d50-193">Hiermee wordt een nieuwe voorziening geoptimaliseerd die u in de grafiek hebt gemaakt door ervoor te zorgen dat er een nul-voorraad ontstaat vóór de volgende voorziening.</span><span class="sxs-lookup"><span data-stu-id="c2d50-193">Optimizes a new supply that you have created in the graph by making sure that it creates zero inventory before the next supply.</span></span>|  
 |<span data-ttu-id="c2d50-194">**Voorziening verwijderen**</span><span class="sxs-lookup"><span data-stu-id="c2d50-194">**Delete Supply**</span></span>|<span data-ttu-id="c2d50-195">Hiermee verwijdert u het element op het sneltabblad **Tijdlijn** en verwijdert u de planningsregel wanneer u **Wijzigingen opslaan** kiest op het tabblad **Verwerken**. Het pictogram verandert in een schijf met een rood kruis nadat de voorziening is verwijderd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-195">Deletes the element in the **Timeline** FastTab and deletes the planning line when you choose **Save Changes** on the **Process** tab. The icon changes to a disk that has a red cross when the supply has been deleted.</span></span> <span data-ttu-id="c2d50-196">**Opmerking:** u kunt alleen een voorziening van het type planningsboodschap *Nieuw* verwijderen.</span><span class="sxs-lookup"><span data-stu-id="c2d50-196">**Note:**  You can only delete a supply of action message type *New*.</span></span> <span data-ttu-id="c2d50-197">Nadat u **Wijzigingen opslaan** hebt gekozen op het tabblad **Verwerken**, moet u handmatig de desbetreffende planningsregel verwijderen in het plannings- of inkoopvoorstel.</span><span class="sxs-lookup"><span data-stu-id="c2d50-197">After you choose **Save Changes** on the **Process** tab, you must manually delete the planning line in question in the planning or requisition worksheet.</span></span>|  
 |<span data-ttu-id="c2d50-198">**Document weergeven**</span><span class="sxs-lookup"><span data-stu-id="c2d50-198">**Show Document**</span></span>|<span data-ttu-id="c2d50-199">Hiermee wordt de order, planningsregel of prognose geopend die het element vertegenwoordigt.</span><span class="sxs-lookup"><span data-stu-id="c2d50-199">Opens the order, planning line, or forecast that the element represents.</span></span>|  
 |<span data-ttu-id="c2d50-200">**Uitzoomen (Ctrl++)**</span><span class="sxs-lookup"><span data-stu-id="c2d50-200">**Zoom Out (Ctrl++)**</span></span>|<span data-ttu-id="c2d50-201">Hiermee wordt de schaal van de x-as groter gemaakt, zodat er minder dagen worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="c2d50-201">Makes the scale of the x-axis larger, so that fewer days are shown.</span></span> <span data-ttu-id="c2d50-202">**Opmerking:** u kunt dit ook doen door op Ctrl + muiswiel te drukken.</span><span class="sxs-lookup"><span data-stu-id="c2d50-202">**Note:**  You can also do this by pressing Ctrl + scroll mouse wheel.</span></span>|  
 |<span data-ttu-id="c2d50-203">**Inzoomen (Ctrl+-)**</span><span class="sxs-lookup"><span data-stu-id="c2d50-203">**Zoom In (Ctrl+-)**</span></span>|<span data-ttu-id="c2d50-204">Hiermee wordt de schaal van de x-as kleiner gemaakt, zodat er meer dagen worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="c2d50-204">Makes the scale of the x-axis smaller, so that more days are shown.</span></span> <span data-ttu-id="c2d50-205">**Opmerking:** u kunt dit ook doen door op Ctrl + muiswiel te drukken.</span><span class="sxs-lookup"><span data-stu-id="c2d50-205">**Note:**  You can also do this by pressing Ctrl + scroll mouse wheel.</span></span>|  
 |<span data-ttu-id="c2d50-206">**Zoom opnieuw instellen (Ctrl+0)**</span><span class="sxs-lookup"><span data-stu-id="c2d50-206">**Reset Zoom (Ctrl+0)**</span></span>|<span data-ttu-id="c2d50-207">Hiermee wordt de schaal van de x-as teruggezet op wat werd gebruikt voordat u inzoomde.</span><span class="sxs-lookup"><span data-stu-id="c2d50-207">Reverts the scale of the x-axis to what was used before you zoomed.</span></span>|  

<span data-ttu-id="c2d50-208">Behalve de toetsenbordacties die eerder werden vermeld, kunt u ook de volgende toetsenbordacties gebruiken op het sneltabblad **Tijdlijn**.</span><span class="sxs-lookup"><span data-stu-id="c2d50-208">In addition to the keyboard actions that were mentioned earlier, you can also use the following keyboard actions in the **TimeLine** FastTab.</span></span>  

 |<span data-ttu-id="c2d50-209">Toetsenbordactie</span><span class="sxs-lookup"><span data-stu-id="c2d50-209">Keyboard Action</span></span>|<span data-ttu-id="c2d50-210">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="c2d50-210">Description</span></span>|  
 |---------------------|---------------------------------------|  
 |<span data-ttu-id="c2d50-211">Ctrl + muiswiel</span><span class="sxs-lookup"><span data-stu-id="c2d50-211">Ctrl + scroll mouse wheel</span></span>|<span data-ttu-id="c2d50-212">Hiermee wordt de schaal van de x-as gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c2d50-212">Changes the scale of the x-axis.</span></span>|  
 |<span data-ttu-id="c2d50-213">Selecteer een element en druk vervolgens op Shift + pijl</span><span class="sxs-lookup"><span data-stu-id="c2d50-213">Select an element, then press Shift+Arrow</span></span>|<span data-ttu-id="c2d50-214">Hiermee wordt het element verplaatst in de richting waarnaar de pijl wijst.</span><span class="sxs-lookup"><span data-stu-id="c2d50-214">Moves the element in the direction of the arrow stroke.</span></span>|  
 |<span data-ttu-id="c2d50-215">Tab</span><span class="sxs-lookup"><span data-stu-id="c2d50-215">Tab</span></span>|<span data-ttu-id="c2d50-216">Hiermee gaat u naar het volgende element.</span><span class="sxs-lookup"><span data-stu-id="c2d50-216">Moves to the next element.</span></span>|  
 |<span data-ttu-id="c2d50-217">Shift + tab</span><span class="sxs-lookup"><span data-stu-id="c2d50-217">Shift+Tab</span></span>|<span data-ttu-id="c2d50-218">Hiermee gaat u naar het vorige element.</span><span class="sxs-lookup"><span data-stu-id="c2d50-218">Moves to the previous element.</span></span>|  
 |<span data-ttu-id="c2d50-219">Druk op Esc terwijl u een element verplaatst.</span><span class="sxs-lookup"><span data-stu-id="c2d50-219">While moving an element, press Esc.</span></span>|<span data-ttu-id="c2d50-220">Hiermee annuleert u de verplaatsing.</span><span class="sxs-lookup"><span data-stu-id="c2d50-220">Cancels the move.</span></span> <span data-ttu-id="c2d50-221">**Opmerking:** werkt niet als u de muisknop hebt losgelaten.</span><span class="sxs-lookup"><span data-stu-id="c2d50-221">**Note:**  Does not work if you have released the mouse button.</span></span>|

## <a name="see-also"></a><span data-ttu-id="c2d50-222">Zie ook</span><span class="sxs-lookup"><span data-stu-id="c2d50-222">See Also</span></span>  
<span data-ttu-id="c2d50-223">[Gepland](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="c2d50-223">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="c2d50-224">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="c2d50-224">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="c2d50-225">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="c2d50-225">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="c2d50-226">Voorraad</span><span class="sxs-lookup"><span data-stu-id="c2d50-226">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="c2d50-227">Inkoop</span><span class="sxs-lookup"><span data-stu-id="c2d50-227">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="c2d50-228">[Ontwerpdetails: Voorzieningsplanning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="c2d50-228">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="c2d50-229">Aanbevolen procedures instellen: voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="c2d50-229">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="c2d50-230">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c2d50-230">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
