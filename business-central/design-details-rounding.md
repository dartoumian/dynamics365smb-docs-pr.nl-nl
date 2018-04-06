---
title: Ontwerpdetails - Afronding | Microsoft Docs
description: Afrondingsverschillen kunnen optreden wanneer u de kosten waardeert van een negatieve voorraadmutatie die in een andere hoeveelheid wordt gemeten dan de overeenkomende positieve voorraadmutatie. Afrondingsverschillen worden berekend voor alle waarderingsmethoden wanneer u de batchverwerking **Kostprijs herwaarderen - Artikelposten** uitvoert.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 231481ed9b8de81fb565e86e9b89c96434545cbf
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-rounding"></a><span data-ttu-id="2e83b-104">Ontwerpdetails: Afronding</span><span class="sxs-lookup"><span data-stu-id="2e83b-104">Design Details: Rounding</span></span>
<span data-ttu-id="2e83b-105">Afrondingsverschillen kunnen optreden wanneer u de kosten waardeert van een negatieve voorraadmutatie die in een andere hoeveelheid wordt gemeten dan de overeenkomende positieve voorraadmutatie.</span><span class="sxs-lookup"><span data-stu-id="2e83b-105">Rounding residuals can occur when you value the cost of an inventory decrease that is measured in a different quantity than the corresponding inventory increase.</span></span> <span data-ttu-id="2e83b-106">Afrondingsverschillen worden berekend voor alle waarderingsmethoden wanneer u de batchverwerking **Kostprijs herwaarderen - Artikelposten** uitvoert.</span><span class="sxs-lookup"><span data-stu-id="2e83b-106">Rounding residuals are calculated for all costing methods when you run the **Adjust Cost - Item Entries** batch job.</span></span>  

 <span data-ttu-id="2e83b-107">Wanneer u de waarderingsmethode Gemiddeld gebruikt, wordt het afrondingsverschil berekend en vastgelegd op een cumulatieve post-per-post-basis.</span><span class="sxs-lookup"><span data-stu-id="2e83b-107">When you use the average costing method, the rounding residual is calculated and recorded on a cumulative, entry-by-entry basis.</span></span>  

 <span data-ttu-id="2e83b-108">Als u een andere waarderingsmethode dan Gemiddeld gebruikt, wordt het afrondingsverschil berekend wanneer de voorraadtoename volledig is vereffend, oftewel wanneer het resterende aantal voor de voorraadtoename gelijk is aan nul.</span><span class="sxs-lookup"><span data-stu-id="2e83b-108">When you use a costing method other than Average, the rounding residual is calculated when the inventory increase has been fully applied, that is when the remaining quantity for the inventory increase is equal to zero.</span></span> <span data-ttu-id="2e83b-109">Vervolgens is een afzonderlijke post gemaakt voor het afrondingsverschil en de boekingsdatum van deze afrondingspost is de boekingsdatum van de laatst gefactureerde waardepost van de positieve voorraadmutatie.</span><span class="sxs-lookup"><span data-stu-id="2e83b-109">A separate entry is then created for the rounding residual, and the posting date on this rounding entry is the posting date of the last invoiced value entry of the inventory increase.</span></span>  

## <a name="example"></a><span data-ttu-id="2e83b-110">Opmerking</span><span class="sxs-lookup"><span data-stu-id="2e83b-110">Example</span></span>  
 <span data-ttu-id="2e83b-111">In het volgende voorbeeld ziet u hoe de verschillende afrondingsverschillen voor respectievelijk de gemiddelde waarderingsmethode en de niet-gemiddelde waarderingsmethode worden verwerkt.</span><span class="sxs-lookup"><span data-stu-id="2e83b-111">The following example illustrates how different rounding residuals are handled for the average costing method and non-Average costing method, respectively.</span></span> <span data-ttu-id="2e83b-112">In beide gevallen is de batchverwerking **Kostprijs herwaarderen - Artikelposten** uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="2e83b-112">In both cases, the **Adjust Cost - Item Entries** batch job has been run.</span></span>  

 <span data-ttu-id="2e83b-113">De volgende tabel toont de artikelposten waarop het voorbeeld is gebaseerd.</span><span class="sxs-lookup"><span data-stu-id="2e83b-113">The following table shows the item ledger entries that the example is based on.</span></span>  

|<span data-ttu-id="2e83b-114">Boekingsdatum</span><span class="sxs-lookup"><span data-stu-id="2e83b-114">Posting Date</span></span>|<span data-ttu-id="2e83b-115">Aantal</span><span class="sxs-lookup"><span data-stu-id="2e83b-115">Quantity</span></span>|<span data-ttu-id="2e83b-116">Volgnummer</span><span class="sxs-lookup"><span data-stu-id="2e83b-116">Entry No.</span></span>|  
|------------------|--------------|---------------|  
|<span data-ttu-id="2e83b-117">01-01-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-117">01-01-20</span></span>|<span data-ttu-id="2e83b-118">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-118">3</span></span>|<span data-ttu-id="2e83b-119">1</span><span class="sxs-lookup"><span data-stu-id="2e83b-119">1</span></span>|  
|<span data-ttu-id="2e83b-120">01-02-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-120">02-01-20</span></span>|<span data-ttu-id="2e83b-121">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-121">-1</span></span>|<span data-ttu-id="2e83b-122">2</span><span class="sxs-lookup"><span data-stu-id="2e83b-122">2</span></span>|  
|<span data-ttu-id="2e83b-123">01-03-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-123">03-01-20</span></span>|<span data-ttu-id="2e83b-124">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-124">-1</span></span>|<span data-ttu-id="2e83b-125">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-125">3</span></span>|  
|<span data-ttu-id="2e83b-126">01-04-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-126">04-01-20</span></span>|<span data-ttu-id="2e83b-127">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-127">-1</span></span>|<span data-ttu-id="2e83b-128">4</span><span class="sxs-lookup"><span data-stu-id="2e83b-128">4</span></span>|  

 <span data-ttu-id="2e83b-129">Voor een artikel dat de waarderingsmethode Gemiddeld gebruikt, wordt de afrondingsrest (1/300) berekend met de eerste vermindering (postnummer 2) en vervolgens overgedragen aan postnummer 3.</span><span class="sxs-lookup"><span data-stu-id="2e83b-129">For an item using the Average costing method, the rounding residual (1/300) is calculated with the first decrease (entry number 2) and is carried forward to entry number 3.</span></span> <span data-ttu-id="2e83b-130">Daarom wordt volgnummer 3 gewaardeerd op 3 – 3,34.</span><span class="sxs-lookup"><span data-stu-id="2e83b-130">Therefore, entry number 3 is valued at –3.34.</span></span>  

 <span data-ttu-id="2e83b-131">De volgende tabel toont de twee soorten resulterende waardeposten.</span><span class="sxs-lookup"><span data-stu-id="2e83b-131">The following table shows the resulting value entries.</span></span>  

|<span data-ttu-id="2e83b-132">Boekingsdatum</span><span class="sxs-lookup"><span data-stu-id="2e83b-132">Posting Date</span></span>|<span data-ttu-id="2e83b-133">Aantal</span><span class="sxs-lookup"><span data-stu-id="2e83b-133">Quantity</span></span>|<span data-ttu-id="2e83b-134">Tot. werk. kosten</span><span class="sxs-lookup"><span data-stu-id="2e83b-134">Cost Amount (Actual)</span></span>|<span data-ttu-id="2e83b-135">Artikelpostnr.</span><span class="sxs-lookup"><span data-stu-id="2e83b-135">Item Ledger Entry No.</span></span>|<span data-ttu-id="2e83b-136">Volgnummer</span><span class="sxs-lookup"><span data-stu-id="2e83b-136">Entry No.</span></span>|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|<span data-ttu-id="2e83b-137">01-01-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-137">01-01-20</span></span>|<span data-ttu-id="2e83b-138">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-138">3</span></span>|<span data-ttu-id="2e83b-139">10</span><span class="sxs-lookup"><span data-stu-id="2e83b-139">10</span></span>|<span data-ttu-id="2e83b-140">1</span><span class="sxs-lookup"><span data-stu-id="2e83b-140">1</span></span>|<span data-ttu-id="2e83b-141">1</span><span class="sxs-lookup"><span data-stu-id="2e83b-141">1</span></span>|  
|<span data-ttu-id="2e83b-142">01-02-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-142">02-01-20</span></span>|<span data-ttu-id="2e83b-143">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-143">-1</span></span>|<span data-ttu-id="2e83b-144">-3,33</span><span class="sxs-lookup"><span data-stu-id="2e83b-144">-3.33</span></span>|<span data-ttu-id="2e83b-145">2</span><span class="sxs-lookup"><span data-stu-id="2e83b-145">2</span></span>|<span data-ttu-id="2e83b-146">2</span><span class="sxs-lookup"><span data-stu-id="2e83b-146">2</span></span>|  
|<span data-ttu-id="2e83b-147">01-03-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-147">03-01-20</span></span>|<span data-ttu-id="2e83b-148">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-148">-1</span></span>|<span data-ttu-id="2e83b-149">-3,34</span><span class="sxs-lookup"><span data-stu-id="2e83b-149">-3.34</span></span>|<span data-ttu-id="2e83b-150">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-150">3</span></span>|<span data-ttu-id="2e83b-151">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-151">3</span></span>|  
|<span data-ttu-id="2e83b-152">01-04-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-152">04-01-20</span></span>|<span data-ttu-id="2e83b-153">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-153">-1</span></span>|<span data-ttu-id="2e83b-154">-3,33</span><span class="sxs-lookup"><span data-stu-id="2e83b-154">-3.33</span></span>|<span data-ttu-id="2e83b-155">4</span><span class="sxs-lookup"><span data-stu-id="2e83b-155">4</span></span>|<span data-ttu-id="2e83b-156">4</span><span class="sxs-lookup"><span data-stu-id="2e83b-156">4</span></span>|  

 <span data-ttu-id="2e83b-157">Voor een artikel waarvoor u een andere waarderingsmethode dan Gemiddelde gebruikt, wordt het afrondingsrestant (0,01) berekend wanneer het resterende aantal voor de voorraadtoename nul is.</span><span class="sxs-lookup"><span data-stu-id="2e83b-157">For an item using a costing method other than Average, the rounding residual (0.01) is calculated when the remaining quantity for the inventory increase is zero.</span></span> <span data-ttu-id="2e83b-158">Het afrondingsverschil heeft een afzonderlijke post (nummer 5).</span><span class="sxs-lookup"><span data-stu-id="2e83b-158">The rounding residual has a separate entry (number 5).</span></span>  

 <span data-ttu-id="2e83b-159">De volgende tabel toont de twee soorten resulterende waardeposten.</span><span class="sxs-lookup"><span data-stu-id="2e83b-159">The following table shows the resulting value entries.</span></span>  

|<span data-ttu-id="2e83b-160">Boekingsdatum</span><span class="sxs-lookup"><span data-stu-id="2e83b-160">Posting Date</span></span>|<span data-ttu-id="2e83b-161">Aantal</span><span class="sxs-lookup"><span data-stu-id="2e83b-161">Quantity</span></span>|<span data-ttu-id="2e83b-162">Tot. werk. kosten</span><span class="sxs-lookup"><span data-stu-id="2e83b-162">Cost Amount (Actual)</span></span>|<span data-ttu-id="2e83b-163">Artikelpostnr.</span><span class="sxs-lookup"><span data-stu-id="2e83b-163">Item Ledger Entry No.</span></span>|<span data-ttu-id="2e83b-164">Volgnummer</span><span class="sxs-lookup"><span data-stu-id="2e83b-164">Entry No.</span></span>|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|<span data-ttu-id="2e83b-165">01-01-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-165">01-01-20</span></span>|<span data-ttu-id="2e83b-166">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-166">3</span></span>|<span data-ttu-id="2e83b-167">10</span><span class="sxs-lookup"><span data-stu-id="2e83b-167">10</span></span>|<span data-ttu-id="2e83b-168">1</span><span class="sxs-lookup"><span data-stu-id="2e83b-168">1</span></span>|<span data-ttu-id="2e83b-169">1</span><span class="sxs-lookup"><span data-stu-id="2e83b-169">1</span></span>|  
|<span data-ttu-id="2e83b-170">01-02-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-170">02-01-20</span></span>|<span data-ttu-id="2e83b-171">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-171">-1</span></span>|<span data-ttu-id="2e83b-172">-3,33</span><span class="sxs-lookup"><span data-stu-id="2e83b-172">-3.33</span></span>|<span data-ttu-id="2e83b-173">2</span><span class="sxs-lookup"><span data-stu-id="2e83b-173">2</span></span>|<span data-ttu-id="2e83b-174">2</span><span class="sxs-lookup"><span data-stu-id="2e83b-174">2</span></span>|  
|<span data-ttu-id="2e83b-175">01-03-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-175">03-01-20</span></span>|<span data-ttu-id="2e83b-176">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-176">-1</span></span>|<span data-ttu-id="2e83b-177">-3,33</span><span class="sxs-lookup"><span data-stu-id="2e83b-177">-3.33</span></span>|<span data-ttu-id="2e83b-178">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-178">3</span></span>|<span data-ttu-id="2e83b-179">3</span><span class="sxs-lookup"><span data-stu-id="2e83b-179">3</span></span>|  
|<span data-ttu-id="2e83b-180">01-04-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-180">04-01-20</span></span>|<span data-ttu-id="2e83b-181">-1</span><span class="sxs-lookup"><span data-stu-id="2e83b-181">-1</span></span>|<span data-ttu-id="2e83b-182">-3,33</span><span class="sxs-lookup"><span data-stu-id="2e83b-182">-3.33</span></span>|<span data-ttu-id="2e83b-183">4</span><span class="sxs-lookup"><span data-stu-id="2e83b-183">4</span></span>|<span data-ttu-id="2e83b-184">4</span><span class="sxs-lookup"><span data-stu-id="2e83b-184">4</span></span>|  
|<span data-ttu-id="2e83b-185">01-01-20</span><span class="sxs-lookup"><span data-stu-id="2e83b-185">01-01-20</span></span>|<span data-ttu-id="2e83b-186">0</span><span class="sxs-lookup"><span data-stu-id="2e83b-186">0</span></span>|<span data-ttu-id="2e83b-187">-0,01</span><span class="sxs-lookup"><span data-stu-id="2e83b-187">-0.01</span></span>|<span data-ttu-id="2e83b-188">1</span><span class="sxs-lookup"><span data-stu-id="2e83b-188">1</span></span>|<span data-ttu-id="2e83b-189">5</span><span class="sxs-lookup"><span data-stu-id="2e83b-189">5</span></span>|  

## <a name="see-also"></a><span data-ttu-id="2e83b-190">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2e83b-190">See Also</span></span>  
 <span data-ttu-id="2e83b-191">[Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="2e83b-191">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="2e83b-192">[Ontwerpdetails: Kostenwaardering](design-details-cost-adjustment.md) </span><span class="sxs-lookup"><span data-stu-id="2e83b-192">[Design Details: Cost Adjustment](design-details-cost-adjustment.md) </span></span>  
 <span data-ttu-id="2e83b-193">[Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md) [Voorraadkosten beheren](finance-manage-inventory-costs.md)</span><span class="sxs-lookup"><span data-stu-id="2e83b-193">[Design Details: Costing Methods](design-details-costing-methods.md) [Managing Inventory Costs](finance-manage-inventory-costs.md)</span></span>  
 [<span data-ttu-id="2e83b-194">Financiën</span><span class="sxs-lookup"><span data-stu-id="2e83b-194">Finance</span></span>](finance.md)  
 <span data-ttu-id="2e83b-195">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2e83b-195">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
