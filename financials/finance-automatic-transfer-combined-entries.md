---
title: Automatische overdracht en gecombineerde posten | Microsoft Docs
description: In kostprijsboekhouding kunt u grootboekposten overbrengen naar een kostensoort door middel van een gecombineerde boeking. U kunt opgeven of een kostensoort gecombineerde posten ontvangt in het veld **Posten combineren** in de definitie van het kostensoort. De volgende tabel beschrijft de verschillende opties.
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
ms.openlocfilehash: bd80d0a7a701256dfdae3346e899b84eeb990a40
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="automatic-transfer-and-combined-entries"></a><span data-ttu-id="54ffa-105">Automatische overdracht en gecombineerde posten</span><span class="sxs-lookup"><span data-stu-id="54ffa-105">Automatic Transfer and Combined Entries</span></span>
<span data-ttu-id="54ffa-106">In kostprijsboekhouding kunt u grootboekposten overbrengen naar een kostensoort door middel van een gecombineerde boeking.</span><span class="sxs-lookup"><span data-stu-id="54ffa-106">In cost accounting, you can transfer general ledger entries to a cost type by using a combined posting.</span></span> <span data-ttu-id="54ffa-107">U kunt opgeven of een kostensoort gecombineerde posten ontvangt in het veld **Posten combineren** in de definitie van het kostensoort.</span><span class="sxs-lookup"><span data-stu-id="54ffa-107">You can specify if a cost type receives combined entries in the **Combine Entries** field in the cost type definition.</span></span> <span data-ttu-id="54ffa-108">De volgende tabel beschrijft de verschillende opties.</span><span class="sxs-lookup"><span data-stu-id="54ffa-108">The following table describes the different options.</span></span>  

|<span data-ttu-id="54ffa-109">Posten combineren</span><span class="sxs-lookup"><span data-stu-id="54ffa-109">Combine entries</span></span>|<span data-ttu-id="54ffa-110">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="54ffa-110">Description</span></span>|  
|---------------------|-----------------|  
|<span data-ttu-id="54ffa-111">Geen</span><span class="sxs-lookup"><span data-stu-id="54ffa-111">None</span></span>|<span data-ttu-id="54ffa-112">Elke grootboekpost wordt afzonderlijk overgebracht naar het bijbehorende kostensoort.</span><span class="sxs-lookup"><span data-stu-id="54ffa-112">Each general ledger entry is transferred individually to the corresponding cost type.</span></span>|  
|<span data-ttu-id="54ffa-113">Dag</span><span class="sxs-lookup"><span data-stu-id="54ffa-113">Day</span></span>|<span data-ttu-id="54ffa-114">Grootboekposten met dezelfde boekingsdatum worden als één post overgeboekt naar de bijbehorende kostensoort.</span><span class="sxs-lookup"><span data-stu-id="54ffa-114">General ledger entries with the same posting date are transferred as one entry to the corresponding cost type.</span></span>|  
|<span data-ttu-id="54ffa-115">Maand</span><span class="sxs-lookup"><span data-stu-id="54ffa-115">Month</span></span>|<span data-ttu-id="54ffa-116">Alle grootboekposten in dezelfde kalendermaand worden als één post overgeboekt naar de bijbehorende kostensoort.</span><span class="sxs-lookup"><span data-stu-id="54ffa-116">All general ledger entries in the same calendar month are transferred as one entry to the corresponding cost type.</span></span>|  

> [!IMPORTANT]  
>  <span data-ttu-id="54ffa-117">Als u het selectievakje **Automatisch overdragen van GB** in het venster **Instelling kostprijsboekhouding** hebt ingeschakeld, wordt de kostprijsboekhouding automatisch bijgewerkt in [!INCLUDE[d365fin](includes/d365fin_md.md)] na elke boeking in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="54ffa-117">If you have selected the **Auto Transfer from G/L** check box in the **Cost Accounting Setup** window, [!INCLUDE[d365fin](includes/d365fin_md.md)] updates the cost accounting after every posting in the general ledger.</span></span> <span data-ttu-id="54ffa-118">Gecombineerde posten zijn niet mogelijk.</span><span class="sxs-lookup"><span data-stu-id="54ffa-118">Combined entries are not possible.</span></span>  

## <a name="see-also"></a><span data-ttu-id="54ffa-119">Zie ook</span><span class="sxs-lookup"><span data-stu-id="54ffa-119">See Also</span></span>  
 <span data-ttu-id="54ffa-120">[Procedure: grootboekposten overbrengen naar kostenposten](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="54ffa-120">[How to: Transfer General Ledger Entries to Cost Entries](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="54ffa-121">[Criteria voor het overbrengen van grootboekposten naar kostenposten.](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="54ffa-121">[Criteria for Transferring General Ledger Entries to Cost Entries](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md) </span></span>  
 <span data-ttu-id="54ffa-122">[Resultaten van de overboeking](finance-results-of-the-transfer.md) </span><span class="sxs-lookup"><span data-stu-id="54ffa-122">[Results of the Transfer](finance-results-of-the-transfer.md) </span></span>  
 [<span data-ttu-id="54ffa-123">Kostenposten overbrengen en boeken</span><span class="sxs-lookup"><span data-stu-id="54ffa-123">Transferring and Posting Cost Entries</span></span>](finance-transfer-and-post-cost-entries.md)  
 <span data-ttu-id="54ffa-124">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="54ffa-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
