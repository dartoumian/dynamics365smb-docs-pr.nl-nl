---
title: 'Ontwerpdetails: Assemblageorderboeking | Microsoft Docs'
description: Assemblageorderboeking wordt gebaseerd op dezelfde principes als wanneer de soortgelijke activiteiten van verkooporders en productieverbruik/-output worden geboekt. De principes worden echter gecombineerd in de zin dat assemblageorders hun eigen boeking-UI hebben, zoals die voor verkooporders, terwijl de feitelijke postboeking op de achtergrond wordt uitgevoerd als directe artikel- en resourcedagboekboekingen, zoals die voor productieverbruik, output en capaciteit.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 66590eb8ce7749658bad1fc3c9e54c1dff538abd
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-assembly-order-posting"></a><span data-ttu-id="79e43-104">Ontwerpdetails: Assemblageorderboeking</span><span class="sxs-lookup"><span data-stu-id="79e43-104">Design Details: Assembly Order Posting</span></span>
<span data-ttu-id="79e43-105">Assemblageorderboeking wordt gebaseerd op dezelfde principes als wanneer de soortgelijke activiteiten van verkooporders en productieverbruik/-output worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="79e43-105">Assembly order posting is based on the same principles as when posting the similar activities of sales orders and production consumption/output.</span></span> <span data-ttu-id="79e43-106">De principes worden echter gecombineerd in de zin dat assemblageorders hun eigen boeking-UI hebben, zoals die voor verkooporders, terwijl de feitelijke postboeking op de achtergrond wordt uitgevoerd als directe artikel- en resourcedagboekboekingen, zoals die voor productieverbruik, output en capaciteit.</span><span class="sxs-lookup"><span data-stu-id="79e43-106">However, the principles are combined in that assembly orders have their own posting UI, like that for sales orders, while the actual entry posting happens in the background as direct item and resource journal postings, like that for production consumption, output, and capacity.</span></span>  

<span data-ttu-id="79e43-107">Net als bij productieorderboeking worden de verbruikte materialen en de gebruikte resources omgezet en uitgevoerd als de component wanneer de productieorder is voltooid.</span><span class="sxs-lookup"><span data-stu-id="79e43-107">Similarly to production order posting, the consumed components and the used resources are converted and output as the assembly item when the assembly order is posted.</span></span> <span data-ttu-id="79e43-108">Zie [Ontwerpdetails: Productieorderboeking](design-details-production-order-posting.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="79e43-108">For more information, see [Design Details: Production Order Posting](design-details-production-order-posting.md).</span></span> <span data-ttu-id="79e43-109">De kostenstroom voor assemblageorders is echter minder complex, met name omdat de assemblagekostenboeking slechts eenmaal plaatsvindt en daarom geen OHW-voorraad genereert.</span><span class="sxs-lookup"><span data-stu-id="79e43-109">However, the cost flow for assembly orders is less complex, especially because assembly cost posting only occurs once and therefore does not generate work-in-process inventory.</span></span>  

<span data-ttu-id="79e43-110">De volgende dagboekboekingen treden op tijdens assemblageorderboekingen:</span><span class="sxs-lookup"><span data-stu-id="79e43-110">The following journal postings occur during assembly order posting:</span></span>  

-   <span data-ttu-id="79e43-111">Het artikeldagboek boekt positieve artikelposten, die output van het assemblageartikel vertegenwoordigen, uit de assemblageorderkop.</span><span class="sxs-lookup"><span data-stu-id="79e43-111">The item journal posts positive item ledger entries, representing output of the assembly item, from the assembly order header</span></span>  
-   <span data-ttu-id="79e43-112">Het artikeldagboek boekt negatieve artikelposten, die verbruik van assemblagecomponenten vertegenwoordigen, uit de assemblageorderregels.</span><span class="sxs-lookup"><span data-stu-id="79e43-112">The item journal posts negative item ledger entries, representing consumption of assembly components, from the assembly order lines.</span></span>  
-   <span data-ttu-id="79e43-113">Het resourcedagboek boekt gebruik van assemblageresources (tijdseenheden) vanaf de assemblageorderregels.</span><span class="sxs-lookup"><span data-stu-id="79e43-113">The resource journal posts usage of assembly resources (time units), from the assembly order lines.</span></span>  
-   <span data-ttu-id="79e43-114">Het capaciteitsdagboek boekt waardeposten die betrekking hebben op het resourceverbruik, vanaf de assemblageorderregels.</span><span class="sxs-lookup"><span data-stu-id="79e43-114">The capacity journal posts value entries relating to the resource usage, from the assembly order lines.</span></span>  

<span data-ttu-id="79e43-115">Het volgende diagram bevat de structuur van artikel- en resourceposten die het gevolg zijn van assemblageorderboeking.</span><span class="sxs-lookup"><span data-stu-id="79e43-115">The following diagram shows the structure of item and resource ledger entries that result from assembly order posting.</span></span>  

<span data-ttu-id="79e43-116">![Resource- en capaciteitskosten](media/design_details_assembly_posting_1.png "design_details_assembly_posting_1")</span><span class="sxs-lookup"><span data-stu-id="79e43-116">![Resource and capacity costs](media/design_details_assembly_posting_1.png "design_details_assembly_posting_1")</span></span>  

> [!NOTE]  
>  <span data-ttu-id="79e43-117">Bewerkingsplaatsen en afdelingen zijn opgenomen om te illustreren dat capaciteitsposten zowel worden gemaakt vanuit productie als vanuit assemblage.</span><span class="sxs-lookup"><span data-stu-id="79e43-117">Machine and work centers are included to illustrate that capacity ledger entries are created from both production and assembly.</span></span>  

<span data-ttu-id="79e43-118">In het volgende diagram wordt aangegeven hoe assemblagegegevens in posten stromen tijdens het boeken:</span><span class="sxs-lookup"><span data-stu-id="79e43-118">The following diagram shows how assembly data flows into ledger entries during posting:</span></span>  

<span data-ttu-id="79e43-119">![Gegevensstroom tijdens het boeken](media/design_details_assembly_posting_2.png "design_details_assembly_posting_2")</span><span class="sxs-lookup"><span data-stu-id="79e43-119">![Data flow during posting](media/design_details_assembly_posting_2.png "design_details_assembly_posting_2")</span></span>  

## <a name="posting-sequence"></a><span data-ttu-id="79e43-120">Boekingsvolgorde</span><span class="sxs-lookup"><span data-stu-id="79e43-120">Posting Sequence</span></span>  
<span data-ttu-id="79e43-121">De boeking van een assemblageorder vindt plaats in de volgende volgorde:</span><span class="sxs-lookup"><span data-stu-id="79e43-121">The posting of an assembly order occurs in the following order:</span></span>  

1.  <span data-ttu-id="79e43-122">De assemblageorderregels zijn geboekt.</span><span class="sxs-lookup"><span data-stu-id="79e43-122">The assembly order lines are posted.</span></span>  
2.  <span data-ttu-id="79e43-123">De assemblageorderkop is geboekt.</span><span class="sxs-lookup"><span data-stu-id="79e43-123">The assembly order header is posted.</span></span>  

<span data-ttu-id="79e43-124">De volgende tabel toont de volgorde van de acties.</span><span class="sxs-lookup"><span data-stu-id="79e43-124">The following table outlines the sequence of actions.</span></span>  

|<span data-ttu-id="79e43-125">Actie</span><span class="sxs-lookup"><span data-stu-id="79e43-125">Action</span></span>|<span data-ttu-id="79e43-126">Description</span><span class="sxs-lookup"><span data-stu-id="79e43-126">Description</span></span>|  
|------------|-----------------|  
|<span data-ttu-id="79e43-127">Boeking initialiseren</span><span class="sxs-lookup"><span data-stu-id="79e43-127">Initialize Posting</span></span>|<span data-ttu-id="79e43-128">1. Voer voorlopige controles uit.</span><span class="sxs-lookup"><span data-stu-id="79e43-128">1.  Make preliminary checks.</span></span><br /><span data-ttu-id="79e43-129">2. Voeg een boekingsnummer toe en wijzig de assemblageorderkop.</span><span class="sxs-lookup"><span data-stu-id="79e43-129">2.  Add posting number and modify the assembly order header.</span></span><br /><span data-ttu-id="79e43-130">3. Geef de assemblageorder vrij.</span><span class="sxs-lookup"><span data-stu-id="79e43-130">3.  Release the assembly order.</span></span>|  
|<span data-ttu-id="79e43-131">Post</span><span class="sxs-lookup"><span data-stu-id="79e43-131">Post</span></span>|<ol><li><span data-ttu-id="79e43-132">Maak de geboekte assemblageorderkop.</span><span class="sxs-lookup"><span data-stu-id="79e43-132">Create the posted assembly order header.</span></span></li><li><span data-ttu-id="79e43-133">Kopieer opmerkingsregels.</span><span class="sxs-lookup"><span data-stu-id="79e43-133">Copy comment lines.</span></span></li><li><span data-ttu-id="79e43-134">Boek assemblageorderregels (verbruik):</span><span class="sxs-lookup"><span data-stu-id="79e43-134">Post assembly order lines (consumption):</span></span><br /><br /> <ol><li><span data-ttu-id="79e43-135">Maak een statusvenster om assemblageverbruik te berekenen.</span><span class="sxs-lookup"><span data-stu-id="79e43-135">Create a status window to calculate assembly consumption.</span></span></li><li><span data-ttu-id="79e43-136">Haal het resterende aantal op waarop de artikeldagboekregel wordt gebaseerd.</span><span class="sxs-lookup"><span data-stu-id="79e43-136">Get the remaining quantity on which the item journal line will be based.</span></span></li><li><span data-ttu-id="79e43-137">Stel de verbruikte en resterende aantallen opnieuw in.</span><span class="sxs-lookup"><span data-stu-id="79e43-137">Reset the consumed and remaining quantities.</span></span></li><li><span data-ttu-id="79e43-138">Voor assemblageorderregels van de soort Artikel:</span><span class="sxs-lookup"><span data-stu-id="79e43-138">For assembly order lines of type Item:</span></span><br /><br /> <ol><li><span data-ttu-id="79e43-139">Vul velden op de artikeldagboekregel in.</span><span class="sxs-lookup"><span data-stu-id="79e43-139">Populate fields on the item journal line.</span></span></li><li><span data-ttu-id="79e43-140">Breng reserveringen over naar de artikeldagboekregel.</span><span class="sxs-lookup"><span data-stu-id="79e43-140">Transfer reservations to the item journal line.</span></span></li><li><span data-ttu-id="79e43-141">Boek de artikeldagboekregel om de artikelposten te maken.</span><span class="sxs-lookup"><span data-stu-id="79e43-141">Post the item journal line to create the item ledger entries.</span></span></li><li><span data-ttu-id="79e43-142">Maak magazijndagboekregels en boek ze.</span><span class="sxs-lookup"><span data-stu-id="79e43-142">Create warehouse journal lines and post them.</span></span></li></ol></li><li><span data-ttu-id="79e43-143">Voor assemblageorderregels van de soort Resource:</span><span class="sxs-lookup"><span data-stu-id="79e43-143">For assembly order lines of type Resource:</span></span><br /><br /> <ol><li><span data-ttu-id="79e43-144">Vul velden op de artikeldagboekregel in.</span><span class="sxs-lookup"><span data-stu-id="79e43-144">Populate fields on the item journal line.</span></span></li><li><span data-ttu-id="79e43-145">Boek de artikeldagboekregel.</span><span class="sxs-lookup"><span data-stu-id="79e43-145">Post the item journal line.</span></span> <span data-ttu-id="79e43-146">Hierdoor ontstaan capaciteitsposten.</span><span class="sxs-lookup"><span data-stu-id="79e43-146">This creates capacity ledger entries.</span></span></li><li><span data-ttu-id="79e43-147">Maak en boek een resourcedagboekregel.</span><span class="sxs-lookup"><span data-stu-id="79e43-147">Create and post resource journal line.</span></span></li></ol></li><li><span data-ttu-id="79e43-148">Breng veldwaarden van de assemblageorderregel over naar een zojuist gemaakte, geboekte assemblageorderregel.</span><span class="sxs-lookup"><span data-stu-id="79e43-148">Transfer field values from the assembly order line into a newly created posted assembly order line.</span></span></li></ol></li><li><span data-ttu-id="79e43-149">Boek de assemblageorderkop (output):</span><span class="sxs-lookup"><span data-stu-id="79e43-149">Post the assembly order header (output):</span></span><br /><br /> <ol><li><span data-ttu-id="79e43-150">Vul velden op de artikeldagboekregel in.</span><span class="sxs-lookup"><span data-stu-id="79e43-150">Populate fields on the item journal line.</span></span></li><li><span data-ttu-id="79e43-151">Breng reserveringen over naar de artikeldagboekregel.</span><span class="sxs-lookup"><span data-stu-id="79e43-151">Transfer reservations to the item journal line.</span></span></li><li><span data-ttu-id="79e43-152">Boek de artikeldagboekregel om de artikelposten te maken.</span><span class="sxs-lookup"><span data-stu-id="79e43-152">Post the item journal line to create the item ledger entries.</span></span></li><li><span data-ttu-id="79e43-153">Maak magazijndagboekregels en boek ze.</span><span class="sxs-lookup"><span data-stu-id="79e43-153">Create warehouse journal lines and post them.</span></span></li><li><span data-ttu-id="79e43-154">Stel de assemblageaantallen en de resterende aantallen opnieuw in.</span><span class="sxs-lookup"><span data-stu-id="79e43-154">Reset the assembly quantities and remaining quantities.</span></span></li></ol></li></ol>|  

> [!IMPORTANT]  
>  <span data-ttu-id="79e43-155">In tegenstelling tot productieoutput, die wordt geboekt tegen verwachte kosten, wordt assemblyuitvoer tegen de feitelijke prijs geboekt.</span><span class="sxs-lookup"><span data-stu-id="79e43-155">Unlike for production output, which is posted at expected cost, assembly output is posted at actual cost.</span></span>  

## <a name="cost-adjustment"></a><span data-ttu-id="79e43-156">Kostenherwaardering</span><span class="sxs-lookup"><span data-stu-id="79e43-156">Cost Adjustment</span></span>  
 <span data-ttu-id="79e43-157">Zodra een assemblageorder is geboekt, wat inhoudt dat materiaal (onderdelen) en resources in een nieuw artikel worden geassembleerd, moet het mogelijk zijn om de werkelijke kosten van dat assemblageartikel en de werkelijke voorraadkosten van de betrokken onderdelen te bepalen.</span><span class="sxs-lookup"><span data-stu-id="79e43-157">Once an assembly order is posted, meaning that components (material) and resources are assembled into a new item, then it should be possible to determine the actual cost of that assembly item, and the actual inventory cost of the components involved.</span></span> <span data-ttu-id="79e43-158">Hiervoor worden kosten van de geboekte posten van de bron (de onderdelen en resources) naar de geboekte posten van het doel (de component) doorgestuurd.</span><span class="sxs-lookup"><span data-stu-id="79e43-158">This is achieved by forwarding costs from the posted entries of the source (the components and resources) to the posted entries of the destination (the assembly item).</span></span> <span data-ttu-id="79e43-159">Het doorsturen van kosten wordt uitgevoerd door het berekenen en genereren van nieuwe posten, zogenaamde herwaarderingsposten, die aan de doelposten worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="79e43-159">The forwarding of costs is done by calculating and generating new entries, called adjustment entries that become associated with the destination entries.</span></span>  

 <span data-ttu-id="79e43-160">De door te sturen assemblagekosten worden gedetecteerd met het detectiemechanisme op orderniveau.</span><span class="sxs-lookup"><span data-stu-id="79e43-160">The assembly costs to be forwarded are detected with the Order Level detection mechanism.</span></span> <span data-ttu-id="79e43-161">Zie voor informatie over andere mechanismen voor herwaarderingsdetectie [Ontwerpdetails: Kostenwaardering](design-details-cost-adjustment.md)</span><span class="sxs-lookup"><span data-stu-id="79e43-161">For information about other adjustment detection mechanisms, see [Design Details: Cost Adjustment](design-details-cost-adjustment.md).</span></span>  

### <a name="detecting-the-adjustment"></a><span data-ttu-id="79e43-162">De correctie detecteren</span><span class="sxs-lookup"><span data-stu-id="79e43-162">Detecting the Adjustment</span></span>  
<span data-ttu-id="79e43-163">De detectiefunctie op orderniveau wordt gebruikt voor conversiescenario's, productie en assemblage.</span><span class="sxs-lookup"><span data-stu-id="79e43-163">The order Level detection function is used in conversion scenarios, production and assembly.</span></span> <span data-ttu-id="79e43-164">De functie werkt als volgt:</span><span class="sxs-lookup"><span data-stu-id="79e43-164">The function works as follows:</span></span>  

-   <span data-ttu-id="79e43-165">Kostenherwaardering wordt gedetecteerd door de order te markeren telkens wanneer een materiaal/resource wordt geboekt als verbruikt/gebruikt voor de order.</span><span class="sxs-lookup"><span data-stu-id="79e43-165">Cost adjustment is detected by marking the order whenever a material/resource is posted as consumed/used.</span></span>  
-   <span data-ttu-id="79e43-166">Kosten wordt doorgestuurd door de kosten voor het materiaal/de resource toe te passen op de uitvoerposten die aan dezelfde order zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="79e43-166">Cost is forwarding by applying the costs from material/resource to the output entries associated with the same order.</span></span>  

<span data-ttu-id="79e43-167">De volgende afbeelding toont de structuur van de herwaarderingspost en hoe assemblagekosten worden aangepast.</span><span class="sxs-lookup"><span data-stu-id="79e43-167">The following graphic shows the adjustment entry structure and how assembly costs are adjusted.</span></span>  

<span data-ttu-id="79e43-168">![Structuur van herwaarderingspost](media/design_details_assembly_posting_3.png "design_details_assembly_posting_3")</span><span class="sxs-lookup"><span data-stu-id="79e43-168">![Adjustment entry structure](media/design_details_assembly_posting_3.png "design_details_assembly_posting_3")</span></span>  

### <a name="performing-the-adjustment"></a><span data-ttu-id="79e43-169">De aanpassing doorvoeren</span><span class="sxs-lookup"><span data-stu-id="79e43-169">Performing the Adjustment</span></span>  
<span data-ttu-id="79e43-170">De spreiding van gedetecteerde correcties van materiaal en resourcekosten op de assemblyuitvoerposten wordt uitgevoerd door de batchverwerking **Kostprijs herwaarderen - Artikelposten**.</span><span class="sxs-lookup"><span data-stu-id="79e43-170">The spreading of detected adjustments from material and resource costs onto the assembly output entries is performed by the **Adjust Cost – Item Entries** batch job.</span></span> <span data-ttu-id="79e43-171">Deze bevat de functie Aanpassing op meerdere niveaus aanbrengen, die bestaat uit de volgende twee elementen:</span><span class="sxs-lookup"><span data-stu-id="79e43-171">It contains the Make Multilevel Adjustment function, which consists of the following two elements:</span></span>  

-   <span data-ttu-id="79e43-172">Assemblageordercorrectie aanbrengen - hiermee worden kosten van materiaal en resourcegebruik doorgestuurd naar de assemblage-uitvoerpost.</span><span class="sxs-lookup"><span data-stu-id="79e43-172">Make Assembly Order Adjustment – which forwards cost from material and resource usage to the assembly output entry.</span></span> <span data-ttu-id="79e43-173">Regel 5 en 6 in het algoritme hieronder zijn hiervoor verantwoordelijk.</span><span class="sxs-lookup"><span data-stu-id="79e43-173">Lines 5 and 6 in the algorithm below are responsible for that.</span></span>  
-   <span data-ttu-id="79e43-174">Correcties op één niveau aanbrengen - hiermee worden kosten voor afzonderlijke artikelen doorgestuurd met behulp van de waarderingsmethode ervan.</span><span class="sxs-lookup"><span data-stu-id="79e43-174">Make Single Level Adjustments – which forwards costs for individual items using their costing method.</span></span> <span data-ttu-id="79e43-175">Regels 9 en 10 in het algoritme hieronder zijn hiervoor verantwoordelijk.</span><span class="sxs-lookup"><span data-stu-id="79e43-175">Lines 9 and 10 in the algorithm below are responsible for that.</span></span>  

<span data-ttu-id="79e43-176">![Algoritme van assemblageherwaardering](media/design_details_assembly_posting_4.jpg "design_details_assembly_posting_4")</span><span class="sxs-lookup"><span data-stu-id="79e43-176">![Assembly adjustment algorithm](media/design_details_assembly_posting_4.jpg "design_details_assembly_posting_4")</span></span>  

> [!NOTE]  
>  <span data-ttu-id="79e43-177">Het element voor het maken van OHW- herwaarderingen op regel 7 en 8 is verantwoordelijk voor het doorsturen van productiemateriaal en capaciteitsverbruik naar de output van onvoltooide productieorders.</span><span class="sxs-lookup"><span data-stu-id="79e43-177">The Make WIP Adjustments element, in lines 7 and 8, is responsible for forwarding production material and capacity usage to the output of unfinished production orders.</span></span> <span data-ttu-id="79e43-178">Dit wordt niet gebruikt bij het aanpassen van assemblageorderkosten aangezien het concept OHW niet van toepassing is op assemblage.</span><span class="sxs-lookup"><span data-stu-id="79e43-178">This is not used when adjusting assembly order costs as the concept of WIP does not apply to assembly.</span></span>  

<span data-ttu-id="79e43-179">Voor informatie over hoe kosten van assemblage en productie worden geboekt naar het grootboek raadpleegt u [Ontwerpdetails: voorraadboeking](design-details-inventory-posting.md).</span><span class="sxs-lookup"><span data-stu-id="79e43-179">For information about how costs from assembly and production are posted to the general ledger, see [Design Details: Inventory Posting](design-details-inventory-posting.md).</span></span>  

## <a name="assembly-costs-are-always-actual"></a><span data-ttu-id="79e43-180">Assemblagekosten zijn altijd werkelijk</span><span class="sxs-lookup"><span data-stu-id="79e43-180">Assembly Costs are Always Actual</span></span>  
 <span data-ttu-id="79e43-181">Het concept van onderhanden werk (OHW) geldt niet voor assemblageorderboeking.</span><span class="sxs-lookup"><span data-stu-id="79e43-181">The concept of work in process (WIP) does not apply in assembly order posting.</span></span> <span data-ttu-id="79e43-182">Assemblagekosten worden alleen geboekt als werkelijke kosten, nooit als verwachte kosten.</span><span class="sxs-lookup"><span data-stu-id="79e43-182">Assembly costs are only posted as actual cost, never as expected cost.</span></span> <span data-ttu-id="79e43-183">Zie [Ontwerpdetails: verwachte-kostenboeking](design-details-expected-cost-posting.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="79e43-183">For more information, see [Design Details: Expected Cost Posting](design-details-expected-cost-posting.md).</span></span>  

<span data-ttu-id="79e43-184">Dit wordt ingeschakeld door de volgende gegevensstructuur.</span><span class="sxs-lookup"><span data-stu-id="79e43-184">This is enabled by the following data structure.</span></span>  

-   <span data-ttu-id="79e43-185">In het veld **Soort** op artikeldagboekregels in de tabellen **Capaciteitspost** en **Waardepost** wordt *Resource* gebruikt om posten van assemblageresources te identificeren.</span><span class="sxs-lookup"><span data-stu-id="79e43-185">In the **Type** field on item journal lines, in the **Capacity Ledger Entry** and **Value Entry** tables, *Resource* is used to identify assembly resource entries.</span></span>  
-   <span data-ttu-id="79e43-186">In het veld **Artikelboekingssoort** op artikeldagboekregels in de tabellen **Capaciteitspost** en **Waardepost** worden *Assemblage-uitvoer* en *Assemblageverbruik* gebruikt om respectievelijk de artikelposten van assemblage-uitvoer en de posten van verbruikte assemblagecomponenten te identificeren.</span><span class="sxs-lookup"><span data-stu-id="79e43-186">In the **Item Ledger Entry Type** field on item journal lines, in the **Capacity Ledger Entry** and **Value Entry** tables, *Assembly Output* and *Assembly Consumption* are used to identify the output assembly item entries and the consumed assembly component entries respectively.</span></span>  

<span data-ttu-id="79e43-187">Daarnaast worden boekingsgroepsvelden in de assemblageorderkop en de assemblageorderregels standaard als volgt ingevuld.</span><span class="sxs-lookup"><span data-stu-id="79e43-187">In addition, posting group fields on the assembly order header and assembly order lines are populated by default as follows.</span></span>  

|<span data-ttu-id="79e43-188">Entiteit</span><span class="sxs-lookup"><span data-stu-id="79e43-188">Entity</span></span>|<span data-ttu-id="79e43-189">Soort</span><span class="sxs-lookup"><span data-stu-id="79e43-189">Type</span></span>|<span data-ttu-id="79e43-190">Boekingsgroep</span><span class="sxs-lookup"><span data-stu-id="79e43-190">Posting Group</span></span>|<span data-ttu-id="79e43-191">Prod.-boekingsgroep</span><span class="sxs-lookup"><span data-stu-id="79e43-191">Gen. Prod. Posting Group</span></span>|  
|------------|----------|-------------------|------------------------------|  
|<span data-ttu-id="79e43-192">Assemblageorderkop</span><span class="sxs-lookup"><span data-stu-id="79e43-192">Assembly Order Header</span></span>|<span data-ttu-id="79e43-193">Artikel</span><span class="sxs-lookup"><span data-stu-id="79e43-193">Item</span></span>|<span data-ttu-id="79e43-194">Voorraadboekingsgroep</span><span class="sxs-lookup"><span data-stu-id="79e43-194">Inventory Posting Group</span></span>|<span data-ttu-id="79e43-195">Prod.-boekingsgroep</span><span class="sxs-lookup"><span data-stu-id="79e43-195">Gen. Prod. Posting Group</span></span>|  
|<span data-ttu-id="79e43-196">Assemblageorderregel</span><span class="sxs-lookup"><span data-stu-id="79e43-196">Assembly Order Line</span></span>|<span data-ttu-id="79e43-197">Artikel</span><span class="sxs-lookup"><span data-stu-id="79e43-197">Item</span></span>|<span data-ttu-id="79e43-198">Voorraadboekingsgroep</span><span class="sxs-lookup"><span data-stu-id="79e43-198">Inventory Posting Group</span></span>|<span data-ttu-id="79e43-199">Prod.-boekingsgroep</span><span class="sxs-lookup"><span data-stu-id="79e43-199">Gen. Prod. Posting Group</span></span>|  
|<span data-ttu-id="79e43-200">Assemblageorderregel</span><span class="sxs-lookup"><span data-stu-id="79e43-200">Assembly Order Line</span></span>|<span data-ttu-id="79e43-201">Resource</span><span class="sxs-lookup"><span data-stu-id="79e43-201">Resource</span></span>||<span data-ttu-id="79e43-202">Prod.-boekingsgroep</span><span class="sxs-lookup"><span data-stu-id="79e43-202">Gen. Prod. Posting Group</span></span>|  

<span data-ttu-id="79e43-203">Alleen werkelijke kosten worden geboekt naar het grootboek en er worden geen interimrekeningen gevuld vanuit assemblageorderboeking.</span><span class="sxs-lookup"><span data-stu-id="79e43-203">Accordingly, only actual costs are posted to the general ledger, and no interim accounts are populated from assembly order posting.</span></span> <span data-ttu-id="79e43-204">Zie voor meer informatie [Ontwerpdetails: rekeningen in het grootboek](design-details-accounts-in-the-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="79e43-204">For more information, see [Design Details: Accounts in the General Ledger](design-details-accounts-in-the-general-ledger.md)</span></span>  

## <a name="assemble-to-order"></a><span data-ttu-id="79e43-205">Op order assembleren</span><span class="sxs-lookup"><span data-stu-id="79e43-205">Assemble to Order</span></span>  
<span data-ttu-id="79e43-206">De artikelpost die het resultaat is van het boeken van een op-order-assembleren-verkoop wordt vast toegepast op de bijbehorende artikelpost voor de assemblageuitvoer.</span><span class="sxs-lookup"><span data-stu-id="79e43-206">The item ledger entry that results from posting an assemble-to-order sale is fixed applied to the related item ledger entry for the assembly output.</span></span> <span data-ttu-id="79e43-207">Dienovereenkomstig, worden de kosten van een op-order-assembleren-verkoop afgeleid van de assemblageorder waaraan deze verkoop is gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="79e43-207">Accordingly, the cost of an assemble-to-order sale is derived from the assembly order that it was linked to.</span></span>  

<span data-ttu-id="79e43-208">Artikelposten van de soort Verkoop die het gevolg zijn van het boeken van op-order-assembleren aantallen, worden gemarkeerd met **Ja** in het veld **Op order assembleren**.</span><span class="sxs-lookup"><span data-stu-id="79e43-208">Item ledger entries of type Sale that result from posting assemble-to-order quantities are marked with **Yes** in the **Assemble to Order** field.</span></span>  

<span data-ttu-id="79e43-209">Bij het boeken van verkooporderregels waarbij een gedeelte afkomstig is uit voorraad en een ander gedeelte een op-order-assembleren aantal is, worden afzonderlijke artikelposten gemaakt, één voor het voorraadaantal en één voor het op-order-assembleren aantal.</span><span class="sxs-lookup"><span data-stu-id="79e43-209">Posting sales order lines where a part is inventory quantity and another part is assemble-to-order quantity results in separate item ledger entries, one for the inventory quantity and one for the assemble-to-order quantity.</span></span>  

## <a name="see-also"></a><span data-ttu-id="79e43-210">Zie ook</span><span class="sxs-lookup"><span data-stu-id="79e43-210">See Also</span></span>  
 <span data-ttu-id="79e43-211">[Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="79e43-211">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="79e43-212">[Ontwerpdetails: Productieorderboeking](design-details-production-order-posting.md) </span><span class="sxs-lookup"><span data-stu-id="79e43-212">[Design Details: Production Order Posting](design-details-production-order-posting.md) </span></span>  
 [<span data-ttu-id="79e43-213">Ontwerpdetails: Waarderingsmethoden</span><span class="sxs-lookup"><span data-stu-id="79e43-213">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)  
 [<span data-ttu-id="79e43-214">Voorraadkosten beheren</span><span class="sxs-lookup"><span data-stu-id="79e43-214">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
 [<span data-ttu-id="79e43-215">Financiën</span><span class="sxs-lookup"><span data-stu-id="79e43-215">Finance</span></span>](finance.md)  
 <span data-ttu-id="79e43-216">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="79e43-216">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
