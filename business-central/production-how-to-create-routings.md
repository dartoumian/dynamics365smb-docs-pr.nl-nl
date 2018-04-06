---
title: Bewerkingsplannen maken | Microsoft Docs
description: Een bewerkingsplan bevat de belangrijkste gegevens met betrekking tot wat er nodig is voor het productieproces voor een bepaald geproduceerd artikel. Zodra er voor een artikel een productieorder is gemaakt, worden op basis van het bewerkingsplan ervan de bewerkingen gepland zoals weergegeven in het venster **Prod.-orderbewerkingsplan** onder de productieorder.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 0fd098170ac96b03f6f1da64b8de23b3f500c565
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="create-routings"></a><span data-ttu-id="c03d6-104">Bewerkingsplannen maken</span><span class="sxs-lookup"><span data-stu-id="c03d6-104">Create Routings</span></span>
<span data-ttu-id="c03d6-105">Productiebedrijven maken gebruik van bewerkingsplannen om het productieproces te visualiseren en aan te sturen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-105">Manufacturing companies use routings to visualize and direct the manufacturing process.</span></span>

<span data-ttu-id="c03d6-106">Een bewerkingsplan vormt de basis voor procesplanning, capaciteitsplanning, de geplande toewijzing van materiaalbehoeften en productiedocumenten.</span><span class="sxs-lookup"><span data-stu-id="c03d6-106">The routing is the basis of process scheduling, capacity scheduling, scheduled assignment of material needs, and manufacturing documents.</span></span>  

<span data-ttu-id="c03d6-107">Voor productiestuklijsten worden de bewerkingsplannen toegewezen aan het productie-eindartikel.</span><span class="sxs-lookup"><span data-stu-id="c03d6-107">As for production BOMs, the routings are assigned to the manufacturing end item.</span></span> <span data-ttu-id="c03d6-108">Een bewerkingsplan bevat de belangrijkste gegevens met betrekking tot wat er nodig is voor het productieproces voor een bepaald geproduceerd artikel.</span><span class="sxs-lookup"><span data-stu-id="c03d6-108">A routing holds master data that captures the process requirements of a given produced item.</span></span> <span data-ttu-id="c03d6-109">Zodra er voor een artikel een productieorder is gemaakt, worden op basis van het bewerkingsplan ervan de bewerkingen gepland zoals weergegeven in het venster **Prod.-orderbewerkingsplan** onder de productieorder.</span><span class="sxs-lookup"><span data-stu-id="c03d6-109">Once a production order is created for that item, its routing will govern the scheduling of operations as represented in the **Prod. Order Routing** window under the production order.</span></span>  

<span data-ttu-id="c03d6-110">Voordat u een bewerkingsplan kunt instellen, moet het volgende zijn gedaan:</span><span class="sxs-lookup"><span data-stu-id="c03d6-110">Before you can set up a routing, the following must be in place:</span></span>  

- <span data-ttu-id="c03d6-111">Er zijn artikelkaarten gemaakt voor hoofdartikelen die onderdeel zijn van de productie.</span><span class="sxs-lookup"><span data-stu-id="c03d6-111">Item cards are created for parent items that take part in manufacturing.</span></span> <span data-ttu-id="c03d6-112">Zie voor meer informatie [Nieuwe artikelen registreren](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="c03d6-112">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span>
- <span data-ttu-id="c03d6-113">Er zijn productieresources ingesteld.</span><span class="sxs-lookup"><span data-stu-id="c03d6-113">Production resources are set up.</span></span> <span data-ttu-id="c03d6-114">Zie voor meer informatie [Afdelingen en bewerkingsplaatsen instellen](production-how-to-set-up-work-and-machine-centers.md).</span><span class="sxs-lookup"><span data-stu-id="c03d6-114">For more information, see [Set Up Work Centers and Machine Centers](production-how-to-set-up-work-and-machine-centers.md).</span></span>

## <a name="to-create-a-routing"></a><span data-ttu-id="c03d6-115">Een bewerkingsplan maken</span><span class="sxs-lookup"><span data-stu-id="c03d6-115">To create a routing</span></span>  
1.  <span data-ttu-id="c03d6-116">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c03d6-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c03d6-117">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-117">Choose the **New** action.</span></span>  
3. <span data-ttu-id="c03d6-118">Vul de velden in.</span><span class="sxs-lookup"><span data-stu-id="c03d6-118">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  <span data-ttu-id="c03d6-119">Selecteer in het veld **Soort** de optie **Serieel** om bewerkingen in het productiebewerkingsplan te berekenen op basis van de waarde in het veld **Bewerkingsnr.**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-119">In the **Type** field, select **Serial** to calculate the production routing according to the value in the **Operation No.**</span></span> <span data-ttu-id="c03d6-120">te kiezen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-120">field.</span></span>   
    <span data-ttu-id="c03d6-121">Selecteer **Parallel** om de bewerkingen te berekenen op basis van de waarde in het **Volgend bewerkingsnr.**</span><span class="sxs-lookup"><span data-stu-id="c03d6-121">Select **Parallel** to calculate the operations according to the value in the **Next Operation No.**</span></span> <span data-ttu-id="c03d6-122">te kiezen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-122">field.</span></span>  
5.  <span data-ttu-id="c03d6-123">Als u het bewerkingsplan wilt bewerken, stelt u het veld **Status** in op **Nieuw** of **In ontwikkeling**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-123">To edit the routing, set the **Status** field to **New** or **Under Development**.</span></span> <span data-ttu-id="c03d6-124">Als u het wilt inschakelen, stelt u het veld **Status** in op **Gecertificeerd**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-124">To activate it, set the **Status** field to **Certified**.</span></span>  

    <span data-ttu-id="c03d6-125">Vul de bewerkingsplanregels in.</span><span class="sxs-lookup"><span data-stu-id="c03d6-125">Proceed to fill in the routing lines.</span></span>
6.  <span data-ttu-id="c03d6-126">Voer in het veld **Bewerkingsnr.**</span><span class="sxs-lookup"><span data-stu-id="c03d6-126">In the **Operation No.**</span></span> <span data-ttu-id="c03d6-127">het nummer in van de eerste bewerking in, bijvoorbeeld **10**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-127">field, enter the number of the first operation, for example,  **10**.</span></span>  
7.  <span data-ttu-id="c03d6-128">In het veld **Soort** geeft u op wat voor soort resource wordt gebruikt (bijvoorbeeld **Afdeling**).</span><span class="sxs-lookup"><span data-stu-id="c03d6-128">In the **Type** field, specify which kind of resource is used, for example, **Work Center**.</span></span>  
8.  <span data-ttu-id="c03d6-129">Selecteer in het veld **Nr.**</span><span class="sxs-lookup"><span data-stu-id="c03d6-129">In the **No.**</span></span> <span data-ttu-id="c03d6-130">de resource of typ deze resource in het veld.</span><span class="sxs-lookup"><span data-stu-id="c03d6-130">field, select the resource to be used, or type it in the field.</span></span>  
9.  <span data-ttu-id="c03d6-131">In het veld **Bewerkingsplankoppeling** voert u een code in om het onderdeel aan een bepaalde bewerking te koppelen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-131">In the **Routing Link Code** field, enter a code to connect the component to a specific operation.</span></span> <span data-ttu-id="c03d6-132">Zie de sectie Bewerkingsplankoppelingen maken voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c03d6-132">For more information, see the "To create routing links" section.</span></span>
10.  <span data-ttu-id="c03d6-133">Geef in de velden **Bewerkingstijd** en **Insteltijd** de verwerkingstijden op die nodig zijn voor de uitvoering van de bewerking.</span><span class="sxs-lookup"><span data-stu-id="c03d6-133">In the **Run Time** and **Setup Time** fields, enter the process times needed to perform the operation.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="c03d6-134">De insteltijd wordt per productieorder berekend en de bewerkingstijd per geproduceerd artikel.</span><span class="sxs-lookup"><span data-stu-id="c03d6-134">Setup time is calculated per production order, whereas run time is calculated per produced item.</span></span>  

11.  <span data-ttu-id="c03d6-135">Geef in het veld **Gelijktijdige capaciteit** op hoeveel eenheden van de geselecteerde resource worden gebruikt om de bewerking uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="c03d6-135">In the **Concurrent Capacities** field, specify how many units of the selected resource are used to perform the operation.</span></span> <span data-ttu-id="c03d6-136">Bij toewijzing van twee personen aan één verpakkingsbewerking wordt de bewerkingstijd bijvoorbeeld gehalveerd</span><span class="sxs-lookup"><span data-stu-id="c03d6-136">For example, two people allocated to one packing operation will halve the run time.</span></span>  
12.  <span data-ttu-id="c03d6-137">Ga door met het invullen van de regels voor alle bewerkingen die betrokken zijn bij de productie van het desbetreffende artikel.</span><span class="sxs-lookup"><span data-stu-id="c03d6-137">Continue to fill in lines for all operations involved in producing the item in question.</span></span>  
13.  <span data-ttu-id="c03d6-138">Als u regels wilt kopiëren uit een bestaand bewerkingsplan, kiest u de actie **Bewerkingsplan kopiëren** om bestaande regels te selecteren.</span><span class="sxs-lookup"><span data-stu-id="c03d6-138">To copy lines from an existing routing, choose the **Copy Routing** action to select existing lines.</span></span>  
14. <span data-ttu-id="c03d6-139">Certificeer het bewerkingsplan.</span><span class="sxs-lookup"><span data-stu-id="c03d6-139">Certify the routing.</span></span>  
15. <span data-ttu-id="c03d6-140">U kunt nu het nieuwe bewerkingsplan aan de kaart van het desbetreffende productieartikel koppelen door het veld **Bew.-plannr.** in te vullen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-140">You can now attach the new routing to the card of the production item in question, by filling in the **Routing No.** field.</span></span> <span data-ttu-id="c03d6-141">Zie voor meer informatie [Nieuwe artikelen registreren](inventory-how-register-new-items.md).</span><span class="sxs-lookup"><span data-stu-id="c03d6-141">For more information, see [Register New Items](inventory-how-register-new-items.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="c03d6-142">Zorg ervoor dat u de vaste verrekenprijs van het artikel opnieuw berekent vanuit de kaart **Artikel**: kies hiervoor achtereenvolgens de acties **Productie**, **Vaste verrekenprijs berekenen** en **Alle niveaus**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-142">Remember also to recalculate the item’s standard cost from the **Item** card: Choose the **Manufacturing** action, select the **Calc. Standard Cost** action, and then select the **All Levels** action.</span></span>  

## <a name="to-create-routing-links"></a><span data-ttu-id="c03d6-143">Bewerkingsplankoppelingen maken</span><span class="sxs-lookup"><span data-stu-id="c03d6-143">To create routing links</span></span>
<span data-ttu-id="c03d6-144">Met bewerkingsplankoppelingen kunt u materialen zodanig aan bepaalde bewerkingen koppelen dat hun relatie behouden blijft ook al wordt de productiestuklijst of het bewerkingsplan gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="c03d6-144">You can create routing links to connect components to specific operations in order to retain their relationship even though the production BOM or routing is modified.</span></span> <span data-ttu-id="c03d6-145">Ook kunnen hierdoor gemakkelijker materialen nog op het laatste moment worden afgeboekt, namelijk op het moment dat de specifieke gekoppelde bewerking wordt opgestart in plaats van wanneer de gehele productieorder wordt vrijgegeven.</span><span class="sxs-lookup"><span data-stu-id="c03d6-145">It also facilitates just-in-time flushing of components, namely when the specific linked operation starts, not when the complete production order is released.</span></span> <span data-ttu-id="c03d6-146">Zie voor meer informatie [Materialen afboeken op basis van de uitvoer van een bewerking](production-how-to-flush-components-according-to-operation-output.md).</span><span class="sxs-lookup"><span data-stu-id="c03d6-146">For more information see [Flush Components According to Operation Output](production-how-to-flush-components-according-to-operation-output.md).</span></span>  

<span data-ttu-id="c03d6-147">Een ander belangrijk voordeel van het koppelen van materialen en bewerkingen is dat beide elementen in een logische processtructuur worden weergegeven wanneer u het venster **Productiedagboek** gebruikt voor het boeken van output en verbruik.</span><span class="sxs-lookup"><span data-stu-id="c03d6-147">Another important benefit is that linked components and operations are displayed in a logical process structure when you use the **Production Journal** window for output and consumption posting.</span></span>  

1.  <span data-ttu-id="c03d6-148">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c03d6-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c03d6-149">Open het bewerkingsplan dat de bewerkingen bevat die moeten worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="c03d6-149">Open the routing that contains the operations that you want to link.</span></span>  

    <span data-ttu-id="c03d6-150">Controleer of de status van het bewerkingsplan **In ontwikkeling** is.</span><span class="sxs-lookup"><span data-stu-id="c03d6-150">Make sure the routing status is **Under Development**.</span></span>  

3.  <span data-ttu-id="c03d6-151">Op de desbetreffende bewerkingsplanregel in de **Bewerkingsplankoppeling** selecteert u een code.</span><span class="sxs-lookup"><span data-stu-id="c03d6-151">On the relevant routing line, in the **Routing Link Code** field, select a code.</span></span>  
4.  <span data-ttu-id="c03d6-152">Voeg in het bewerkingsplan desgewenst nog andere koppelingen toe aan andere bewerkingen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-152">Proceed to add different routing link codes to other operations in the routing, if relevant.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="c03d6-153">U kunt het beste niet meer dan één bewerking in een bewerkingsplan koppelen om te voorkomen dat u per ongeluk hetzelfde materiaal aan twee verschillende bewerkingen koppelt, zodat het tweemaal wordt verbruikt.</span><span class="sxs-lookup"><span data-stu-id="c03d6-153">You should not use the same routing link code in different operations on a routing because you may incorrectly link a component to two different operations, so that it is consumed two times.</span></span>  
    >   
    >  <span data-ttu-id="c03d6-154">Het is aan te raden om de bewerkingsplankoppeling dezelfde naam te geven als de bewerking zelf om er zeker van te zijn dat materialen maar aan één bewerking worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="c03d6-154">It is a good idea to name the routing link code after the operation in order to ensure operation-specific routing links.</span></span>

5.  <span data-ttu-id="c03d6-155">Stel de status van het bewerkingsplan in op **Gecertificeerd**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-155">Set the routing status to **Certified**.</span></span>  

    <span data-ttu-id="c03d6-156">Nu worden bewerkingsplankoppelingen aan bewerkingen toegewezen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-156">Routing link codes are now assigned to operations.</span></span> <span data-ttu-id="c03d6-157">Vervolgens moet u de feitelijke koppeling maken door dezelfde codes toe te wijzen aan bepaalde materialen in de desbetreffende productiestuklijst.</span><span class="sxs-lookup"><span data-stu-id="c03d6-157">Next, you must create the actual link by assigning the same codes to specific components in the relevant production BOM.</span></span>  

6.  <span data-ttu-id="c03d6-158">Open de **productiestuklijst** met de onderdelen die aan de bovenstaande bewerkingen moeten worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="c03d6-158">Open the **Production BOM** that contains the components that you want to link to the above operations.</span></span> <span data-ttu-id="c03d6-159">Zie voor meer informatie [Productiestuklijsten maken](production-how-to-create-production-boms.md).</span><span class="sxs-lookup"><span data-stu-id="c03d6-159">For more information, see [Create Production BOMs](production-how-to-create-production-boms.md).</span></span>
7.  <span data-ttu-id="c03d6-160">Controleer of de status van de stuklijst **In ontwikkeling** is.</span><span class="sxs-lookup"><span data-stu-id="c03d6-160">Make sure the BOM status is **Under Development**.</span></span>  
8.  <span data-ttu-id="c03d6-161">Op de regel van de desbetreffende productiestuklijst in het veld **Bewerkingsplankoppeling** selecteert u de code die u zojuist hebt toegewezen aan de desbetreffende bewerking.</span><span class="sxs-lookup"><span data-stu-id="c03d6-161">On the relevant production BOM line, in the **Routing Link Code** field, select the code that you have just assigned to the relevant operation.</span></span>  
9. <span data-ttu-id="c03d6-162">Ga door met het toevoegen van materialen aan unieke bewerkingen waar dat nodig is.</span><span class="sxs-lookup"><span data-stu-id="c03d6-162">Proceed to add routing link codes to other components according to the unique operations where they are used.</span></span>  
10. <span data-ttu-id="c03d6-163">Stel de status van de productiestuklijst in op **Gecertificeerd**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-163">Set the production BOM status to **Certified**.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="c03d6-164">In een bestaande productieorder kunnen de bewerkingsplankoppelingen pas worden gebruikt nadat u die order hebt vernieuwd.</span><span class="sxs-lookup"><span data-stu-id="c03d6-164">To enable the routing links on an existing production order, you must refresh the productio1n order.</span></span> <span data-ttu-id="c03d6-165">Zie voor meer informatie [Productieorders maken](production-how-to-create-production-orders.md).</span><span class="sxs-lookup"><span data-stu-id="c03d6-165">For more information, see [Create Production Orders](production-how-to-create-production-orders.md).</span></span>  

<span data-ttu-id="c03d6-166">De geselecteerde materialen worden gekoppeld aan de geselecteerde bewerkingen zodra u een productieorder maakt of vernieuwt met behulp van de desbetreffende productiestuklijst en het desbetreffende bewerkingsplan.</span><span class="sxs-lookup"><span data-stu-id="c03d6-166">The selected components will now be linked to the selected operations when you create or refresh a production order using the production BOM and routing in question.</span></span> <span data-ttu-id="c03d6-167">Dit is in het venster **Prod.-ordermaterialen** te zien onder de productieorder. In dit venster kunt u ook op elk moment bewerkingsplankoppelingen verwijderen en toevoegen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-167">This is visible in the **Prod. Order Components** window under the production order, and here you can also remove and add the defined routing link codes at any time.</span></span>

## <a name="to-assign-personnel-tools-and-quality-measures-to-routing-operations"></a><span data-ttu-id="c03d6-168">Medewerkers, tools en kwaliteitsmetingen toewijzen aan bewerkingsplannen</span><span class="sxs-lookup"><span data-stu-id="c03d6-168">To assign personnel, tools, and quality measures to routing operations.</span></span>
<span data-ttu-id="c03d6-169">Als u voor een bewerking medewerkers met speciale kwalificaties, speciale kennis of speciale autorisaties nodig hebt, kunt u deze medewerkers toewijzen aan de bewerking.</span><span class="sxs-lookup"><span data-stu-id="c03d6-169">If you require personnel with qualifications, special knowledge, or special authorization for an operation, you can assign these personnel to the operation.</span></span> <span data-ttu-id="c03d6-170">Daarnaast kunt u tools en kwaliteitsvereisten toewijzen aan de bewerking.</span><span class="sxs-lookup"><span data-stu-id="c03d6-170">In addition, you can assign tools and quality requirements to the operation.</span></span> <span data-ttu-id="c03d6-171">In deze procedure wordt beschreven hoe u personeel toewijst.</span><span class="sxs-lookup"><span data-stu-id="c03d6-171">This procedure describes how to assign personnel.</span></span> <span data-ttu-id="c03d6-172">De stappen zijn vergelijkbaar voor andere soorten bewerkinginformatie.</span><span class="sxs-lookup"><span data-stu-id="c03d6-172">The steps are similar for other types of operation information.</span></span>

1.  <span data-ttu-id="c03d6-173">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c03d6-173">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c03d6-174">Open het betreffende bewerkingsplan.</span><span class="sxs-lookup"><span data-stu-id="c03d6-174">Open the relevant routing.</span></span>  
3.  <span data-ttu-id="c03d6-175">Op het sneltabblad **Regels** selecteert u de regel die u wilt verwerken en vervolgens kiest u de actie **Medewerkers**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-175">On the **Lines** FastTab, select the line that you want to process, and then choose the **Personnel** action.</span></span>  
4.  <span data-ttu-id="c03d6-176">Vul de velden in het venster **Medewerkers bewerkingsplan** in.</span><span class="sxs-lookup"><span data-stu-id="c03d6-176">Fill in the fields in the **Routing Personnel** window.</span></span>  
5.  <span data-ttu-id="c03d6-177">Kies de knop **OK** om het venster te verlaten.</span><span class="sxs-lookup"><span data-stu-id="c03d6-177">Choose the **OK** button to exit the window.</span></span> <span data-ttu-id="c03d6-178">De ingevoerde waarden worden gekopieerd en toegewezen aan de bewerking.</span><span class="sxs-lookup"><span data-stu-id="c03d6-178">The entered values are copied and assigned to the operation.</span></span>    

## <a name="to-create-a-new-versions-of-a-routing"></a><span data-ttu-id="c03d6-179">Nieuwe versies maken van bewerkingsplannen</span><span class="sxs-lookup"><span data-stu-id="c03d6-179">To create a new versions of a routing</span></span>  
<span data-ttu-id="c03d6-180">Het versieprincipe stelt u in staat verschillende versies van een bewerkingsplan te beheren.</span><span class="sxs-lookup"><span data-stu-id="c03d6-180">The version principle enables you to manage several versions of a routing.</span></span> <span data-ttu-id="c03d6-181">De structuur van de bewerkingsplanversie komt overeen met de structuur van het bewerkingsplan: een bewerkingsplanversiekop en -regels.</span><span class="sxs-lookup"><span data-stu-id="c03d6-181">The structure of the routing version corresponds to the structure of the routing consisting of the routing version header and the routing version lines.</span></span> <span data-ttu-id="c03d6-182">Het belangrijkste verschil wordt bepaald door de begindatum.</span><span class="sxs-lookup"><span data-stu-id="c03d6-182">The basic difference is defined by the starting date.</span></span>  

1.  <span data-ttu-id="c03d6-183">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bewerkingsplannen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c03d6-183">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Routings**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c03d6-184">Selecteer het bewerkingsplan dat u wilt kopiëren en kies de actie **Versies**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-184">Select the routing to be copied, and then choose the **Versions** action.</span></span>  
3. <span data-ttu-id="c03d6-185">Kies in het venster **Bewerkingsplanversies** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-185">In the **Routing Versions** window, choose the **New** action.</span></span>
4. <span data-ttu-id="c03d6-186">Vul de velden in.</span><span class="sxs-lookup"><span data-stu-id="c03d6-186">Fill in the fields as necessary.</span></span>
5.  <span data-ttu-id="c03d6-187">Voer in het veld **Versiecode** de unieke identificatie van de versie in.</span><span class="sxs-lookup"><span data-stu-id="c03d6-187">In the **Version Code** field, enter the unique identification of the version.</span></span> <span data-ttu-id="c03d6-188">Alle combinaties van cijfers en letters zijn toegestaan.</span><span class="sxs-lookup"><span data-stu-id="c03d6-188">Any combination of numbers and letters is permitted.</span></span>  

    <span data-ttu-id="c03d6-189">De nieuwe versie krijgt automatisch de status **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-189">The newly created version is automatically assigned the status **New**.</span></span>  
6.  <span data-ttu-id="c03d6-190">Als u bewerkingsregels wilt maken, selecteert u de eerste lege regel en vult u bij **Bewerkingsnr.** de waarde</span><span class="sxs-lookup"><span data-stu-id="c03d6-190">To create operation lines, select the first blank line, and then fill in the **Operation No.**</span></span> <span data-ttu-id="c03d6-191">in die overeenkomt met de volgorde van de bewerkingen.</span><span class="sxs-lookup"><span data-stu-id="c03d6-191">field according to the sequence of operations.</span></span>

    <span data-ttu-id="c03d6-192">De bewerkingsregels worden in oplopende volgorde gesorteerd op bewerkingsnummers.</span><span class="sxs-lookup"><span data-stu-id="c03d6-192">The operation lines are sorted in ascending order by operation numbers.</span></span> <span data-ttu-id="c03d6-193">Als u later nog wijzigingen of toevoegingen wilt maken, is het raadzaam dat u tussen iedere stap voldoende ruimte voor tussenstappen laat.</span><span class="sxs-lookup"><span data-stu-id="c03d6-193">To be able to make changes later, we recommend you to select adequate step widths.</span></span> <span data-ttu-id="c03d6-194">Het veld **Volgend bewerkingsnr.**</span><span class="sxs-lookup"><span data-stu-id="c03d6-194">The **Next Operation No.**</span></span> <span data-ttu-id="c03d6-195">verwijst naar de volgende bewerking.</span><span class="sxs-lookup"><span data-stu-id="c03d6-195">field refers to the following operation.</span></span> <span data-ttu-id="c03d6-196">Het nummer van de bewerking kan rechtstreeks worden ingevoerd.</span><span class="sxs-lookup"><span data-stu-id="c03d6-196">The number of the operation can be entered directly.</span></span>

7. <span data-ttu-id="c03d6-197">Wanneer de bewerkingsplanversie is voltooid, wordt het veld **Status** ingesteld op **Gecertificeerd**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-197">When the routing version is completed, setting the **Status** field to **Certified**.</span></span>

<span data-ttu-id="c03d6-198">De geldigheid van de versie wordt aangegeven in het veld **Begindatum**.</span><span class="sxs-lookup"><span data-stu-id="c03d6-198">The time validity of the version is specified by the **Starting Date** field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c03d6-199">Zie ook</span><span class="sxs-lookup"><span data-stu-id="c03d6-199">See Also</span></span>  
[<span data-ttu-id="c03d6-200">Productiestuklijsten maken</span><span class="sxs-lookup"><span data-stu-id="c03d6-200">Create Production BOMs</span></span>](production-how-to-create-production-boms.md)  
[<span data-ttu-id="c03d6-201">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="c03d6-201">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="c03d6-202">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="c03d6-202">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
<span data-ttu-id="c03d6-203">[Gepland](production-planning.md) </span><span class="sxs-lookup"><span data-stu-id="c03d6-203">[Planning](production-planning.md) </span></span>  
[<span data-ttu-id="c03d6-204">Voorraad</span><span class="sxs-lookup"><span data-stu-id="c03d6-204">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="c03d6-205">Inkoop</span><span class="sxs-lookup"><span data-stu-id="c03d6-205">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="c03d6-206">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c03d6-206">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
