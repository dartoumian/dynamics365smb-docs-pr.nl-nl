---
title: 'Ontwerpdetails: Prioriteit geven aan orders | Microsoft Docs'
description: Lees hoe u prioriteiten stelt om aan de vereisten van vraag en aanbod te voldoen.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, priority, prioritize, order, sku, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 6e09ad64750493f99210d47516410d8471a83011
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-prioritizing-orders"></a><span data-ttu-id="38ae7-103">Ontwerpdetails: Prioriteit geven aan orders</span><span class="sxs-lookup"><span data-stu-id="38ae7-103">Design Details: Prioritizing Orders</span></span>
<span data-ttu-id="38ae7-104">Binnen een bepaalde SKU staat de verzochte of beschikbare datum voor de hoogste prioriteit; de vraag van vandaag moet worden verwerkt vóór de vraag van volgende week.</span><span class="sxs-lookup"><span data-stu-id="38ae7-104">Within a given SKU, the requested or available date represents the highest priority; the demand of today should be dealt with before the demand of next week.</span></span> <span data-ttu-id="38ae7-105">Naast deze algemene prioriteit zal het planningssysteem ook voorstellen aan welk soort vraag moet worden voldaan voordat aan andere vraag wordt voldaan.</span><span class="sxs-lookup"><span data-stu-id="38ae7-105">But in addition to this overall priority, the planning system will also suggest which type of demand should be fulfilled before fulfilling another demand.</span></span> <span data-ttu-id="38ae7-106">Zo wordt ook voorgesteld welke voorzieningenbron moet worden toegepast voordat andere voorzieningenbronnen worden toegepast.</span><span class="sxs-lookup"><span data-stu-id="38ae7-106">Likewise, it will suggest what source of supply should be applied before applying other sources of supply.</span></span> <span data-ttu-id="38ae7-107">Dit gebeurt op basis van orderprioriteiten.</span><span class="sxs-lookup"><span data-stu-id="38ae7-107">This is done according to order priorities.</span></span>  
  
<span data-ttu-id="38ae7-108">Geladen vraag en aanbod dragen bij aan een profiel voor de voorspelde voorraad op basis van de volgende prioriteiten:</span><span class="sxs-lookup"><span data-stu-id="38ae7-108">Loaded demand and supply contribute to a profile for the projected inventory according to the following priorities:</span></span>  
  
## <a name="priorities-on-the-demand-side"></a><span data-ttu-id="38ae7-109">Prioriteiten aan de vraagkant</span><span class="sxs-lookup"><span data-stu-id="38ae7-109">Priorities on the Demand Side</span></span>  
1. <span data-ttu-id="38ae7-110">Al verzonden: Artikelpost</span><span class="sxs-lookup"><span data-stu-id="38ae7-110">Already shipped: Item Ledger Entry</span></span>  
2. <span data-ttu-id="38ae7-111">Inkoopretourorder</span><span class="sxs-lookup"><span data-stu-id="38ae7-111">Purchase Return Order</span></span>  
3. <span data-ttu-id="38ae7-112">Verkooporder</span><span class="sxs-lookup"><span data-stu-id="38ae7-112">Sales Order</span></span>  
4. <span data-ttu-id="38ae7-113">Onderhoudsorder</span><span class="sxs-lookup"><span data-stu-id="38ae7-113">Service Order</span></span>  
5. <span data-ttu-id="38ae7-114">Behoefte aan productieonderdelen</span><span class="sxs-lookup"><span data-stu-id="38ae7-114">Production Component Need</span></span>  
6. <span data-ttu-id="38ae7-115">Assemblageorderregel</span><span class="sxs-lookup"><span data-stu-id="38ae7-115">Assembly Order Line</span></span>  
7. <span data-ttu-id="38ae7-116">Uitgaande transferorder</span><span class="sxs-lookup"><span data-stu-id="38ae7-116">Outbound Transfer Order</span></span>  
8. <span data-ttu-id="38ae7-117">Raamcontract (dat niet al is verbruikt door verwante verkooporders)</span><span class="sxs-lookup"><span data-stu-id="38ae7-117">Blanket Order (that has not already been consumed by related sales orders)</span></span>  
9. <span data-ttu-id="38ae7-118">Prognose (die niet al is verbruikt door andere verkooporders)</span><span class="sxs-lookup"><span data-stu-id="38ae7-118">Forecast (that has not already been consumed by other sales orders)</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="38ae7-119">Inkoopretouren zijn meestal niet betrokken bij voorraadplanning; ze moeten altijd worden gereserveerd vanuit de lot die geretourneerd zal worden.</span><span class="sxs-lookup"><span data-stu-id="38ae7-119">Purchase returns are usually not involved in supply planning; they should always be reserved from the lot that is going to be returned.</span></span> <span data-ttu-id="38ae7-120">Indien niet gereserveerd, spelen inkoopretouren een rol in de beschikbaarheid en hebben ze een hoge prioriteit om te voorkomen dat het planningssysteem een voorzieningenorder voorstelt, puur met het oog op een inkoopretour.</span><span class="sxs-lookup"><span data-stu-id="38ae7-120">If not reserved, purchase returns play a role in the availability and are highly prioritized to avoid that the planning system suggests a supply order just to serve a purchase return.</span></span>  
  
## <a name="priorities-on-the-supply-side"></a><span data-ttu-id="38ae7-121">Prioriteiten aan de aanbodkant</span><span class="sxs-lookup"><span data-stu-id="38ae7-121">Priorities on the Supply Side</span></span>  
1. <span data-ttu-id="38ae7-122">Al in voorraad: Artikelpost (Planningsflexibiliteit = geen)</span><span class="sxs-lookup"><span data-stu-id="38ae7-122">Already in inventory: Item Ledger Entry (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="38ae7-123">Verkoopretourorder (Planningsflexibiliteit = Geen)</span><span class="sxs-lookup"><span data-stu-id="38ae7-123">Sales Return Order (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="38ae7-124">Inkomende transferorder</span><span class="sxs-lookup"><span data-stu-id="38ae7-124">Inbound Transfer Order</span></span>  
4. <span data-ttu-id="38ae7-125">Productieorder</span><span class="sxs-lookup"><span data-stu-id="38ae7-125">Production Order</span></span>  
5. <span data-ttu-id="38ae7-126">Assemblageorder</span><span class="sxs-lookup"><span data-stu-id="38ae7-126">Assembly Order</span></span>  
6. <span data-ttu-id="38ae7-127">Inkooporder</span><span class="sxs-lookup"><span data-stu-id="38ae7-127">Purchase Order</span></span>  
  
## <a name="priority-related-to-the-state-of-demand-and-supply"></a><span data-ttu-id="38ae7-128">Prioriteit met betrekking tot de status van vraag en aanbod</span><span class="sxs-lookup"><span data-stu-id="38ae7-128">Priority Related to the State of Demand and Supply</span></span>  
<span data-ttu-id="38ae7-129">Afgezien van prioriteiten als gevolg van het soort vraag en aanbod geeft de huidige status van de orders in het uitvoeringsproces ook een prioriteit aan.</span><span class="sxs-lookup"><span data-stu-id="38ae7-129">Apart from priorities given by the type of demand and supply, the present state of the orders in the execution process also defines a priority.</span></span> <span data-ttu-id="38ae7-130">Magazijnactiviteiten hebben bijvoorbeeld invloed en er wordt rekening gehouden met de status van verkoop-, inkoop-, transfer-, assemblage- en productieorders:</span><span class="sxs-lookup"><span data-stu-id="38ae7-130">For example, warehouse activities have an impact, and the status of sales, purchase, transfer, assembly, and production orders is taken into account:</span></span>  
  
1. <span data-ttu-id="38ae7-131">Gedeeltelijk verwerkt (Planningsflexibiliteit = Geen)</span><span class="sxs-lookup"><span data-stu-id="38ae7-131">Partly handled (Planning Flexibility = None)</span></span>  
2. <span data-ttu-id="38ae7-132">Al in verwerking in het magazijn (Planningsflexibiliteit = geen)</span><span class="sxs-lookup"><span data-stu-id="38ae7-132">Already in process in the warehouse (Planning Flexibility = None)</span></span>  
3. <span data-ttu-id="38ae7-133">Vrijgegeven - alle ordersoorten (Planningsflexibiliteit = Onbeperkt)</span><span class="sxs-lookup"><span data-stu-id="38ae7-133">Released – all order types (Planning Flexibility = Unlimited)</span></span>  
4. <span data-ttu-id="38ae7-134">Vaste geplande productieorder (Planningsflexibiliteit = Onbeperkt)</span><span class="sxs-lookup"><span data-stu-id="38ae7-134">Firm Planned Production Order (Planning Flexibility = Unlimited)</span></span>  
5. <span data-ttu-id="38ae7-135">Gepland/open - alle ordersoorten (Planningsflexibiliteit = Onbeperkt)</span><span class="sxs-lookup"><span data-stu-id="38ae7-135">Planned/Open – all order types (Planning Flexibility = Unlimited)</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="38ae7-136">Zie ook</span><span class="sxs-lookup"><span data-stu-id="38ae7-136">See Also</span></span>  
<span data-ttu-id="38ae7-137">[Ontwerpdetails: Vraag en aanbod afstemmen](design-details-balancing-demand-and-supply.md) </span><span class="sxs-lookup"><span data-stu-id="38ae7-137">[Design Details: Balancing Demand and Supply](design-details-balancing-demand-and-supply.md) </span></span>  
<span data-ttu-id="38ae7-138">[Ontwerpdetails: Centrale begrippen van het planningssysteem](design-details-central-concepts-of-the-planning-system.md) </span><span class="sxs-lookup"><span data-stu-id="38ae7-138">[Design Details: Central Concepts of the Planning System](design-details-central-concepts-of-the-planning-system.md) </span></span>  
[<span data-ttu-id="38ae7-139">Ontwerpdetails: Voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="38ae7-139">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)