---
title: Ontwerpdetails - Verschil | Microsoft Docs
description: Verschil wordt gedefinieerd als het verschil tussen de werkelijke kosten en de vaste verrekenprijs, zoals in de volgende formule wordt beschreven.
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
ms.openlocfilehash: 04faa28799288e272da93c60cbb90fa19fd190f0
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="design-details-variance"></a><span data-ttu-id="401f1-103">Ontwerpdetails: Verschil</span><span class="sxs-lookup"><span data-stu-id="401f1-103">Design Details: Variance</span></span>
<span data-ttu-id="401f1-104">Verschil wordt gedefinieerd als het verschil tussen de werkelijke kosten en de vaste verrekenprijs, zoals in de volgende formule wordt beschreven.</span><span class="sxs-lookup"><span data-stu-id="401f1-104">Variance is defined as the difference between the actual cost and the standard cost, as described in the following formula.</span></span>  

 <span data-ttu-id="401f1-105">werkelijke kosten – standaardkosten = verschil</span><span class="sxs-lookup"><span data-stu-id="401f1-105">actual cost – standard cost = variance</span></span>  

 <span data-ttu-id="401f1-106">Als de werkelijke kosten veranderen, bijvoorbeeld omdat u een artikeltoeslag boekt op een latere datum, wordt het verschil overeenkomstig bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="401f1-106">If the actual cost changes, for example, because you post an item charge on a later date, then the variance is updated accordingly.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="401f1-107">Herwaardering heeft geen invloed op de verschilberekening, omdat herwaardering alleen de voorraadwaarde wijzigt.</span><span class="sxs-lookup"><span data-stu-id="401f1-107">Revaluation does not affect the variance calculation, because revaluation only changes the inventory value.</span></span>  

## <a name="example"></a><span data-ttu-id="401f1-108">Opmerking</span><span class="sxs-lookup"><span data-stu-id="401f1-108">Example</span></span>  
 <span data-ttu-id="401f1-109">In het volgende voorbeeld ziet u hoe het verschil wordt berekend voor aangeschafte artikelen.</span><span class="sxs-lookup"><span data-stu-id="401f1-109">The following example illustrates how variance is calculated for purchased items.</span></span> <span data-ttu-id="401f1-110">Het is gebaseerd op het volgende scenario:</span><span class="sxs-lookup"><span data-stu-id="401f1-110">It is based on the following scenario:</span></span>  

1.  <span data-ttu-id="401f1-111">De gebruiker koopt een artikel tegen LV 90,00, maar de vaste verrekenprijs is LV 100,00.</span><span class="sxs-lookup"><span data-stu-id="401f1-111">The user purchases an item at LCY 90.00, but the standard cost is LCY 100.00.</span></span> <span data-ttu-id="401f1-112">Het inkoopverschil is dus LV -10,00.</span><span class="sxs-lookup"><span data-stu-id="401f1-112">Accordingly, the purchase variance is LCY –10.00.</span></span>  
2.  <span data-ttu-id="401f1-113">LV 10,00 wordt gecrediteerd naar de inkoopverschillenrekening.</span><span class="sxs-lookup"><span data-stu-id="401f1-113">LCY 10.00 is credited to the purchase variance account.</span></span>  
3.  <span data-ttu-id="401f1-114">De gebruiker boekt een artikeltoeslag van LV 20,00.</span><span class="sxs-lookup"><span data-stu-id="401f1-114">The user posts an item charge of LCY 20.00.</span></span> <span data-ttu-id="401f1-115">De werkelijke kosten worden verhoogd tot LV 110,00 en de waarde van het inkoopverschil wordt LV 10,00.</span><span class="sxs-lookup"><span data-stu-id="401f1-115">Accordingly, the actual cost is increased to LCY 110.00, and the value of the purchase variance becomes LCY 10.00.</span></span>  
4.  <span data-ttu-id="401f1-116">LV 20,00 wordt gedebiteerd naar de inkoopverschillenrekening.</span><span class="sxs-lookup"><span data-stu-id="401f1-116">LCY 20.00 is debited to the purchase variance account.</span></span> <span data-ttu-id="401f1-117">Het netto-inkoopverschil wordt LV 10,00.</span><span class="sxs-lookup"><span data-stu-id="401f1-117">Accordingly, the net purchase variance becomes LCY 10.00.</span></span>  
5.  <span data-ttu-id="401f1-118">De gebruiker herwaardeert het artikel van LV 100,00 naar LV 70,00.</span><span class="sxs-lookup"><span data-stu-id="401f1-118">The user revalues the item from LCY 100.00 to LCY 70.00.</span></span> <span data-ttu-id="401f1-119">Dit heeft geen invloed op de verschilberekening, alleen op de voorraadwaarde.</span><span class="sxs-lookup"><span data-stu-id="401f1-119">This does not affect the variance calculation, only the inventory value.</span></span>  

 <span data-ttu-id="401f1-120">De volgende tabel toont de twee soorten resulterende waardeposten.</span><span class="sxs-lookup"><span data-stu-id="401f1-120">The following table shows the resulting value entries.</span></span>  

 <span data-ttu-id="401f1-121">![Berekening van het inkoopverschil](media/design_details_inventory_costing_11_purchase_variance.png "design_details_inventory_costing_11_purchase_variance")</span><span class="sxs-lookup"><span data-stu-id="401f1-121">![Purchase variance calculation](media/design_details_inventory_costing_11_purchase_variance.png "design_details_inventory_costing_11_purchase_variance")</span></span>  

## <a name="determining-the-standard-cost"></a><span data-ttu-id="401f1-122">De standaardkosten bepalen</span><span class="sxs-lookup"><span data-stu-id="401f1-122">Determining the Standard Cost</span></span>  
 <span data-ttu-id="401f1-123">De vaste verrekenprijs wordt gebruikt bij het berekenen van het te kapitaliseren verschil en aantal.</span><span class="sxs-lookup"><span data-stu-id="401f1-123">The standard cost is used when calculating variance and the amount to capitalize.</span></span> <span data-ttu-id="401f1-124">Aangezien de vaste verrekenprijs na verloop van tijd kan worden gewijzigd als gevolg van handmatige updateberekeningen, hebt u een tijdstip nodig waarop de vaste verrekenprijs wordt vastgesteld voor verschilberekening.</span><span class="sxs-lookup"><span data-stu-id="401f1-124">Since the standard cost can be changed over time because of manual update calculation, you need a point in time when the standard cost is fixed for variance calculation.</span></span> <span data-ttu-id="401f1-125">Dit punt is wanneer de voorraadtoename wordt gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="401f1-125">This point is when the inventory increase is invoiced.</span></span> <span data-ttu-id="401f1-126">Voor geproduceerde of geassembleerde artikelen worden standaardkosten bepaald wanneer de kosten worden gewaardeerd.</span><span class="sxs-lookup"><span data-stu-id="401f1-126">For produced or assembled items, the point when standard cost is determined is when the cost is adjusted.</span></span>  

 <span data-ttu-id="401f1-127">De volgende tabel toont hoe verschillende kostenaandelen worden gegenereerd voor geproduceerde en geassembleerde artikelen als u de functie Vaste verrekenprijs berekenen gebruikt.</span><span class="sxs-lookup"><span data-stu-id="401f1-127">The following table shows how different cost shares are calculated for produced and assembled items when you use the Calculate Standard Cost function.</span></span>  

|<span data-ttu-id="401f1-128">Aandeel kosten</span><span class="sxs-lookup"><span data-stu-id="401f1-128">Cost Share</span></span>|<span data-ttu-id="401f1-129">Ingekocht artikel</span><span class="sxs-lookup"><span data-stu-id="401f1-129">Purchased Item</span></span>|<span data-ttu-id="401f1-130">Geproduceerd/geassembleerd artikel</span><span class="sxs-lookup"><span data-stu-id="401f1-130">Produced/Assembled Item</span></span>|  
|----------------|--------------------|------------------------------|  
|<span data-ttu-id="401f1-131">**Vaste verrekenprijs**</span><span class="sxs-lookup"><span data-stu-id="401f1-131">**Standard Cost**</span></span>||<span data-ttu-id="401f1-132">Materiaalkosten (één niveau) + Capaciteitskosten (één niveau) + Uitbestedingskosten (één niveau) + Cap.-overheadkosten (één niveau) + Prod.-overheadkosten (één niveau)</span><span class="sxs-lookup"><span data-stu-id="401f1-132">Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost + Single-Level Cap. Ovhd. Cost + Single-Level Mfg. Ovhd. Cost</span></span>|  
|<span data-ttu-id="401f1-133">**Materiaalkosten (Eén niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-133">**Single-Level Material Cost**</span></span>|<span data-ttu-id="401f1-134">Kostprijs</span><span class="sxs-lookup"><span data-stu-id="401f1-134">Unit Cost</span></span>|<span data-ttu-id="401f1-135">![Vergelijking 1](media/design_details_inventory_costing_11_equation_1.png "design_details_inventory_costing_11_equation_1")</span><span class="sxs-lookup"><span data-stu-id="401f1-135">![Equation 1](media/design_details_inventory_costing_11_equation_1.png "design_details_inventory_costing_11_equation_1")</span></span>|  
|<span data-ttu-id="401f1-136">**Capaciteitskosten (Eén niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-136">**Single-Level Capacity Cost**</span></span>|<span data-ttu-id="401f1-137">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-137">Not applicable</span></span>|<span data-ttu-id="401f1-138">![Vergelijking 2](media/design_details_inventory_costing_11_equation_2.png "design_details_inventory_costing_11_equation_2")</span><span class="sxs-lookup"><span data-stu-id="401f1-138">![Equation 2](media/design_details_inventory_costing_11_equation_2.png "design_details_inventory_costing_11_equation_2")</span></span>|  
|<span data-ttu-id="401f1-139">**Uitbestedingskosten (Eén niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-139">**Single-Level Subcontrd. Cost**</span></span>|<span data-ttu-id="401f1-140">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-140">Not applicable</span></span>|<span data-ttu-id="401f1-141">![Vergelijking 3](media/design_details_inventory_costing_11_equation_3.png "design_details_inventory_costing_11_equation_3")</span><span class="sxs-lookup"><span data-stu-id="401f1-141">![Equation 3](media/design_details_inventory_costing_11_equation_3.png "design_details_inventory_costing_11_equation_3")</span></span>|  
|<span data-ttu-id="401f1-142">**Cap.-overheadkosten (Eén niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-142">**Single-Level Cap. Ovhd Cost**</span></span>|<span data-ttu-id="401f1-143">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-143">Not applicable</span></span>|<span data-ttu-id="401f1-144">![Vergelijking 4](media/design_details_inventory_costing_11_equation_4.png "design_details_inventory_costing_11_equation_4")</span><span class="sxs-lookup"><span data-stu-id="401f1-144">![Equation 4](media/design_details_inventory_costing_11_equation_4.png "design_details_inventory_costing_11_equation_4")</span></span>|  
|<span data-ttu-id="401f1-145">**Prod.-overheadkosten. (Eén niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-145">**Single-Level Mfg. Ovhd Cost**</span></span>|<span data-ttu-id="401f1-146">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-146">Not applicable</span></span>|<span data-ttu-id="401f1-147">(Materiaalkosten (één niveau) + Capaciteitskosten (één niveau) + Uitbestedingskosten (één niveau)) * Indirecte kosten % / 100 + Overheadtarief</span><span class="sxs-lookup"><span data-stu-id="401f1-147">(Single-Level Material Cost + Single-Level Capacity Cost + Single-Level Subcontrd. Cost) * Indirect Cost % / 100 + Overhead Rate</span></span>|  
|<span data-ttu-id="401f1-148">**Materiaalkosten (Alle niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-148">**Rolled-up Material Cost**</span></span>|<span data-ttu-id="401f1-149">Kostprijs</span><span class="sxs-lookup"><span data-stu-id="401f1-149">Unit Cost</span></span>|<span data-ttu-id="401f1-150">![Vergelijking 5](media/design_details_inventory_costing_11_equation_5.png "design_details_inventory_costing_11_equation_5")</span><span class="sxs-lookup"><span data-stu-id="401f1-150">![Equation 5](media/design_details_inventory_costing_11_equation_5.png "design_details_inventory_costing_11_equation_5")</span></span>|  
|<span data-ttu-id="401f1-151">**Capaciteitskosten (Alle niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-151">**Rolled-up Capacity Cost**</span></span>|<span data-ttu-id="401f1-152">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-152">Not applicable</span></span>|<span data-ttu-id="401f1-153">![Vergelijking 6](media/design_details_inventory_costing_11_equation_6.png "design_details_inventory_costing_11_equation_6")</span><span class="sxs-lookup"><span data-stu-id="401f1-153">![Equation 6](media/design_details_inventory_costing_11_equation_6.png "design_details_inventory_costing_11_equation_6")</span></span>|  
|<span data-ttu-id="401f1-154">**Uitbestedingskosten (Alle niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-154">**Rolled-Up Subcontracted Cost**</span></span>|<span data-ttu-id="401f1-155">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-155">Not applicable</span></span>|<span data-ttu-id="401f1-156">![Vergelijking 7](media/design_details_inventory_costing_11_equation_7.png "design_details_inventory_costing_11_equation_7")</span><span class="sxs-lookup"><span data-stu-id="401f1-156">![Equation 7](media/design_details_inventory_costing_11_equation_7.png "design_details_inventory_costing_11_equation_7")</span></span>|  
|<span data-ttu-id="401f1-157">**Samengevouwen capaciteitsoverheadkosten**</span><span class="sxs-lookup"><span data-stu-id="401f1-157">**Rolled-up Capacity Ovhd. Cost**</span></span>|<span data-ttu-id="401f1-158">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-158">Not applicable</span></span>|<span data-ttu-id="401f1-159">![Vergelijking 8](media/design_details_inventory_costing_11_equation_8.png "design_details_inventory_costing_11_equation_8")</span><span class="sxs-lookup"><span data-stu-id="401f1-159">![Equation 8](media/design_details_inventory_costing_11_equation_8.png "design_details_inventory_costing_11_equation_8")</span></span>|  
|<span data-ttu-id="401f1-160">**Prod.-overheadkosten (Alle niv.)**</span><span class="sxs-lookup"><span data-stu-id="401f1-160">**Rolled-up Mfg. Ovhd. Cost**</span></span>|<span data-ttu-id="401f1-161">Niet van toepassing</span><span class="sxs-lookup"><span data-stu-id="401f1-161">Not applicable</span></span>|<span data-ttu-id="401f1-162">![Vergelijking 9](media/design_details_inventory_costing_11_equation_9.png "design_details_inventory_costing_11_equation_9")</span><span class="sxs-lookup"><span data-stu-id="401f1-162">![Equation 9](media/design_details_inventory_costing_11_equation_9.png "design_details_inventory_costing_11_equation_9")</span></span>|  

## <a name="see-also"></a><span data-ttu-id="401f1-163">Zie ook</span><span class="sxs-lookup"><span data-stu-id="401f1-163">See Also</span></span>  
 <span data-ttu-id="401f1-164">[Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="401f1-164">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="401f1-165">[Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md) [Voorraadkosten beheren](finance-manage-inventory-costs.md)</span><span class="sxs-lookup"><span data-stu-id="401f1-165">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span></span>  
 [<span data-ttu-id="401f1-166">Financiën</span><span class="sxs-lookup"><span data-stu-id="401f1-166">Finance</span></span>](finance.md)  
 <span data-ttu-id="401f1-167">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="401f1-167">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
