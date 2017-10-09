---
title: Productieoutput opslaan | Microsoft Docs
description: Hoe u de productieoutput opslaat, is afhankelijk van de vestigingsinstellingen van het magazijn.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 9555f2810e82711c9cac98cfe002cb99289ce474
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-put-away-production-or-assembly-output"></a><span data-ttu-id="6e2ea-103">Procedure: Productie- of assemblageoutput opslaan</span><span class="sxs-lookup"><span data-stu-id="6e2ea-103">How to: Put Away Production or Assembly Output</span></span>
<span data-ttu-id="6e2ea-104">Hoe u de productieoutput opslaat, is afhankelijk van de vestigingsinstellingen van het magazijn.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-104">How you put away your output from production depends on how your warehouse is set up as a location.</span></span> <span data-ttu-id="6e2ea-105">Zie voor meer informatie [Magazijnbeheer instellen](warehouse-setup-warehouse.md).</span><span class="sxs-lookup"><span data-stu-id="6e2ea-105">For more information, see [Setting Up Warehouse Management](warehouse-setup-warehouse.md).</span></span>  

<span data-ttu-id="6e2ea-106">In standaardmagazijnconfiguraties waar voor uw vestiging opslagverwerking vereist is, maar ontvangstverwerking niet, gebruikt u het document **Voorraadopslag** om de opslag van productieoutput te beheren en vast te leggen.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-106">In basic warehouse configurations where the location requires put-away processing, but not receive processing, you use the **Inventory Put-away** document to organize and record the put-away of output.</span></span>  

<span data-ttu-id="6e2ea-107">In geavanceerde magazijnconfiguraties waar voor de vestiging zowel opslag- als ontvangstverwerking vereist is, kunt u een interne-opslagdocument of een verplaatsingsdocument maken om de output op te slaan.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-107">In advanced warehouse configurations where the location requires both put-away and receive processing, you create either an internal put-away document or a movement document to put away the output.</span></span>  

<span data-ttu-id="6e2ea-108">De eerste stap bij het opslaan van output is het maken van het inkomende magazijnverzoek.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-108">The first step in creating putting output away is to create the inbound warehouse request.</span></span> <span data-ttu-id="6e2ea-109">Deze aanvraag informeert het magazijn dat de output van de productie- of assemblageorder gereed is voor opslag.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-109">This request informs the warehouse that the production or assembly order output is ready to be put away.</span></span>

## <a name="to-create-the-inbound-warehouse-request"></a><span data-ttu-id="6e2ea-110">Ink.magazijnontvangst maken</span><span class="sxs-lookup"><span data-stu-id="6e2ea-110">To create the inbound warehouse request</span></span>  
1.  <span data-ttu-id="6e2ea-111">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vrijgegeven productieorder** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Released Production Order**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6e2ea-112">Kies in de productieorder die gereed is voor opslag de actie **Ink. magazijnontvangst maken**.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-112">On the production order that is ready for put-away, choose the **Create Inbound Whse. Request** action.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="6e2ea-113">U kunt de inkomende magazijnaanvraag ook maken door het selectievakje **Inkomend verzoek maken** in te schakelen bij het vernieuwen van de productieorder.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-113">You can also create the inbound warehouse request by selecting the **Create Inbound Request** check box when you refresh the production order.</span></span> <span data-ttu-id="6e2ea-114">Zie [Procedure: Productieorders vernieuwen of opnieuw plannen](production-how-to-replan-refresh-production-orders.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-114">For more information, see [How to: Refresh or Replan Production Orders](production-how-to-replan-refresh-production-orders.md).</span></span>  

## <a name="to-put-output-away-with-an-inventory-put-away"></a><span data-ttu-id="6e2ea-115">Output opslaan met een voorraadopslag</span><span class="sxs-lookup"><span data-stu-id="6e2ea-115">To put output away with an inventory put-away</span></span>  
1.  <span data-ttu-id="6e2ea-116">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Voorraadopslag** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Inventory Put-away**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6e2ea-117">Een nieuwe voorraadopslag maken.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-117">Create a new inventory put-away.</span></span> <span data-ttu-id="6e2ea-118">Zie voor meer informatie [Procedure: artikelen opslaan met een voorraadopslag](warehouse-how-to-put-items-away-with-inventory-put-aways.md).</span><span class="sxs-lookup"><span data-stu-id="6e2ea-118">For more information, see [How to: Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md).</span></span>
3.  <span data-ttu-id="6e2ea-119">Kies de actie **Brondocumenten ophalen** en selecteer de vrijgegeven productieorder om de productieorderoutput te openen.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-119">To access the production order output, choose the **Get Source Documents** action, and then select the released production order.</span></span>  
4.  <span data-ttu-id="6e2ea-120">Vul de opslagregels in.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-120">Fill in the put-away lines as appropriate.</span></span>
5.  <span data-ttu-id="6e2ea-121">Wanneer de regels gereed zijn voor boeken, kiest u de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-121">When the lines are ready for posting, choose the **Post** action.</span></span> <span data-ttu-id="6e2ea-122">Het boeken leidt tot het maken van de benodigde magazijnposten en tot het boeken van de output van de artikelen.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-122">The posting will create the necessary warehouse entries and post the output of the items.</span></span>  

<span data-ttu-id="6e2ea-123">Het is ook mogelijk om rechtstreeks vanuit een vrijgegeven productieorder een **Voorraadopslag** te maken.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-123">You can also create an **Inventory Put-away** directly from the released production order.</span></span> <span data-ttu-id="6e2ea-124">Zie voor meer informatie [Procedure: artikelen opslaan met een voorraadopslag](warehouse-how-to-put-items-away-with-inventory-put-aways.md).</span><span class="sxs-lookup"><span data-stu-id="6e2ea-124">For more information, see [How to: Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md).</span></span>  

<span data-ttu-id="6e2ea-125">Wanneer u een voorraadopslag boekt, wordt ervan uitgegaan dat alle bewerkingen worden geboekt overeenkomstig het standaardbewerkingsplan, dus dat de outputhoeveelheid wordt geboekt overeenkomstig de laatste bewerking.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-125">When you post an inventory put-away, it is assumed that all the operations are posted according to the standard routing, that is, output quantity is posted according to the last operation.</span></span> <span data-ttu-id="6e2ea-126">U kunt het outputdagboek gebruiken om verschillen in de outputhoeveelheid en de instel- en bewerkingstijd te boeken.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-126">You can use the output journal to post variances in output quantity and the setup and run times.</span></span> <span data-ttu-id="6e2ea-127">Als u een gedeeltelijke boeking moet uitvoeren nadat u de voorraadopslag hebt gemaakt, kunt u dit doen voor insteltijden en hoeveelheden voor alle bewerkingen, behalve de laatste.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-127">If it is required to post partially after you have created the inventory put-away, you can do so on setup times and quantities for all operations except the last one.</span></span> <span data-ttu-id="6e2ea-128">In dat geval wordt de laatste bewerking bestuurd door de voorraadopslag.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-128">In that case, the last operation is controlled by the inventory put-away.</span></span>  

<span data-ttu-id="6e2ea-129">Als u alleen instel- of bewerkingstijd hoeft te boeken voor de laatste bewerking, stelt u de outputhoeveelheid voor de laatste bewerking in op 0.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-129">If you only need to post setup or run time on the last operation, then set the output quantity on the last operation to 0.</span></span> <span data-ttu-id="6e2ea-130">Eventueel kunt u ervoor kiezen om de laatste regel helemaal niet te boeken door deze te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-130">Alternatively, you can choose not to post the last line at all by simply deleting it</span></span>  

## <a name="to-put-output-away-with-a-warehouse-internal-put-away"></a><span data-ttu-id="6e2ea-131">Output opslaan via interne magazijnopslag</span><span class="sxs-lookup"><span data-stu-id="6e2ea-131">To put output away with a warehouse internal put-away</span></span>
1.  <span data-ttu-id="6e2ea-132">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Interne mag.-opslag** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Whse. Internal Put-away**, and then choose the related link.</span></span>  
2. <span data-ttu-id="6e2ea-133">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-133">Choose the **New** action.</span></span>
3. <span data-ttu-id="6e2ea-134">Vul de velden op de kop van een nieuwe interne opslag in. Vermeld in ieder geval de **vestiging**.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-134">Fill in the header of a new internal put-away with at least the **Location Code**.</span></span>  
4. <span data-ttu-id="6e2ea-135">Vul voor ieder artikel dat u naar het magazijn wilt verplaatsen een regel in.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-135">Fill in a line for each item you wish to move to the warehouse.</span></span> <span data-ttu-id="6e2ea-136">U hoeft alleen de velden **Artikelnr.** en **Aantal** in te vullen.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-136">You only have to fill in the **Item No.** and the **Quantity** fields.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6e2ea-137">Wanneer u het veld **Artikelnr.** selecteert, wordt het **opslaglocatie-inhoudsoverzicht** geopend in plaats van de **artikellijst**.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-137">When you select the **Item No.** field, the **Bin Contents List** opens instead of the **Item List**.</span></span> <span data-ttu-id="6e2ea-138">Het artikel dat u wilt opslaan behoort namelijk tot de inhoud van een bepaalde opslaglocatie. Bovendien weet u al uit welke opslaglocatie het artikel moet worden gehaald.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-138">This is because you want to put away an item that is in a particular bin - a Bin Content - not just an item, and you already know the bin the item should be taken from.</span></span>  

4.  <span data-ttu-id="6e2ea-139">Kies de actie **Opslaglocatie-inhoud ophalen** om de voorstelregels te vullen met de volledige of gefilterde inhoud van de opslaglocaties in de vestiging.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-139">To fill the worksheet lines with the entire bin content or the filtered bin content of bins in the location, choose the **Get Bin Content** action.</span></span>  
5.  <span data-ttu-id="6e2ea-140">Kies de actie **Opslag maken**. De artikelen die u uit het productieproces wilt halen, worden nu opgenomen in opslaginstructies, zodat ze in het magazijn kunnen worden opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-140">Choose the **Create Put-away** action, and the items you want to move out of production are now on put-away instructions waiting to be stored in the warehouse.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="6e2ea-141">Als voor uw magazijnvestiging gestuurde opslag en pick is ingesteld, wordt het magazijn via de standaardproductieopslaglocaties gekoppeld aan de productieafdeling: de inkomende en uitgaande productieopslaglocaties en de open shopflooropslaglocatie, die u definieert op het sneltabblad **Opslaglocaties** van de vestigingskaart.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-141">When your warehouse location is set up to use directed put-away and pick, the warehouse is linked to your manufacturing facility through the default production bins: the inbound and outbound production bins and the open shop bin, all of which you define on the **Bins** FastTab of the location card.</span></span> <span data-ttu-id="6e2ea-142">Wanneer u de output van een productieorder boekt, wordt de output in de **uitgaande productieopslaglocatie** geplaatst.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-142">When you post the output of a production order, the output is placed in the **Outbound Production Bin**.</span></span> <span data-ttu-id="6e2ea-143">Volg de bovenstaande procedure om de productieoutput op te slaan. Sla de output echter niet direct op in de standaardopslaglocatie van de artikelen, maar verplaats de artikelen van de **Uitgaande productieopslaglocatie** naar de standaardopslaglocatie.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-143">You follow the same procedure as described above to put-away the production output, except that instead of using the item's default bin, you will move or put-away the items from the **Outbound Production Bin** to the item's default bin.</span></span>  

## <a name="to-manually-specify-a-bin-to-store-items-from-production-output"></a><span data-ttu-id="6e2ea-144">Handmatig een opslaglocatie opgeven voor het opslaan van artikelen uit de productieoutput</span><span class="sxs-lookup"><span data-stu-id="6e2ea-144">To manually specify a bin to store items from production output</span></span>  
1.  <span data-ttu-id="6e2ea-145">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verplaatsingsvoorstel** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Movement Worksheet**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6e2ea-146">Vul de kop in en maak een regel voor elk artikel dat u naar het magazijn wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-146">Fill in the header, and create a line for each item you wish to move to the warehouse.</span></span>  
3.  <span data-ttu-id="6e2ea-147">Vul de velden **Van opslaglocatie** en **Naar opslaglocatie** in en geef het aantal artikelen op in het veld **Aantal**.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-147">Fill in both the **From Bin Code** and the **To Bin Code** fields, and enter the quantity in the **Quantity** field.</span></span>  
4.  <span data-ttu-id="6e2ea-148">Kies de actie **Opslaglocatie-inhoud ophalen** om de voorstelregels te vullen met de volledige of gefilterde inhoud van de opslaglocaties in de vestiging.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-148">To fill the worksheet lines with the entire bin content or the filtered bin content of bins in the location, choose the **Get Bin Content** action.</span></span>  
5. <span data-ttu-id="6e2ea-149">Kies de actie **Verplaatsing maken**.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-149">Choose the **Create Movement** action.</span></span> <span data-ttu-id="6e2ea-150">Er wordt een verplaatsingsinstructie voor het magazijn gemaakt met Nemen- en Plaatsen-regels die door de magazijnmedewerkers kunnen worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-150">The warehouse movement instructions are created with Take and Place lines for warehouse employees to perform.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="6e2ea-151">In geen van beide procedures kan het brondocumentnummer, zoals Productieordernr. worden ingevoerd in de documenten interne opslag, opslag of verplaatsing.</span><span class="sxs-lookup"><span data-stu-id="6e2ea-151">You cannot enter the source document number, such as the Production Order No., in the internal put-away, put-away, or movement documents for either of these procedures.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6e2ea-152">Zie ook</span><span class="sxs-lookup"><span data-stu-id="6e2ea-152">See Also</span></span>  
[<span data-ttu-id="6e2ea-153">Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="6e2ea-153">Warehouse Management</span></span>](warehouse-manage-warehouse.md)  
[<span data-ttu-id="6e2ea-154">Voorraad</span><span class="sxs-lookup"><span data-stu-id="6e2ea-154">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="6e2ea-155">[Magazijnbeheer instellen](warehouse-setup-warehouse.md)   </span><span class="sxs-lookup"><span data-stu-id="6e2ea-155">[Setting Up Warehouse Management](warehouse-setup-warehouse.md)   </span></span>  
<span data-ttu-id="6e2ea-156">[Assemblagebeheer](assembly-assemble-items.md)  </span><span class="sxs-lookup"><span data-stu-id="6e2ea-156">[Assembly Management](assembly-assemble-items.md)  </span></span>  
[<span data-ttu-id="6e2ea-157">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="6e2ea-157">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="6e2ea-158">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6e2ea-158">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
