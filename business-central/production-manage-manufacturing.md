---
title: Productie uitvoeren | Microsoft Docs
description: Wanneer er voor vraag is gepland en de materialen zijn uitgegeven op basis van productiestuklijsten, kunnen de daadwerkelijke productiebewerkingen starten en vervolgens worden uitgevoerd in de volgorde die is gedefinieerd in het bewerkingsplan van de productieorder.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: c97cdafceb5fbf8df403309dddda0faeac7a26b6
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="manufacturing"></a><span data-ttu-id="840be-103">Productie</span><span class="sxs-lookup"><span data-stu-id="840be-103">Manufacturing</span></span>
<span data-ttu-id="840be-104">Wanneer er voor vraag is gepland en de materialen zijn uitgegeven op basis van productiestuklijsten, kunnen de daadwerkelijke productiebewerkingen starten en vervolgens worden uitgevoerd in de volgorde die is gedefinieerd in het bewerkingsplan van de productieorder.</span><span class="sxs-lookup"><span data-stu-id="840be-104">When demand is planned for and the materials have been issued according to production BOMs, then the actual production operations can start and be executed in the sequence defined by the production order routing.</span></span>  

<span data-ttu-id="840be-105">Een uit systeemoogpunt belangrijk deel van de uitvoering van productie is het boeken van productie-output in de database om voortgang te melden en om de voorraad met de gereedgemelde artikelen bij te werken.</span><span class="sxs-lookup"><span data-stu-id="840be-105">An important part of executing production, from a system point of view, is to post production output to the database to report progress and to update inventory with the finished items.</span></span> <span data-ttu-id="840be-106">Output-boeking kan handmatig worden gedaan door na de productiebewerkingen dagboekregels in te vullen en te boeken.</span><span class="sxs-lookup"><span data-stu-id="840be-106">Output posting can be done manually, by filling and posting journal lines after production operations.</span></span> <span data-ttu-id="840be-107">Of het kan automatisch worden gedaan door middel van achterwaarts afboeken.</span><span class="sxs-lookup"><span data-stu-id="840be-107">Or, it can be done automatically with the use of backward flushing.</span></span> <span data-ttu-id="840be-108">In dat geval wordt materiaalverbruik automatisch samen met de output geboekt, wanneer de productieorder wordt gereedgemeld.</span><span class="sxs-lookup"><span data-stu-id="840be-108">In that case material consumption is automatically posted along with output when the production order changes to finished.</span></span>  

<span data-ttu-id="840be-109">Als alternatief voor het in batches boeken van output voor meerdere productieorders kunt u het venster **Productiedagboek** gebruiken om verbruik en/of output voor één productieorderregel te boeken.</span><span class="sxs-lookup"><span data-stu-id="840be-109">As an alternative to the batch journal for output posting for multiple production orders, you can use the **Production Journal** window to post consumption and/or output for one production order line.</span></span>

<span data-ttu-id="840be-110">Voordat u artikelen kunt gaan produceren, moet u verschillende zaken instellen, zoals afdelingen, bewerkingsplannen en productiestuklijsten.</span><span class="sxs-lookup"><span data-stu-id="840be-110">Before you can begin to produce items, you must make various setup, such as work centers, routings, and production BOMs.</span></span> <span data-ttu-id="840be-111">Zie [Productie instellen](production-configure-production-processes.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="840be-111">For more information, see [Setting Up Manufacturing](production-configure-production-processes.md).</span></span>

<span data-ttu-id="840be-112">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="840be-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="840be-113">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="840be-113">**To**</span></span>|<span data-ttu-id="840be-114">**Zie**</span><span class="sxs-lookup"><span data-stu-id="840be-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="840be-115">Begrijpen hoe de productieorders werken.</span><span class="sxs-lookup"><span data-stu-id="840be-115">Understand how production orders work.</span></span>|[<span data-ttu-id="840be-116">Informatie over productieorders</span><span class="sxs-lookup"><span data-stu-id="840be-116">About Production Orders</span></span>](production-about-production-orders.md)|
|<span data-ttu-id="840be-117">Handmatig productieorders maken.</span><span class="sxs-lookup"><span data-stu-id="840be-117">Create production orders manually.</span></span>|[<span data-ttu-id="840be-118">Productieorders maken</span><span class="sxs-lookup"><span data-stu-id="840be-118">Create Production Orders</span></span>](production-how-to-create-production-orders.md)|
|<span data-ttu-id="840be-119">Alle of bepaalde bewerkingen in een productieorder uitbesteden aan een toeleverancier.</span><span class="sxs-lookup"><span data-stu-id="840be-119">Outsource all or selected operations in a production order to a subcontractor.</span></span>|[<span data-ttu-id="840be-120">Productie uitbesteden</span><span class="sxs-lookup"><span data-stu-id="840be-120">Subcontract Manufacturing</span></span>](production-how-to-subcontract-manufacturing.md)|
|<span data-ttu-id="840be-121">Productie-output en verbruikte materiaal en tijd vastleggen voor één vrijgegeven productieorderregel.</span><span class="sxs-lookup"><span data-stu-id="840be-121">Record and post production output along with material and time consumption for a single released production order line.</span></span>|[<span data-ttu-id="840be-122">Verbruik en output boeken voor één vrijgegeven productieorderregel.</span><span class="sxs-lookup"><span data-stu-id="840be-122">Post Consumption and Output for One Released Production Order Line</span></span>](production-how-to-register-consumption-and-output.md)|  
|<span data-ttu-id="840be-123">Het aantal gebruikte onderdelen per bewerking in batches in een dagboek boeken waarin meerdere geplande productieorders kunnen worden verwerkt.</span><span class="sxs-lookup"><span data-stu-id="840be-123">Batch post the quantity of components used per operation in a journal that can processes multiple planned production orders.</span></span>|[<span data-ttu-id="840be-124">Verbruik in batches boeken</span><span class="sxs-lookup"><span data-stu-id="840be-124">Batch Post Consumption</span></span>](production-how-to-post-consumption.md)|
|<span data-ttu-id="840be-125">Het aantal voltooide artikelen en de bestede tijd per bewerking in een dagboek boeken waarin meerdere vrijgegeven productieorders kunnen worden verwerkt.</span><span class="sxs-lookup"><span data-stu-id="840be-125">Post the quantity of finished items and the time spent per operation in a journal that can processes multiple released production orders.</span></span>|[<span data-ttu-id="840be-126">Output en bewerkingstijden in batches boeken</span><span class="sxs-lookup"><span data-stu-id="840be-126">Batch Post Output and Run Times</span></span>](production-how-to-post-output-quantity.md)|  
|<span data-ttu-id="840be-127">Het aantal artikelen boeken dat is geproduceerd in elke voltooide bewerking, maar niet geldt als voltooide output maar als uitgevallen materiaal.</span><span class="sxs-lookup"><span data-stu-id="840be-127">Post the number of items produced in each finished operation which do not qualify as finished output, but as scrapped material.</span></span>|[<span data-ttu-id="840be-128">Uitval boeken</span><span class="sxs-lookup"><span data-stu-id="840be-128">Post Scrap</span></span>](production-how-to-post-scrap.md)|
|<span data-ttu-id="840be-129">De werklast voor de shopfloor als resultaat van geplande en vrijgegeven productieorders weergeven.</span><span class="sxs-lookup"><span data-stu-id="840be-129">View the shop floor load as a result of planned and released production orders.</span></span>|[<span data-ttu-id="840be-130">De werklast in afdelingen en bewerkingsplaatsen weergeven</span><span class="sxs-lookup"><span data-stu-id="840be-130">View the Load in Work and Machine Centers</span></span>](production-how-to-view-the-load-on-work-centers.md)|      
|<span data-ttu-id="840be-131">Het venster **Capaciteitsdagboek** gebruiken om verbruikte capaciteit te boeken die niet is toegewezen aan een productieorder, zoals onderhoudswerkzaamheden.</span><span class="sxs-lookup"><span data-stu-id="840be-131">Use the **Capacity Journal** window to post consumed capacities that are not assigned to a production order, such as maintenance work.</span></span>|[<span data-ttu-id="840be-132">Capaciteit boeken</span><span class="sxs-lookup"><span data-stu-id="840be-132">Post Capacities</span></span>](production-how-to-post-capacities.md)|  
|<span data-ttu-id="840be-133">De kosten van gereedgemelde productieartikelen en verbruikte materialen berekenen en aanpassen voor financiële reconciliatie.</span><span class="sxs-lookup"><span data-stu-id="840be-133">Calculate and adjust the cost of finished production items and consumed components for financial reconciliation.</span></span>|[<span data-ttu-id="840be-134">Over de kosten van de gereedgemelde productieorder</span><span class="sxs-lookup"><span data-stu-id="840be-134">About Finished Production Order Costs</span></span>](finance-about-finished-production-order-costs.md)|  

## <a name="see-also"></a><span data-ttu-id="840be-135">Zie ook</span><span class="sxs-lookup"><span data-stu-id="840be-135">See Also</span></span>  
[<span data-ttu-id="840be-136">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="840be-136">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
<span data-ttu-id="840be-137">[Gepland](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="840be-137">[Planning](production-planning.md)    </span></span>  
[<span data-ttu-id="840be-138">Voorraad</span><span class="sxs-lookup"><span data-stu-id="840be-138">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="840be-139">Inkoop</span><span class="sxs-lookup"><span data-stu-id="840be-139">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="840be-140">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="840be-140">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
## [!INCLUDE[d365fin](includes/training_link_md.md)]
