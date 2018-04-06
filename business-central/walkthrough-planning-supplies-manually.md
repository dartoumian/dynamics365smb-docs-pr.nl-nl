---
title: 'Procedure: Leveringen handmatig plannen | Microsoft Docs'
description: In het volgende overzicht ziet u het proces voor het plannen van voorraadorders om aan nieuwe vraag te voldoen. U kunt voorraadplanning starten met vaste tussenpozen, bijvoorbeeld elke ochtend of elke maandag, of wanneer u bericht krijgt van verkoop of productie, afhankelijk van het type vraag.
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
ms.openlocfilehash: 2992c2a9cbd2142e69cfb59294791ec31ce4dcb1
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="walkthrough-planning-supplies-manually"></a><span data-ttu-id="9b626-104">Procedure: Leveringen handmatig plannen</span><span class="sxs-lookup"><span data-stu-id="9b626-104">Walkthrough: Planning Supplies Manually</span></span>
<span data-ttu-id="9b626-105">In het volgende overzicht ziet u het proces voor het plannen van voorraadorders om aan nieuwe vraag te voldoen.</span><span class="sxs-lookup"><span data-stu-id="9b626-105">This walkthrough demonstrates the process of planning supply orders to fulfill new demand.</span></span> <span data-ttu-id="9b626-106">U kunt voorraadplanning starten met vaste tussenpozen, bijvoorbeeld elke ochtend of elke maandag, of wanneer u bericht krijgt van verkoop of productie, afhankelijk van het type vraag.</span><span class="sxs-lookup"><span data-stu-id="9b626-106">You can initiate supply planning at fixed intervals, for example, every morning or every Monday, or when you are notified by sales or production, depending on the type of demand.</span></span> <span data-ttu-id="9b626-107">In dit scenario gebruikt u het venster **Orderplanning**, een eenvoudig voorraadplanningshulpmiddel op basis van handmatige besluitvorming in plaats van automatische planning op basis van parameters.</span><span class="sxs-lookup"><span data-stu-id="9b626-107">In this walkthrough you will use the **Order Planning** window, a simple supply planning tool that is based on manual decision-making instead of parameter-based automatic planning.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="9b626-108">Informatie over deze procedure</span><span class="sxs-lookup"><span data-stu-id="9b626-108">About This Walkthrough</span></span>  
 <span data-ttu-id="9b626-109">In deze procedure worden de volgende taken beschreven:</span><span class="sxs-lookup"><span data-stu-id="9b626-109">This walkthrough illustrates the following tasks:</span></span>  

-   <span data-ttu-id="9b626-110">Een inkooporder plannen voor het fabriceren van onderdelen.</span><span class="sxs-lookup"><span data-stu-id="9b626-110">Planning a purchase order for manufacturing components.</span></span>  
-   <span data-ttu-id="9b626-111">Een transferorder plannen om aan de verkoopvraag te voldoen.</span><span class="sxs-lookup"><span data-stu-id="9b626-111">Planning a transfer order to fulfill sales demand.</span></span>  
-   <span data-ttu-id="9b626-112">Een productieorder plannen voor een artikel met meerdere niveaus.</span><span class="sxs-lookup"><span data-stu-id="9b626-112">Planning a production order for a multilevel item.</span></span>  

## <a name="roles"></a><span data-ttu-id="9b626-113">Rollen</span><span class="sxs-lookup"><span data-stu-id="9b626-113">Roles</span></span>  
 <span data-ttu-id="9b626-114">In deze procedure worden taken gedemonstreerd voor de volgende gebruikersrollen:</span><span class="sxs-lookup"><span data-stu-id="9b626-114">This walkthrough demonstrates tasks performed by the following user roles:</span></span>  

-   <span data-ttu-id="9b626-115">Productieplanner</span><span class="sxs-lookup"><span data-stu-id="9b626-115">Production Planner</span></span>  
-   <span data-ttu-id="9b626-116">Inkoper</span><span class="sxs-lookup"><span data-stu-id="9b626-116">Purchasing Agent</span></span>  
-   <span data-ttu-id="9b626-117">Verkooporderverwerker</span><span class="sxs-lookup"><span data-stu-id="9b626-117">Sales Order Processor</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="9b626-118">Vereisten</span><span class="sxs-lookup"><span data-stu-id="9b626-118">Prerequisites</span></span>  
 <span data-ttu-id="9b626-119">Voordat u met dit scenario begint, moet u de [!INCLUDE[d365fin](includes/d365fin_md.md)] installeren.</span><span class="sxs-lookup"><span data-stu-id="9b626-119">Before you begin this walkthrough, you must install the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="9b626-120">Breng de volgende wijzigingen aan in de database:</span><span class="sxs-lookup"><span data-stu-id="9b626-120">The following modifications must be made to the database:</span></span>  

-   <span data-ttu-id="9b626-121">Verwijder alle bestaande verkooporders voor fietsen.</span><span class="sxs-lookup"><span data-stu-id="9b626-121">Delete all existing sales orders for bicycles.</span></span>  
-   <span data-ttu-id="9b626-122">Maak één verkooporder voor 10 fietsen op de locatie BLAUW.</span><span class="sxs-lookup"><span data-stu-id="9b626-122">Create one sales order for 10 bicycles at BLUE location.</span></span>  
-   <span data-ttu-id="9b626-123">Verwijder alle geplande en vast geplande productieorders.</span><span class="sxs-lookup"><span data-stu-id="9b626-123">Delete all planned and firm planned production orders.</span></span> <span data-ttu-id="9b626-124">Verwijder geen gestarte orders met posten die al zijn geboekt.</span><span class="sxs-lookup"><span data-stu-id="9b626-124">Do not delete started orders with entries that are already posted.</span></span>  

 <span data-ttu-id="9b626-125">Gebruik als algemene regel de voorgestelde gegevens uit deze procedure aangezien deze gegevens de benodigde records bevatten.</span><span class="sxs-lookup"><span data-stu-id="9b626-125">As a rule, use the suggested data in this walkthrough because this data has the necessary records.</span></span>  

## <a name="story"></a><span data-ttu-id="9b626-126">Scenario</span><span class="sxs-lookup"><span data-stu-id="9b626-126">Story</span></span>  
 <span data-ttu-id="9b626-127">Eduardo, de productieplanner van een klein productiebedrijf is bezig met het plannen van de productie en inkooporders om te voldoen aan de nieuwe verkoopvraag.</span><span class="sxs-lookup"><span data-stu-id="9b626-127">Eduardo, the Production Planner of a small manufacturing company, is about to plan production and purchase orders to fulfill new sales demand.</span></span>  

 <span data-ttu-id="9b626-128">Aangezien de producten uit slechts enkele stuklijstniveaus bestaan en de orderstroom tamelijk gering is, gebruikt Eduardo het venster **Orderplanning** om de orders voor voorzieningen handmatig te maken, met één productniveau tegelijk.</span><span class="sxs-lookup"><span data-stu-id="9b626-128">Because the products have few BOM levels and the flow of orders is relatively low, Eduardo uses the **Order Planning** window to manually create supply orders, one product level at a time.</span></span>  

 <span data-ttu-id="9b626-129">In een meer complexe productieomgeving wordt het planningsvoorstel gebruikt om de voorraad te plannen op basis van artikelparameters als herplanningsperiode, veiligheidstijd, bestelpunt en batchberekeningen van de geconsolideerde aanvraag van alle productniveaus.</span><span class="sxs-lookup"><span data-stu-id="9b626-129">In a more complex manufacturing environment, the planning worksheet is used to plan supply based on item parameters such as rescheduling period, safety lead time, reorder point, and batch calculations of consolidated demand from all product levels.</span></span>  

## <a name="setting-up-the-sample-data"></a><span data-ttu-id="9b626-130">Voorbeeldgegevens instellen</span><span class="sxs-lookup"><span data-stu-id="9b626-130">Setting Up the Sample Data</span></span>  
 <span data-ttu-id="9b626-131">In het standaarddemobedrijf CRONUS is momenteel sprake van een grote hoeveelheid niet-geplande vraag.</span><span class="sxs-lookup"><span data-stu-id="9b626-131">The standard CRONUS demonstration company currently has lots of unplanned demand.</span></span> <span data-ttu-id="9b626-132">Tijdens de verschillende planningstaken in deze procedure moet u afwijken van de realistische bedrijfswerkstroom door de vraag met vervaldatums in de nabije toekomst te negeren en in plaats daarvan de vraag te gebruiken met latere vervaldatums.</span><span class="sxs-lookup"><span data-stu-id="9b626-132">During the different planning tasks in this walkthrough, you will have to deviate from the realistic business flow by ignoring demand with close due dates and instead use demand with later due dates.</span></span>  

## <a name="using-the-order-planning-window"></a><span data-ttu-id="9b626-133">Het venster Orderplanning gebruiken</span><span class="sxs-lookup"><span data-stu-id="9b626-133">Using the Order Planning Window</span></span>  

<!-- 
The **Order Planning** window can be accessed from several different locations on the **Departments** menu in the navigation pane:  

-   Manufacturing, Planning  
-   Sales & Marketing, Order Processing  
-   Purchase, Planning  
-   In addition, you can open this window for a specific production order by choosing **Planning** on the **Navigate** tab in the **Order** group.

-->  

### <a name="to-use-the-order-planning-window"></a><span data-ttu-id="9b626-134">Het venster Orderplanning gebruiken</span><span class="sxs-lookup"><span data-stu-id="9b626-134">To use the Order Planning window</span></span>  

1.  <span data-ttu-id="9b626-135">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Orderplanning** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9b626-135">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Order Planning**, and then choose the related link.</span></span>  

     <span data-ttu-id="9b626-136">Als het venster **Orderplanning** voor het eerst wordt geopend, moet er een planning worden berekend om de nieuwe vraag weer te geven sinds deze voor het laatst is berekend.</span><span class="sxs-lookup"><span data-stu-id="9b626-136">When the **Order Planning** window first opens, a plan must be calculated to show the new demand since it was last calculated.</span></span>  

2.  <span data-ttu-id="9b626-137">Kies de actie **Plan berekenen**.</span><span class="sxs-lookup"><span data-stu-id="9b626-137">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="9b626-138">Het planningssysteem analyseert de nieuwe vraag die is geïntroduceerd, zoals nieuwe of gewijzigde verkoop- of productieorders.</span><span class="sxs-lookup"><span data-stu-id="9b626-138">The planning system analyzes any new demand that has been introduced, such as new sales, changed sales, or production orders.</span></span>  

     <span data-ttu-id="9b626-139">Op basis van de totale beschikbaarheid wordt de benodigde hoeveelheid voor elke vraagregel berekend.</span><span class="sxs-lookup"><span data-stu-id="9b626-139">Based on total availability, the quantity needed for each demand line is calculated.</span></span> <span data-ttu-id="9b626-140">Deze berekening wordt per order uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="9b626-140">This calculation is performed order-by-order.</span></span> <span data-ttu-id="9b626-141">Dit betekent dat de order met de vraagregel met de vroegste verval- of verzenddatum eerst wordt berekend.</span><span class="sxs-lookup"><span data-stu-id="9b626-141">This means that the order which includes the demand line with the earliest due date or shipment date will be calculated first.</span></span> <span data-ttu-id="9b626-142">Vervolgens worden aanvullende vraagregels in dezelfde volgorde berekend, ongeacht de vervaldatum of de verzenddatum.</span><span class="sxs-lookup"><span data-stu-id="9b626-142">After that, additional demand lines will be calculated in the same order, regardless of the due date or shipment date.</span></span>  

3.  <span data-ttu-id="9b626-143">Het venster **Orderplanning** moet zijn gemaximaliseerd en de afmetingen van de kolomvelden moeten zo zijn ingesteld dat alle standaardveldnamen zichtbaar zijn.</span><span class="sxs-lookup"><span data-stu-id="9b626-143">Be sure that the **Order Planning** window is maximized and that column fields are resized to show all the default field names.</span></span>  

     <span data-ttu-id="9b626-144">Wanneer de berekening is voltooid, worden in het venster alle niet-afgehandelde vraagregels weergegeven als samengevouwen orderkopregels gesorteerd op de vroegste vraagdatum.</span><span class="sxs-lookup"><span data-stu-id="9b626-144">When the calculation is completed, the window displays all unfulfilled demand as collapsed order header lines sorted by earliest demand date.</span></span>  

     <span data-ttu-id="9b626-145">U ziet dat CRONUS diverse orders heeft met niet-afgehandelde vraag.</span><span class="sxs-lookup"><span data-stu-id="9b626-145">Notice that CRONUS has several orders with unfulfilled demand.</span></span> <span data-ttu-id="9b626-146">Elke vette planningsregel geeft een order weer, verkoop of productie, met inbegrip van ten minste één orderregel met onvoldoende beschikbaarheid.</span><span class="sxs-lookup"><span data-stu-id="9b626-146">Each bold planning line represents an order, sales order, or production order, including at least one order line with insufficient availability.</span></span>  

4.  <span data-ttu-id="9b626-147">Selecteer in het veld **Vraag weergeven als** het filter **Alle vraag**.</span><span class="sxs-lookup"><span data-stu-id="9b626-147">In the **Show Demand As** field, select the **All Demand** filter.</span></span>  

     <span data-ttu-id="9b626-148">In het veld **Soort vraag** kunt u kiezen welke soorten orders u wilt weergeven.</span><span class="sxs-lookup"><span data-stu-id="9b626-148">With the **Demand Type** field, you can choose which order types that you want to display.</span></span>  

     <span data-ttu-id="9b626-149">Orders zonder beschikbaarheidsproblemen worden niet weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9b626-149">Orders that do not have availability problems are not shown.</span></span> <span data-ttu-id="9b626-150">Als er geen orders bestaan wanneer een planning wordt berekend, verschijnt een bericht en worden er geen planningsregels weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9b626-150">If no orders exist when a plan is calculated, a message will display and no planning lines will appear.</span></span>  

## <a name="planning-a-purchase-order-to-fulfill-component-demand"></a><span data-ttu-id="9b626-151">Een inkooporder plannen om te voldoen aan de vraag naar onderdelen</span><span class="sxs-lookup"><span data-stu-id="9b626-151">Planning a Purchase Order to Fulfill Component Demand</span></span>  
 <span data-ttu-id="9b626-152">In deze procedure maakt u een inkooporder voor de benodigde productieonderdelen.</span><span class="sxs-lookup"><span data-stu-id="9b626-152">In this procedure, you create a purchase order for needed manufacturing components.</span></span>  

### <a name="to-plan-a-purchase-order-to-fulfill-component-need-in-production"></a><span data-ttu-id="9b626-153">Een inkooporder plannen om te voldoen aan de onderdelenbehoefte voor de productie</span><span class="sxs-lookup"><span data-stu-id="9b626-153">To plan a purchase order to fulfill component need in production</span></span>  

1.  <span data-ttu-id="9b626-154">Vouw de eerste regel uit (klik op het symbool +).</span><span class="sxs-lookup"><span data-stu-id="9b626-154">Expand the first line (choose the + symbol).</span></span>  
2.  <span data-ttu-id="9b626-155">Kies de eerste vraagregel met, artikel, **LSU-15** en kies de actie **Document weergeven**.</span><span class="sxs-lookup"><span data-stu-id="9b626-155">Choose the first demand line, with item **LSU-15**, and then choose the **Show Document** action.</span></span>  
3.  <span data-ttu-id="9b626-156">Sluit de geopende productieorder om terug te keren naar het venster **Orderplanning**.</span><span class="sxs-lookup"><span data-stu-id="9b626-156">Close the opened production order to return to the **Order Planning** window.</span></span>  
4.  <span data-ttu-id="9b626-157">Selecteer **Inkoop** in het veld **Aanvullingsmethode**.</span><span class="sxs-lookup"><span data-stu-id="9b626-157">In the **Replenishment System** field, select **Purchase**.</span></span>  

     <span data-ttu-id="9b626-158">De standaardwaarde komt van de artikelkaart (of SKU-kaart), maar u kunt dit wijzigen in een van de volgende opties:</span><span class="sxs-lookup"><span data-stu-id="9b626-158">The default value is from the item card, or SKU card, but you can change it to one of the following options:</span></span>  

    -   <span data-ttu-id="9b626-159">**Inkoop** – een inkooporder maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-159">**Purchase** – To create a purchase order.</span></span>  
    -   <span data-ttu-id="9b626-160">**Transfer** – een transferorder maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-160">**Transfer** – To create a transfer order.</span></span>  
    -   <span data-ttu-id="9b626-161">**Prod.-order** – een productieorder maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-161">**Prod. Order** – To create a production order.</span></span>  

5.  <span data-ttu-id="9b626-162">Selecteer in het veld **Aanleveren van** een van de volgende opties op basis van de geselecteerde aanvullingsmethode:</span><span class="sxs-lookup"><span data-stu-id="9b626-162">In the **Supply From** field, select one of the following options according to the selected replenishment system:</span></span>  

    -   <span data-ttu-id="9b626-163">**Leverancier** – Voor inkoop</span><span class="sxs-lookup"><span data-stu-id="9b626-163">**Vendor** – For purchases</span></span>  
    -   <span data-ttu-id="9b626-164">**Locatie** – voor transfers</span><span class="sxs-lookup"><span data-stu-id="9b626-164">**Location** – For transfers</span></span>  

     <span data-ttu-id="9b626-165">Als het veld niet is ingevuld, verschijnt er een foutbericht wanneer u voorraadorders probeert te maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-165">If the field is not filled in, an error message will display when you try to create the supply orders.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9b626-166">Als voor de onderdelen een standaardleveranciernummer is ingesteld op de artikelkaarten, zijn de regels vooraf ingevuld.</span><span class="sxs-lookup"><span data-stu-id="9b626-166">If the components have a default vendor number set up on the item cards, the lines will be preset.</span></span>  

6.  <span data-ttu-id="9b626-167">Kies het veld **Aanleveren van**.</span><span class="sxs-lookup"><span data-stu-id="9b626-167">Choose the **Supply From**  field.</span></span>  
7.  <span data-ttu-id="9b626-168">Kies in het venster **Artikelleveranciers** de actie **Nieuw** en selecteer leverancier **30000**.</span><span class="sxs-lookup"><span data-stu-id="9b626-168">In the **Item Vendor Catalogue** window, choose the **New** action, and then select vendor **30000**.</span></span>  
8.  <span data-ttu-id="9b626-169">Kies de knop **OK** om terug te gaan naar het venster **Orderplanning**.</span><span class="sxs-lookup"><span data-stu-id="9b626-169">Choose the **OK** button to return to the **Order Planning** window.</span></span>  
9. <span data-ttu-id="9b626-170">Kopieer leveranciernummer **30000** naar de overige regels voor luidsprekeronderdelen in deze productieorder.</span><span class="sxs-lookup"><span data-stu-id="9b626-170">Copy vendor **30000** to the other lines for loudspeaker components on this production order.</span></span>  

     <span data-ttu-id="9b626-171">U kunt nu een inkooporder gaan maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-171">You are now ready to create a purchase order.</span></span>  

10. <span data-ttu-id="9b626-172">Kies de actie **Orders maken**.</span><span class="sxs-lookup"><span data-stu-id="9b626-172">Choose the **Make Orders** action.</span></span> <span data-ttu-id="9b626-173">Het venster **Orders voor voorzieningen maken** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="9b626-173">The **Make Supply Orders** window opens.</span></span>  
11. <span data-ttu-id="9b626-174">Kies op het sneltabblad **Orderplanning** in het veld **Orders maken voor** de optie **Actieve order**.</span><span class="sxs-lookup"><span data-stu-id="9b626-174">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **Active Order** option.</span></span>  
12. <span data-ttu-id="9b626-175">Kies op het sneltabblad **Opties** in het veld **Inkooporder maken** de optie **Inkooporders maken**.</span><span class="sxs-lookup"><span data-stu-id="9b626-175">On the **Options** FastTab, in the **Create Purchase Order** field, choose the **Make Purch. Order** option.</span></span>  
13. <span data-ttu-id="9b626-176">Klik op **OK** om inkooporders te maken voor alle onderdelen van de order.</span><span class="sxs-lookup"><span data-stu-id="9b626-176">Choose the **OK** button to create purchase orders for all the components of the order.</span></span>  

     <span data-ttu-id="9b626-177">De inkooporders worden gemaakt en opgeslagen als de laatste orders in de lijst met inkooporders.</span><span class="sxs-lookup"><span data-stu-id="9b626-177">The purchase orders are now created and saved as the last orders in the list of purchase orders.</span></span>  

## <a name="planning-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="9b626-178">Een transferorder plannen om aan de verkoopvraag te voldoen</span><span class="sxs-lookup"><span data-stu-id="9b626-178">Planning a Transfer Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="9b626-179">In deze procedure gaat u plannen voor de vraag van een verkooporder.</span><span class="sxs-lookup"><span data-stu-id="9b626-179">In this procedure, you will plan for demand from a sales order.</span></span> <span data-ttu-id="9b626-180">Vraagregels geven de verkoopregels aan en niet de onderdeelregels, zoals bij de productievraag.</span><span class="sxs-lookup"><span data-stu-id="9b626-180">Demand lines represent sales lines and not component lines, as in production demand.</span></span>  

### <a name="to-plan-a-transfer-order-to-fulfill-sales-demand"></a><span data-ttu-id="9b626-181">Een transferorder plannen om aan de verkoopvraag te voldoen</span><span class="sxs-lookup"><span data-stu-id="9b626-181">To plan a transfer order to fulfill sales demand</span></span>  

1.  <span data-ttu-id="9b626-182">Verplaats de aanwijzer naar de planningsregel voor ordernummer **2008**.</span><span class="sxs-lookup"><span data-stu-id="9b626-182">Move the pointer to the planning line for order **2008**.</span></span>  
2.  <span data-ttu-id="9b626-183">Vouw de regel uit en verplaats de aanwijzer naar de vraagregel.</span><span class="sxs-lookup"><span data-stu-id="9b626-183">Expand the line and move the pointer to the demand line.</span></span>  

     <span data-ttu-id="9b626-184">Verkooporder **2008 betreft** tien luidsprekers van het type **LS-120** die zijn besteld door John Haddock Insurance Co.</span><span class="sxs-lookup"><span data-stu-id="9b626-184">Sales order **2008** is for ten loudspeakers, item **LS-120**, ordered by John Haddock Insurance Co.</span></span>  

     <span data-ttu-id="9b626-185">Voor het artikel is het aanvulsysteem geselecteerd en de standaardleverancier wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9b626-185">The item’s defined replenishment system and default vendor will display.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9b626-186">Onder aan het venster staan vier informatievelden.</span><span class="sxs-lookup"><span data-stu-id="9b626-186">At the bottom of the window, there are four information fields.</span></span> <span data-ttu-id="9b626-187">In het veld **Vroegste beschikbaarheidsdatum** zijn de tien stuks die nodig zijn, beschikbaar via een inkomende voorraadorder, maar pas negen dagen na de huidige vervaldatum.</span><span class="sxs-lookup"><span data-stu-id="9b626-187">In the **Earliest Date Available** field, the ten pieces that are needed will be available, on an inbound supply order, nine days later than the current due date.</span></span> <span data-ttu-id="9b626-188">Als dat te laat is voor de klant, bevat het veld **Beschikbaar voor transfer** 13 stuks van het artikel op een andere locatie.</span><span class="sxs-lookup"><span data-stu-id="9b626-188">If this is too late for the customer, the **Available for Transfer** field shows 13 pieces of the item at another location.</span></span> <span data-ttu-id="9b626-189">U gaat voor deze voorraad een planning maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-189">You will want to plan for this stock.</span></span>  

3.  <span data-ttu-id="9b626-190">Kies het veld **Beschikbaar voor transfer** om het venster **Alternatieve voorziening ophalen** te openen.</span><span class="sxs-lookup"><span data-stu-id="9b626-190">Choose the **Available for Transfer** field to open the **Get Alternative Supply** window.</span></span>  
4.  <span data-ttu-id="9b626-191">Klik op **OK** om de tien beschikbare artikelen te boeken.</span><span class="sxs-lookup"><span data-stu-id="9b626-191">Choose the **OK** button to book the ten items that are available.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9b626-192">Op de vraagregel wordt de voorgestelde inkoop vervangen door een transfer van de locatie GROEN.</span><span class="sxs-lookup"><span data-stu-id="9b626-192">In the demand line, the suggested purchase has been exchanged with a transfer from GREEN location.</span></span> <span data-ttu-id="9b626-193">Met de functie **Orders maken** maakt u een transferorder van GROEN naar de gewenste locatie.</span><span class="sxs-lookup"><span data-stu-id="9b626-193">The **Make Orders** function creates a transfer order from GREEN to the demanded location.</span></span> <span data-ttu-id="9b626-194">Het veld **Vervangingsartikel** werkt op dezelfde manier.</span><span class="sxs-lookup"><span data-stu-id="9b626-194">The **Substitutes Exists** field works in the same way.</span></span>  

5.  <span data-ttu-id="9b626-195">Kies de actie **Orders maken**.</span><span class="sxs-lookup"><span data-stu-id="9b626-195">Choose the **Make Orders** action.</span></span> <span data-ttu-id="9b626-196">Het venster **Aanvulorders maken** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="9b626-196">The **Make Supply Orders** window opens.</span></span>  
6.  <span data-ttu-id="9b626-197">Kies op het sneltabblad **Orderplanning** in het veld **Orders maken voor** de optie **Actieve order**.</span><span class="sxs-lookup"><span data-stu-id="9b626-197">On the **Order Planning** FastTab, in the **Make Orders for** field, choose the **The Active Order** option.</span></span>  
7.  <span data-ttu-id="9b626-198">Selecteer op het sneltabblad **Opties** in het veld **Transferorder maken** de optie **Transferorders maken**.</span><span class="sxs-lookup"><span data-stu-id="9b626-198">On the **Options** FastTab, in the **Create Transfer Order** field, select the **Make Trans. Orders** option.</span></span>  
8.  <span data-ttu-id="9b626-199">Klik op **OK** om de transferorder te maken om te voldoen aan de verkooporder.</span><span class="sxs-lookup"><span data-stu-id="9b626-199">Choose the **OK** button to create the transfer order to supply the sales order.</span></span>  

     <span data-ttu-id="9b626-200">De transferorder is nu gemaakt en in de lijst opgeslagen als de laatste order in de lijst met open transferorders.</span><span class="sxs-lookup"><span data-stu-id="9b626-200">The transfer order is now created and saved in the list as the last order in the list of open transfer orders.</span></span>  

## <a name="planning-a-multilevel-production-order-to-fulfill-sales-demand"></a><span data-ttu-id="9b626-201">Een productieorder met meerdere niveaus plannen om aan de verkoopvraag te voldoen</span><span class="sxs-lookup"><span data-stu-id="9b626-201">Planning a Multilevel Production Order to Fulfill Sales Demand</span></span>  
 <span data-ttu-id="9b626-202">In deze procedure gaat u plannen om aan de verkoopvraag te voldoen voor een geproduceerd artikel met meerdere productniveaus, waarbij de productievraag voor alle niveaus samenhangt.</span><span class="sxs-lookup"><span data-stu-id="9b626-202">In this procedure, you will plan to fulfill sales demand for a produced item with multiple product levels, each creating dependent production demand.</span></span>  

### <a name="to-plan-multilevel-production-to-fulfill-sales-demand"></a><span data-ttu-id="9b626-203">Een productie met meerdere niveaus plannen om aan de verkoopvraag te voldoen</span><span class="sxs-lookup"><span data-stu-id="9b626-203">To plan multilevel production to fulfill sales demand</span></span>  

1.  <span data-ttu-id="9b626-204">Selecteer de planningsregel met de verkoopvraag voor ordernummer **1001** (gemaakt bij de vereiste gegevens).</span><span class="sxs-lookup"><span data-stu-id="9b626-204">Select the planning line with sales demand for order **1001**, created earlier as prerequisite data.</span></span>  

     <span data-ttu-id="9b626-205">Deze vraag is een verkoopregel maar voor het artikel is het aanvulsysteem **Prod.-order** gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="9b626-205">This demand is a sales line, but the item has a defined replenishment system of **Prod. Order**.</span></span> <span data-ttu-id="9b626-206">Voeg een tweede bel toe aan de onderdelenlijst voor elke fiets.</span><span class="sxs-lookup"><span data-stu-id="9b626-206">Proceed to add an extra bell to the component need of each bicycle.</span></span>  

2.  <span data-ttu-id="9b626-207">Kies de actie **Materialen** om het venster **Planningsmaterialen** te openen.</span><span class="sxs-lookup"><span data-stu-id="9b626-207">Choose the **Components** action to open the **Planning Components** window.</span></span>  
3.  <span data-ttu-id="9b626-208">Wijzig in de regel voor de fietsbel het veld **Aantal per** van **1** in **2**.</span><span class="sxs-lookup"><span data-stu-id="9b626-208">On the line with the Bell item, change the **Quantity per** field from **1** to **2**.</span></span>  
4.  <span data-ttu-id="9b626-209">Bekijk in het venster **Orderplanning** de planningsalternatieven.</span><span class="sxs-lookup"><span data-stu-id="9b626-209">In the **Order Planning** window, consider your planning alternatives.</span></span> <span data-ttu-id="9b626-210">In dit geval zijn er geen alternatieve leveringsmethoden, geen transfer, geen vervangend artikel en geen latere levering.</span><span class="sxs-lookup"><span data-stu-id="9b626-210">In this case, you have no alternative means of supply, no transfer, substitute, or later delivery.</span></span> <span data-ttu-id="9b626-211">U moet de voorgestelde voorzieningsorder, een productieorder, maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-211">You must create the suggested supply order, a production order.</span></span>  
5.  <span data-ttu-id="9b626-212">Kies de actie **Orders maken** om de productieorder te maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-212">Choose the **Make Orders** action to create the production order.</span></span>  

     <span data-ttu-id="9b626-213">U ziet dat in het venster **Orderplanning** de planningregel voor verkooporder **1001** niet meer bestaat en dat aan de eerste verkoopvraag is voldaan.</span><span class="sxs-lookup"><span data-stu-id="9b626-213">In the **Order Planning** window, notice that the planning line for sales order **1001** no longer exists and that the initial sales demand has been covered.</span></span>  

6.  <span data-ttu-id="9b626-214">Sluit het venster **Orderplanning**.</span><span class="sxs-lookup"><span data-stu-id="9b626-214">Close the **Order Planning** window.</span></span>  

     <span data-ttu-id="9b626-215">U zou nu in deze weergave kunnen blijven om alle planningstaken te voltooien.</span><span class="sxs-lookup"><span data-stu-id="9b626-215">Now, you could choose to stay in this view and complete all the planning tasks.</span></span> <span data-ttu-id="9b626-216">In plaats daarvan neemt u nu de rol van de productieplanner op en gaat u naar de zojuist gemaakte productieorder om het venster **Orderplanning** te openen.</span><span class="sxs-lookup"><span data-stu-id="9b626-216">Instead, you will now take on the Production Planner role by going to the production order that you just created and access the **Order Planning** window.</span></span>  

 <span data-ttu-id="9b626-217">Als productieplanner moet u nu een specifieke productieorder plannen.</span><span class="sxs-lookup"><span data-stu-id="9b626-217">As a production planner you now must plan a specific production order.</span></span>  

### <a name="to-plan-a-specific-production-order"></a><span data-ttu-id="9b626-218">Een specifieke productieorder plannen</span><span class="sxs-lookup"><span data-stu-id="9b626-218">To plan a specific production order</span></span>  

1.  <span data-ttu-id="9b626-219">Open de productieorder **101001** (voor tien fietsen) die u hebt gemaakt met de functie **Orders maken**.</span><span class="sxs-lookup"><span data-stu-id="9b626-219">Open the production order **101001**, for ten bicycles, that you just created by using the **Make Orders** function.</span></span>  
2.  <span data-ttu-id="9b626-220">Open het venster **Prod.-ordermaterialen** om te controleren of de extra bel wordt weergegeven op de productieorder.</span><span class="sxs-lookup"><span data-stu-id="9b626-220">Open the **Prod. Order Components** window to check that the extra bell is reflected on the production order.</span></span>  
3.  <span data-ttu-id="9b626-221">Kies de actie **Planning**.</span><span class="sxs-lookup"><span data-stu-id="9b626-221">Choose the **Planning** action.</span></span>  

     <span data-ttu-id="9b626-222">Het venster **Orderplanning** wordt geopend in een weergave die altijd wordt gefilterd op de specifieke productievraag.</span><span class="sxs-lookup"><span data-stu-id="9b626-222">The **Order Planning** window opens in a view that is always filtered on the specific production demand.</span></span> <span data-ttu-id="9b626-223">De verkoopvraag wordt niet weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9b626-223">Sales demand is not displayed.</span></span> <span data-ttu-id="9b626-224">U moet eerst een planning berekenen voordat een nieuwe vraag wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="9b626-224">You must calculate a plan before you can see any additional demand.</span></span>  

4.  <span data-ttu-id="9b626-225">Kies de actie **Plan berekenen**.</span><span class="sxs-lookup"><span data-stu-id="9b626-225">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="9b626-226">U ziet dat er vier nieuwe productieorders verschijnen voor de niet-geplande productievraag op basis van order **101001.**</span><span class="sxs-lookup"><span data-stu-id="9b626-226">Notice that four new production orders appear as unplanned production demand derived from order **101001**.</span></span> <span data-ttu-id="9b626-227">De nieuwe regels geven de nieuwe productievraag weer voor de subassemblages die moeten worden gemaakt om de order te produceren.</span><span class="sxs-lookup"><span data-stu-id="9b626-227">The new lines represent new production demand from the subassemblies that must be created to produce the order.</span></span>  

5.  <span data-ttu-id="9b626-228">Kies de actie **Alles uitvouwen** om een overzicht te krijgen van de volledige productievraag voor de productieorders.</span><span class="sxs-lookup"><span data-stu-id="9b626-228">Choose the **Expand All** action to get an overview of all the production demand for the production orders.</span></span>  

     <span data-ttu-id="9b626-229">Als u aanvullende informatie over de vraagregels wilt verstrekken, kunt u de velden **Aantal vraag** en **Beschikbaar aantal vraag** toevoegen aan uw weergave.</span><span class="sxs-lookup"><span data-stu-id="9b626-229">To provide additional information about the demand lines, you may want to add the **Demand Quantity** and **Demand Qty. Available** fields to your view.</span></span>  

     <span data-ttu-id="9b626-230">U moet nu tien stuks van elk onderdeel leveren.</span><span class="sxs-lookup"><span data-stu-id="9b626-230">Now you must supply ten of each component.</span></span>  

     <span data-ttu-id="9b626-231">Houd er rekening mee dat vier van de vraagregels aanvullingsmethode Prod.-order hebben.</span><span class="sxs-lookup"><span data-stu-id="9b626-231">Note that four of the demand lines have replenishment system Prod. Order.</span></span> <span data-ttu-id="9b626-232">Deze vier halffabrikaten vertegenwoordigen het tweede productniveau van de fiets.</span><span class="sxs-lookup"><span data-stu-id="9b626-232">These four subassemblies represent the second product level of the bicycle.</span></span>  

     <span data-ttu-id="9b626-233">De standaardinstellingen voor aanvulling zijn al ingevuld en u kunt de orders gaan maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-233">The default replenishment settings are already filled in and you can proceed to make orders.</span></span>  

6.  <span data-ttu-id="9b626-234">Kies de actie **Orders maken**.</span><span class="sxs-lookup"><span data-stu-id="9b626-234">Choose the **Make Orders** action.</span></span>  

     <span data-ttu-id="9b626-235">Lees, voordat u de knop **OK** kiest, de tekst op het sneltabblad **Orderplanning**.</span><span class="sxs-lookup"><span data-stu-id="9b626-235">Before you choose the **OK** button, notice the text on the **Order Planning** FastTab.</span></span> <span data-ttu-id="9b626-236">Deze tekst is belangrijk omdat u weet dat de productstructuur van de fiets een aantal geproduceerde onderdelen (subassemblages) bevat die in de vraag worden opgenomen wanneer u deze productieorder maakt.</span><span class="sxs-lookup"><span data-stu-id="9b626-236">This text is important because you know that the bicycle has several produced components, subassemblies, in its product structure that might be in demand when you create this production order.</span></span>  

7.  <span data-ttu-id="9b626-237">Kies in het venster **Orders voor voorzieningen maken** in het veld **Orders maken voor** de optie **Alle regels** en kies vervolgens de knop **OK** om productieorders te maken voor het tweede productniveau van de order.</span><span class="sxs-lookup"><span data-stu-id="9b626-237">In the **Make Supply Order** window, in the **Make Orders for** field, choose the **All Lines** option, and then choose the **OK** button to create production orders for the second product level of the order.</span></span>  

     <span data-ttu-id="9b626-238">U ziet dat de hoogste productievraag voor productieorder 101001 niet meer bestaat.</span><span class="sxs-lookup"><span data-stu-id="9b626-238">Note that the top-level production demand for production order 101001 no longer exists.</span></span> <span data-ttu-id="9b626-239">Dat betekent dat de aanvankelijke productievraag voor subassemblages nu is ingepland.</span><span class="sxs-lookup"><span data-stu-id="9b626-239">This means that the initial production demand for subassemblies has been planned for.</span></span>  

     <span data-ttu-id="9b626-240">Bereken in het venster **Orderplanning** nogmaals de planning om de fietsstructuur te plannen.</span><span class="sxs-lookup"><span data-stu-id="9b626-240">In the **Order Planning** window, you calculate a plan again in order to plan the bicycle structure.</span></span>  

8.  <span data-ttu-id="9b626-241">Kies de actie **Planning berekenen** om de planning opnieuw te berekenen volgens de instructies uit de Help-tekst.</span><span class="sxs-lookup"><span data-stu-id="9b626-241">Choose the **Calculate Plan** action to recalculate the plan as instructed by the embedded Help text.</span></span>  

     <span data-ttu-id="9b626-242">De twee nieuwe regels geven de aanvullende productievraag aan die is afgeleid van de subassemblages die in de vorige stappen zijn gepland.</span><span class="sxs-lookup"><span data-stu-id="9b626-242">The two new lines represent additional production demand derived from the subassemblies planned in the previous steps.</span></span> <span data-ttu-id="9b626-243">Er wordt aangegeven dat u twee productieorders maakt voor de wielnaven, een voor 10 voornaven en een voor 10 achternaven.</span><span class="sxs-lookup"><span data-stu-id="9b626-243">It is suggested that you make two production orders to supply the wheel hubs, one for 10 front hubs and one for 10 back hubs.</span></span>  

9. <span data-ttu-id="9b626-244">Kies de actie **Alles uitvouwen** om een overzicht te krijgen van de twee productieorders.</span><span class="sxs-lookup"><span data-stu-id="9b626-244">Choose the **Expand All** action to get an overview of all the demand for the two production orders.</span></span>  

     <span data-ttu-id="9b626-245">Het voorgestelde voorzieningsplan geeft aan dat er in totaal vier inkooporders worden gemaakt voor de onderdelen.</span><span class="sxs-lookup"><span data-stu-id="9b626-245">The suggested supply plan indicates that a total of four purchase orders will be created for the components.</span></span> <span data-ttu-id="9b626-246">U besluit de voorgestelde orders te maken.</span><span class="sxs-lookup"><span data-stu-id="9b626-246">You decide to make the proposed orders.</span></span>  

10. <span data-ttu-id="9b626-247">Kies de actie **Orders maken**.</span><span class="sxs-lookup"><span data-stu-id="9b626-247">Choose the **Make Orders** action.</span></span>  
11. <span data-ttu-id="9b626-248">Selecteer in het veld **Orders maken voor** de optie **Alle regels** en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="9b626-248">In the **Make Orders for** field, select the **All Lines** option, and then choose the **OK** button.</span></span> <span data-ttu-id="9b626-249">Controleer of er een aanvullende vraag bestaat voor de productie van het hoofdartikel, de fiets (verkocht op verkooporder 1001).</span><span class="sxs-lookup"><span data-stu-id="9b626-249">Check if additional demand exists for the production of the parent item, the bicycle, which is being sold on sales order 1001.</span></span>  
12. <span data-ttu-id="9b626-250">Kies de actie **Plan berekenen**.</span><span class="sxs-lookup"><span data-stu-id="9b626-250">Choose the **Calculate Plan** action.</span></span>  

     <span data-ttu-id="9b626-251">Het bericht geeft aan dat nu in alle vereiste artikelen is voorzien.</span><span class="sxs-lookup"><span data-stu-id="9b626-251">The message indicates that all required items are now supplied.</span></span> <span data-ttu-id="9b626-252">Controleer de vast gepland productieorders die worden gemaakt.</span><span class="sxs-lookup"><span data-stu-id="9b626-252">Verify the firm planned production orders that are created.</span></span>  

13. <span data-ttu-id="9b626-253">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vast geplande productieorders** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9b626-253">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Firm Planned Prod. Orders**, and then choose the related link.</span></span>  

     <span data-ttu-id="9b626-254">Bekijk in het venster **Vast geplande productieorders** hoe de begin- en eindtijden van afzonderlijke orders nu zijn gepland volgens de productstructuur.</span><span class="sxs-lookup"><span data-stu-id="9b626-254">In the **Firm Planned Prod. Orders** window review how start times and end times of individual orders are scheduled according to the product structure.</span></span> <span data-ttu-id="9b626-255">De onderdelen op het laagste niveau worden het eerst geproduceerd.</span><span class="sxs-lookup"><span data-stu-id="9b626-255">The lowest-level components are produced first.</span></span> <span data-ttu-id="9b626-256">Daarom moet u orders met meerdere niveaus plannen zoals is gedemonstreerd in deze planningswerkstroom.</span><span class="sxs-lookup"><span data-stu-id="9b626-256">Therefore, you must plan multilevel orders as demonstrated in this planning workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9b626-257">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9b626-257">See Also</span></span>  
 <span data-ttu-id="9b626-258">[Procedures voor bedrijfsprocessen](walkthrough-business-process-walkthroughs.md) </span><span class="sxs-lookup"><span data-stu-id="9b626-258">[Business Process Walkthroughs](walkthrough-business-process-walkthroughs.md) </span></span>  
 [<span data-ttu-id="9b626-259">Procedure: Goederen automatisch plannen</span><span class="sxs-lookup"><span data-stu-id="9b626-259">Walkthrough: Planning Supplies Automatically</span></span>](walkthrough-planning-supplies-automatically.md)
