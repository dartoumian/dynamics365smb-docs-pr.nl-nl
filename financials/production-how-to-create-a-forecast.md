---
title: Een productieprognose maken | Microsoft Docs
description: U kunt verkoop- en productieprognoses maken in het venster **Productieprognose**.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5dea483395e64eb0635879b5c8821428512481ba
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-create-a-production-forecast"></a><span data-ttu-id="fc6e3-103">Procedure: Een productieprognose maken</span><span class="sxs-lookup"><span data-stu-id="fc6e3-103">How to: Create a Production Forecast</span></span>
<span data-ttu-id="fc6e3-104">U kunt verkoop- en productieprognoses maken in het venster **Productieprognose**.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-104">You can create sales and production forecasts with the **Production Forecast** window.</span></span>  

<span data-ttu-id="fc6e3-105">De prognosefunctionaliteit wordt gebruikt om een verwachte vraag aan te maken; de werkelijke vraag komt voort uit verkoop- en productieorders.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-105">Forecasting functionality is used to create anticipated demand; actual demand is created from sales and production orders.</span></span> <span data-ttu-id="fc6e3-106">Tijdens het opstellen van het MPS (Master Production Schedule) wordt de prognose tot een nettowaarde teruggebracht tegen de verkoop- en productieorders.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-106">During creation of the Master Production Schedule (MPS), the forecast is netted against the sales and production orders.</span></span> <span data-ttu-id="fc6e3-107">De optie *Onderdeel* op de prognose bepaalt met welke soort vraag rekening wordt gehouden in het proces van het berekenen van de nettowaarde.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-107">The *Component* option on the forecast determines which type of requirements to take into consideration in the netting process.</span></span> <span data-ttu-id="fc6e3-108">Als de prognose wordt uitgevoerd voor een verkoopartikel, worden alleen verkooporders gebruikt tegen de prognose.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-108">If the forecast is for a sales item, only sales orders net the forecast.</span></span> <span data-ttu-id="fc6e3-109">Als het materialen betreft, wordt alleen afhankelijke vraag van productieordermaterialen gebruikt tegen de prognose.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-109">If it is for components, only dependent demand from production order components net the forecast.</span></span>  

<span data-ttu-id="fc6e3-110">Met behulp van prognoses kan uw bedrijf "wat als"-scenario's opstellen en efficiënt en kosteneffectief plannen voor en voorzien in de vraag.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-110">Forecasting allows your company to create "what if" scenarios and efficiently and cost-effectively plan for and meet demand.</span></span> <span data-ttu-id="fc6e3-111">Nauwkeurige prognoses kunnen een doorslaggevend verschil maken voor de klanttevredenheid met betrekking tot ordertoezeggingsdatums en tijdige levering.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-111">Accurate forecasting can make a critical difference in customer satisfaction levels with regard to order promising dates and on-time delivery.</span></span>  

## <a name="sales-forecasts-and-production-forecasts"></a><span data-ttu-id="fc6e3-112">Verkoopprognoses en productieprognoses</span><span class="sxs-lookup"><span data-stu-id="fc6e3-112">Sales Forecasts and Production Forecasts</span></span>  
<span data-ttu-id="fc6e3-113">De prognosefunctionaliteit in het programma kan worden gebruikt voor het maken van verkoop- of productieprognoses, in combinatie of onafhankelijk van elkaar.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-113">The forecasting functionality in the program can be used to create sales or production forecasts, in combination or independently.</span></span> <span data-ttu-id="fc6e3-114">De meeste bedrijven die op order produceren, houden bijvoorbeeld geen voorraad eindproducten aan, omdat elk artikel op bestelling wordt geproduceerd.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-114">For example, most make-to-order companies don't carry finished goods inventory, because each item is produced when it is ordered.</span></span> <span data-ttu-id="fc6e3-115">Het vooruitlopen op orders (verkoopprognoses) is van essentieel belang voor een redelijke doorlooptijd van eindproducten (productieprognoses).</span><span class="sxs-lookup"><span data-stu-id="fc6e3-115">Anticipating orders (sales forecasting) is critical for a reasonable turnaround time on the finished goods (production forecasting).</span></span> <span data-ttu-id="fc6e3-116">Zo kunnen bijvoorbeeld onderdelen met een lange levertijd de productie vertragen als deze niet besteld of in voorraad zijn.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-116">As an example, component parts with lengthy delivery times, if not on order or on inventory, can delay production.</span></span>  

-   <span data-ttu-id="fc6e3-117">De verkoopprognose is de beste schatting die de verkoopafdeling kan maken over toekomstige verkopen, en deze wordt gespecificeerd per artikel en per periode.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-117">The sales forecast is the sales department's best guess at what will be sold in the future, and is specified by item and by period.</span></span> <span data-ttu-id="fc6e3-118">De verkoopprognose is echter niet altijd voldoende voor de productie.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-118">However, the sales forecast is not always adequate for production.</span></span>  
-   <span data-ttu-id="fc6e3-119">De productieprognose is de inschatting van de productieplanner van het aantal eindartikelen en afgeleide subassemblageartikelen in specifieke perioden moeten worden geproduceerd om te voldoen aan de voorspelde verkopen.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-119">The production forecast is the production planner's projection of how many end items and derived subassemblies to produce in specific periods to meet the forecasted sales.</span></span>  

<span data-ttu-id="fc6e3-120">In de meeste gevallen wijzigt dus de productieplanner de verkoopprognose zodat deze past bij de productieomstandigheden, terwijl toch aan de verkoopprognose wordt voldaan.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-120">In most cases, then, the production planner modifies the sales forecast to fit the conditions of production, yet still satisfies the sales forecast.</span></span>  

<span data-ttu-id="fc6e3-121">U kunt handmatig prognoses maken in het venster **Productieprognose**.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-121">You create forecasts manually in the **Production Forecast** window.</span></span> <span data-ttu-id="fc6e3-122">Er kunnen in het systeem meerdere prognoses bestaan, die aan de hand van de naam en de soort van elkaar worden onderscheiden.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-122">Multiple forecasts can exist in the system, and are differentiated by name and type.</span></span> <span data-ttu-id="fc6e3-123">Prognoses kunnen desgewenst worden gekopieerd en bewerkt.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-123">Forecasts can be copied and edited as necessary.</span></span> <span data-ttu-id="fc6e3-124">Het is wel zo dat op elk moment slechts één prognose geldig kan zijn voor planningsdoeleinden.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-124">Note that only one forecast is valid for planning purposes at a time.</span></span>  

<span data-ttu-id="fc6e3-125">De prognose bestaat uit een aantal records, die elk het artikelnummer, de prognosedatum en het prognoseaantal bevatten.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-125">The forecast consists of a number of records each stating item number, forecast date, and forecasted quantity.</span></span> <span data-ttu-id="fc6e3-126">De prognose van een artikel bestrijkt een periode, die wordt bepaald door de prognosedatum en de prognosedatum van de volgende (latere) prognoserecord.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-126">The forecast of an item covers a period, which is defined by the forecast date and the forecast date of the next (later) forecast record.</span></span> <span data-ttu-id="fc6e3-127">Vanuit het oogpunt van planning moet het prognoseaantal beschikbaar zijn bij aanvang van de vraagperiode.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-127">From a planning point of view, the forecasted quantity should be available at the start of the demand period.</span></span>  

<span data-ttu-id="fc6e3-128">Een prognose moet worden aangeduid als *Verkoopartikel*, *Materiaal* of *Beide*.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-128">You must designate a forecast as *Sales Item*, *Component*, or *Both*.</span></span> <span data-ttu-id="fc6e3-129">De prognosesoort *Verkoopartikel* wordt gebruikt voor verkoopprognoses.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-129">The forecast type *Sales Item* is used for sales forecasting.</span></span> <span data-ttu-id="fc6e3-130">De productieprognose wordt gemaakt met behulp van de soort *Onderdeel*.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-130">The production forecast is created using the *Component* type.</span></span> <span data-ttu-id="fc6e3-131">De prognosesoort *Beide* wordt alleen gebruikt om de planner een overzicht te geven van zowel de verkoopprognose als de productieprognose.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-131">The forecast type *Both* is only used to give the planner an overview of both the sales forecast and the production forecast.</span></span> <span data-ttu-id="fc6e3-132">Bij deze optie kunnen de prognoseposten niet worden bewerkt.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-132">With this option, the forecast entries are not editable.</span></span> <span data-ttu-id="fc6e3-133">Door deze prognosesoorten hier aan te duiden kunt u hetzelfde werkblad gebruiken voor het invoeren van een verkoopprognose als u doet bij een productieprognose, en kunt u hetzelfde blad gebruiken om beide prognoses tegelijkertijd te bekijken.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-133">By designating these forecast types here, you can use the same worksheet to enter a sales forecast as you do a production forecast, and use the same sheet to view both forecasts simultaneously.</span></span> <span data-ttu-id="fc6e3-134">Het is wel zo dat het systeem de verschillende inputs (verkoop en productie) verschillend gebruikt bij het berekenen van de planning, gebaseerd op artikel, productie en productie-instellingen.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-134">Note that the system treats the different inputs (sales and production) differently when calculating planning, based on item, manufacturing, and production setup.</span></span>  

## <a name="component-forecast"></a><span data-ttu-id="fc6e3-135">Materiaalprognose</span><span class="sxs-lookup"><span data-stu-id="fc6e3-135">Component Forecast</span></span>  
<span data-ttu-id="fc6e3-136">De materiaalprognose kan worden beschouwd als een optieprognose in relatie tot een hoofdartikel.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-136">The component forecast can be seen as an option forecast in relation to a parent item.</span></span> <span data-ttu-id="fc6e3-137">Dit kan bijvoorbeeld nuttig zijn als de planner de vraag naar het materiaal kan schatten.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-137">This can, for example, be useful if the planner can estimate the demand for the component.</span></span>  

<span data-ttu-id="fc6e3-138">Omdat de materiaalprognose is ontworpen om opties te definiëren voor een hoofdartikel, moet de materiaalprognose gelijk aan of kleiner zijn dan het prognoseaantal van het verkoopartikel.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-138">As the component forecast is designed to define options for a parent item, the component forecast should be equal or less than the sales item forecast quantity.</span></span> <span data-ttu-id="fc6e3-139">Als de materiaalprognose hoger is dan de verkoopartikelprognose, beschouwt het systeem het verschil tussen deze twee soorten prognoses als onafhankelijke vraag.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-139">If the component forecast is higher than the sales item forecast, the system treats the difference between these two types of forecast as independent demand.</span></span>  

## <a name="forecasting-periods"></a><span data-ttu-id="fc6e3-140">Prognoseperioden</span><span class="sxs-lookup"><span data-stu-id="fc6e3-140">Forecasting Periods</span></span>  
 <span data-ttu-id="fc6e3-141">De prognoseperiode is geldig vanaf de begindatum tot de datum waarop de volgende prognose begint.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-141">The forecast period is valid from its starting date until the date the next forecast starts.</span></span> <span data-ttu-id="fc6e3-142">Het tijdsintervalvenster biedt u meerdere keuzemogelijkheden om de vraag op en bepaalde datum in een periode in te voegen.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-142">The time interval window gives you multiple choices to insert the demand at a specific date in a period.</span></span> <span data-ttu-id="fc6e3-143">Het is daarom raadzaam om het bereik van de prognoseperiode niet te wijzigen, tenzij u alle prognoseposten naar de begindatum van deze periode wilt verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-143">It is therefore recommended not to change the forecast period scope unless you want to move all forecast entries to the starting date of this period.</span></span>  

## <a name="forecast-by-locations"></a><span data-ttu-id="fc6e3-144">Prognose per locatie</span><span class="sxs-lookup"><span data-stu-id="fc6e3-144">Forecast by Locations</span></span>  
<span data-ttu-id="fc6e3-145">Dit kan worden geconfigureerd in de productie-instellingen.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-145">It can be stated in the manufacturing setup if.</span></span> <span data-ttu-id="fc6e3-146">Het is wel zo dat indien op locatie gebaseerde prognoses los van elkaar worden bekeken, de totale prognose mogelijk niet representatief is.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-146">Note, though, that if location-based forecasts are viewed in isolation, the overall forecast may not be representative.</span></span>

## <a name="to-create-a-production-forecast"></a><span data-ttu-id="fc6e3-147">Een productieprognose maken</span><span class="sxs-lookup"><span data-stu-id="fc6e3-147">To create a production forecast</span></span>

1.  <span data-ttu-id="fc6e3-148">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Productieprognose** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-148">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Production Forecast**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="fc6e3-149">Selecteer op het sneltabblad **Algemeen** een prognose in het veld **Prod.-prognose**.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-149">On the **General** FastTab, select a forecast in the **Production Forecast Name** field.</span></span> <span data-ttu-id="fc6e3-150">Meerdere prognoses zijn mogelijk: deze zijn van elkaar te onderscheiden door de naam en het prognosetype.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-150">Multiple forecasts can exist and are differentiated by name and forecast type.</span></span>  
3.  <span data-ttu-id="fc6e3-151">Selecteer in het veld **Vestigingsfilter** de vestiging waarop deze prognose van toepassing is.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-151">In the **Location Filter** field, select the location to which this forecast will apply.</span></span>  
4.  <span data-ttu-id="fc6e3-152">Selecteer in het veld **Prognosesoort** **Verkoopartikel**, **Component** of **Beide**.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-152">In the **Forecast Type** field, select **Sales Item**,  **Component**, or **Both**.</span></span> <span data-ttu-id="fc6e3-153">Als u **Verkoopartikel** of **Component** selecteert, kunt u het aantal per periode bewerken.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-153">If you select **Sales Item** or **Component**, then you can edit the quantity by period.</span></span> <span data-ttu-id="fc6e3-154">Als u **Beide** selecteert, kunt u het aantal niet bewerken, maar wel de knop met de pijl omlaag kiezen om de posten voor de productieprognose weer te geven.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-154">If you select **Both**, then you cannot edit the quantity, but you can choose the drop-down arrow button and view the production forecast entries.</span></span>  
5.  <span data-ttu-id="fc6e3-155">Geef een **datumfilter** op als u de hoeveelheid gegevens die wordt weergegeven wilt beperken.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-155">Specify a **Date Filter** if you want to limit the amount of data displayed.</span></span>  
6.  <span data-ttu-id="fc6e3-156">Op het sneltabblad **Matrix voor productieprognose** kunt u de voorspelde aantallen **Verkoopartikelen** of de **Materiaalprognose** voor de verschillende perioden opgeven.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-156">On the **Production Forecast Matrix** FastTab, enter the forecasted quantities of **Sales Item** or **Component** forecast for the various periods.</span></span>  
7.  <span data-ttu-id="fc6e3-157">Op het sneltabblad **Matrixopties** stelt u het tijdsinterval in het veld **Weergeven per** in, waarmee u de weergegeven periode per kolom kunt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-157">On the **Matrix Options** FastTab, set the time interval in the **View by** field to change the period that is displayed in each column.</span></span> <span data-ttu-id="fc6e3-158">U kunt kiezen uit de volgende intervallen: **Dag**, **Week**, **Maand**, **Kwartaal**, **Jaar** of de **Boekingsperiode**, zoals ingesteld in Financieel beheer.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-158">You can select from the following intervals: **Day**, **Week**, **Month**, **Quarter**, **Year**, or the **Accounting Period**, as set up in Financial Management.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="fc6e3-159">Bedenk goed welk tijdsinterval u wilt gebruiken voor toekomstige prognoses, zodat u steeds dezelfde tijdsinterval gebruikt.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-159">You should consider which time interval that you want to use for future forecasts so that the time interval is consistent throughout.</span></span> <span data-ttu-id="fc6e3-160">Wanneer u een voorspeld aantal invoert, is dast geldig vanaf de eerste dag van het door u geselecteerde tijdsinterval.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-160">When you enter a forecast quantity, it is valid on the first day of the time interval that you select.</span></span> <span data-ttu-id="fc6e3-161">Als u bijvoorbeeld een maand selecteert, voert u het voorspelde aantal op de eerste dag van de maand in.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-161">For example, if you select a month, then you enter the forecast quantity on the first day of the month.</span></span> <span data-ttu-id="fc6e3-162">Als u een kwartaal selecteert, voert u het voorspelde aantal op de eerste dag van de eerste maand van het kwartaal in.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-162">If you select a quarter, then you enter the forecast quantity on the first day of the first month in the quarter.</span></span>  

8.  <span data-ttu-id="fc6e3-163">Selecteer in het veld **Weergeven als** hoe de voorspelde aantallen voor het tijdsinterval moeten worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-163">In the **View as** field, select how the forecast quantities are shown for the time interval.</span></span> <span data-ttu-id="fc6e3-164">Als u **Mutatie** selecteert, wordt de mutatie in het saldo weergegeven voor het tijdsinterval.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-164">If you select **Net Change**, then the net change in balance is displayed for the time interval.</span></span> <span data-ttu-id="fc6e3-165">Als u **Saldo t/m datum** selecteert, wordt in het venster het saldo van de laatste dag van het tijdsinterval weergegeven.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-165">If you select **Balance at Date**, then the window displays the balance as of the last day in the time interval.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="fc6e3-166">U kunt ook een bestaande prognose bewerken.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-166">You can also edit an existing forecast.</span></span> <span data-ttu-id="fc6e3-167">Kies in het venster **Matrix voor productieprognose** de actie **Prod.-prognose kopiëren** en vul het venster **Prod.-prognose** met een bestaande prognose.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-167">In the **Production Forecast Matrix** window, choose the **Copy Production Forecast** action and populate the **Production Forecast** window with an existing forecast.</span></span> <span data-ttu-id="fc6e3-168">U kunt de aantallen waar nodig wijzigen.</span><span class="sxs-lookup"><span data-stu-id="fc6e3-168">You can then edit quantities as appropriate.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fc6e3-169">Zie ook</span><span class="sxs-lookup"><span data-stu-id="fc6e3-169">See Also</span></span>  
[<span data-ttu-id="fc6e3-170">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="fc6e3-170">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="fc6e3-171">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="fc6e3-171">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
[<span data-ttu-id="fc6e3-172">Voorraad</span><span class="sxs-lookup"><span data-stu-id="fc6e3-172">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="fc6e3-173">Inkoop</span><span class="sxs-lookup"><span data-stu-id="fc6e3-173">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="fc6e3-174">[Ontwerpdetails: Voorzieningsplanning](design-details-supply-planning.md) </span><span class="sxs-lookup"><span data-stu-id="fc6e3-174">[Design Details: Supply Planning](design-details-supply-planning.md) </span></span>  
[<span data-ttu-id="fc6e3-175">Aanbevolen procedures instellen: voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="fc6e3-175">Setup Best Practices: Supply Planning</span></span>](setup-best-practices-supply-planning.md)  
<span data-ttu-id="fc6e3-176">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="fc6e3-176">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
