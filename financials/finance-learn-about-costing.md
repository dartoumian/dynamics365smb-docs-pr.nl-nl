---
title: Over voorraadwaardering | Microsoft Docs
description: Voorraadkosten beheren heeft betrekking op het registreren en rapporteren van operationele bedrijfskosten. Dit omvat de rapportage van productie- en voorraadkosten (dus de waarde van artikelen).
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
ms.openlocfilehash: 5e6b691eae1663cdc93d851f531306c472291484
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="about-inventory-costing"></a><span data-ttu-id="17c0e-104">Over voorraadwaardering</span><span class="sxs-lookup"><span data-stu-id="17c0e-104">About Inventory Costing</span></span>
<span data-ttu-id="17c0e-105">Voorraadkosten beheren heeft betrekking op het registreren en rapporteren van operationele bedrijfskosten.</span><span class="sxs-lookup"><span data-stu-id="17c0e-105">Managing inventory costs is concerned with recording and reporting business operating costs.</span></span> <span data-ttu-id="17c0e-106">Dit omvat de rapportage van productie- en voorraadkosten (dus de waarde van artikelen).</span><span class="sxs-lookup"><span data-stu-id="17c0e-106">It includes the reporting of manufacturing costs and inventory costs, that is, the value of items.</span></span>  

 <span data-ttu-id="17c0e-107">U dient de volgende centrale principes te begrijpen: met waarderingsmethoden wordt gedefinieerd hoe artikelen worden gewaardeerd wanneer ze de voorraad verlaten, met een herwaardering van kosten worden de kosten bijgewerkt van goederen die worden verkocht met gerelateerde inkoopkosten die na de verkoop zijn geboekt en de voorraadwaarden moeten regelmatig worden geboekt naar speciale grootboekrekeningen.</span><span class="sxs-lookup"><span data-stu-id="17c0e-107">Central principles to understand are that costing methods define how items are valued when they leave inventory, that cost adjustment updates the cost of goods sold with related purchase costs posted after the sale, and that inventory values must be posted to dedicated G/L accounts at regular intervals.</span></span>  

 <span data-ttu-id="17c0e-108">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="17c0e-108">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="17c0e-109">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="17c0e-109">**To**</span></span>|<span data-ttu-id="17c0e-110">**Zie**</span><span class="sxs-lookup"><span data-stu-id="17c0e-110">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="17c0e-111">Het verschil te leren tussen de vijf verschillende waarderingsmethoden en hun effect op kostenstromen.</span><span class="sxs-lookup"><span data-stu-id="17c0e-111">Distinguish the five different costing methods and their effect on cost flows.</span></span>|[<span data-ttu-id="17c0e-112">Ontwerpdetails: Waarderingsmethoden</span><span class="sxs-lookup"><span data-stu-id="17c0e-112">Design Details: Costing Methods</span></span>](design-details-costing-methods.md)|  
|<span data-ttu-id="17c0e-113">Meer te weten te komen over hoe artikelvereffeningsposten voorraadafnames en -toenames dynamisch aan elkaar koppelen om controle te houden over de kostenstromen.</span><span class="sxs-lookup"><span data-stu-id="17c0e-113">Learn how item application entries dynamically link inventory decreases with increases to keep control of cost flows.</span></span>|[<span data-ttu-id="17c0e-114">Ontwerpdetails: Artikelvereffening</span><span class="sxs-lookup"><span data-stu-id="17c0e-114">Design Details: Item Application</span></span>](design-details-item-application.md)|  
|<span data-ttu-id="17c0e-115">Meer te weten te komen over hoe de eenheidsprijs van een artikel voortdurend wordt bijgewerkt met de kosten van de recentste transactie ervan volgens de waarderingsmethode van het artikel.</span><span class="sxs-lookup"><span data-stu-id="17c0e-115">Learn how an item's unit cost is continuously updated with the cost of its latest transaction according to the item's costing method.</span></span>|[<span data-ttu-id="17c0e-116">Ontwerpdetails: Kostenwaardering</span><span class="sxs-lookup"><span data-stu-id="17c0e-116">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)|  
|<span data-ttu-id="17c0e-117">Meer te weten te komen over hoe de gemiddelde kostprijs van een artikel dynamisch wordt berekend aan de hand van de geselecteerde periode voor gemiddelde kostprijsberekening.</span><span class="sxs-lookup"><span data-stu-id="17c0e-117">Learn how an item's average cost is dynamically calculated according to the selected average cost period.</span></span>|[<span data-ttu-id="17c0e-118">Ontwerpdetails: Gemiddelde kostprijs</span><span class="sxs-lookup"><span data-stu-id="17c0e-118">Design Details: Average Cost</span></span>](design-details-average-cost.md)|  
|<span data-ttu-id="17c0e-119">Onderscheid te maken tussen verwachte kosten (nog niet gefactureerd) en werkelijke kosten en voor meer informatie over hoe dit wordt beheerd in het grootboek</span><span class="sxs-lookup"><span data-stu-id="17c0e-119">Distinguish expected cost (not yet invoiced) from actual cost and learn how it is managed in the general ledger.</span></span>|[<span data-ttu-id="17c0e-120">Ontwerpdetails: Verwachte kostenboeking</span><span class="sxs-lookup"><span data-stu-id="17c0e-120">Design Details: Expected Cost Posting</span></span>](design-details-expected-cost-posting.md)|  
|<span data-ttu-id="17c0e-121">Het herwaarderingsmechanisme voor kosten te begrijpen, dat ervoor zorgt dat kosten naar voren komen, zelfs wanneer voorraadtransacties willekeurig plaatsvinden.</span><span class="sxs-lookup"><span data-stu-id="17c0e-121">Understand the cost adjustment mechanism, which ensures that costs are brought forward even if inventory transactions happen in a random manner.</span></span>|[<span data-ttu-id="17c0e-122">Ontwerpdetails: Kostenwaardering</span><span class="sxs-lookup"><span data-stu-id="17c0e-122">Design Details: Cost Adjustment</span></span>](design-details-cost-adjustment.md)|  
|<span data-ttu-id="17c0e-123">Te lezen waarom vaste verrekenprijzen vaak worden gebruikt door productiebedrijven als een waarderingsbasis voor onderdelen en eindartikelen.</span><span class="sxs-lookup"><span data-stu-id="17c0e-123">Read why standard costs are often used by manufacturing companies as a valuation base for components and end items.</span></span>|[<span data-ttu-id="17c0e-124">Informatie over het berekenen van vaste verrekenprijzen</span><span class="sxs-lookup"><span data-stu-id="17c0e-124">About Calculating Standard Cost</span></span>](finance-about-calculating-standard-cost.md)|  
|<span data-ttu-id="17c0e-125">Te begrijpen hoe de voorraadwaarde wordt weerspiegeld in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="17c0e-125">Understand how the value of inventory is reflected in the general ledger.</span></span>|[<span data-ttu-id="17c0e-126">Kosten rapporteren en afstemmen met het grootboek</span><span class="sxs-lookup"><span data-stu-id="17c0e-126">Reporting Costs and Reconciling with the General Ledger</span></span>](finance-report-costs-and-reconcile-with-the-general-ledger.md)|  
|<span data-ttu-id="17c0e-127">Meer te weten te komen over hoe artikeltoeslagen, zoals verzendkosten en verzekering, extra kostenonderdelen kunnen toewijzen aan de eenheidsprijs van een artikel.</span><span class="sxs-lookup"><span data-stu-id="17c0e-127">Learn how item charges, such as freight and insurance, can assign additional cost components to an item's unit cost.</span></span>|[<span data-ttu-id="17c0e-128">Procedure: Artikeltoeslagen gebruiken om extra handelskosten te verantwoorden</span><span class="sxs-lookup"><span data-stu-id="17c0e-128">How to: Use Item Charges to Account for Additional Trade Costs</span></span>](payables-how-assign-item-charges.md)|  
|<span data-ttu-id="17c0e-129">Te lezen hoe voorraadperioden een bedrijf kunnen helpen de voorraadwaarde gedurende de tijd te beheren door kortere perioden te definiëren die gedurende het boekjaar voor boeking kunnen worden gesloten.</span><span class="sxs-lookup"><span data-stu-id="17c0e-129">Read how inventory periods help a company to control inventory value over time by defining shorter periods that can be closed for posting as the fiscal year progresses.</span></span>|[<span data-ttu-id="17c0e-130">Procedure: werken met voorraadperioden</span><span class="sxs-lookup"><span data-stu-id="17c0e-130">How to: Work with Inventory Periods</span></span>](finance-how-to-work-with-inventory-periods.md)|  
|<span data-ttu-id="17c0e-131">Alle mechanismen in de kostprijsberekeningengine begrijpen, inclusief wat er gebeurt wanneer u assemblage- en productietransacties boekt.</span><span class="sxs-lookup"><span data-stu-id="17c0e-131">Understand all mechanisms in the costing engine, including what happens when you post assembly and production transactions.</span></span>|[<span data-ttu-id="17c0e-132">Ontwerpdetails: Voorraadwaardering</span><span class="sxs-lookup"><span data-stu-id="17c0e-132">Design Details: Inventory Costing</span></span>](design-details-inventory-costing.md)|

## <a name="see-also"></a><span data-ttu-id="17c0e-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="17c0e-133">See Also</span></span>
<span data-ttu-id="17c0e-134">[Voorraadkosten beheren](finance-manage-inventory-costs.md)  </span><span class="sxs-lookup"><span data-stu-id="17c0e-134">[Managing Inventory Costs](finance-manage-inventory-costs.md)  </span></span>  
<span data-ttu-id="17c0e-135">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="17c0e-135">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
