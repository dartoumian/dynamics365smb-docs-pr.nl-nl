---
title: Outputboeking tegenboeken | Microsoft Docs
description: Het kan voorkomen dat een outputboeking moet worden tegengeboekt. Dit is bijvoorbeeld het geval als er een gegevensinvoerfout is gemaakt en er een onjuiste hoeveelheid output is geboekt op een productieorder.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7ac453ff87d78e6be0567ba93b58c0f8938f4052
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-reverse-output-posting"></a><span data-ttu-id="84db5-104">Procedure: een outputboeking tegenboeken</span><span class="sxs-lookup"><span data-stu-id="84db5-104">How to: Reverse Output Posting</span></span>
<span data-ttu-id="84db5-105">Het kan voorkomen dat een outputboeking moet worden tegengeboekt.</span><span class="sxs-lookup"><span data-stu-id="84db5-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="84db5-106">Dit is bijvoorbeeld het geval als er een gegevensinvoerfout is gemaakt en er een onjuiste hoeveelheid output is geboekt op een productieorder.</span><span class="sxs-lookup"><span data-stu-id="84db5-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="84db5-107">Een outputboeking tegenboeken</span><span class="sxs-lookup"><span data-stu-id="84db5-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="84db5-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Outputdagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="84db5-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="84db5-109">Selecteer uw batch.</span><span class="sxs-lookup"><span data-stu-id="84db5-109">Select your batch.</span></span>  
2. <span data-ttu-id="84db5-110">Vul de velden in.</span><span class="sxs-lookup"><span data-stu-id="84db5-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="84db5-111">Zie voor meer informatie [Procedure: Output en bewerkingstijd in batches boeken](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="84db5-111">For more information, see [How to: Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="84db5-112">Selecteer in het veld **Vereffenen met post** de bijbehorende artikelpost.</span><span class="sxs-lookup"><span data-stu-id="84db5-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="84db5-113">Hiermee voert u een tegenboeking uit van de capaciteit en artikelposten.</span><span class="sxs-lookup"><span data-stu-id="84db5-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="84db5-114">Boek de tegenboeking door het dagboek te boeken.</span><span class="sxs-lookup"><span data-stu-id="84db5-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="84db5-115">De posten van het outputdagboek worden als positieve herwaardering geboekt op de artikelposten.</span><span class="sxs-lookup"><span data-stu-id="84db5-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="84db5-116">Zie ook</span><span class="sxs-lookup"><span data-stu-id="84db5-116">See Also</span></span>  
 <span data-ttu-id="84db5-117">[Productie](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="84db5-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="84db5-118">Productie instellen</span><span class="sxs-lookup"><span data-stu-id="84db5-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="84db5-119">[Gepland](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="84db5-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="84db5-120">Voorraad</span><span class="sxs-lookup"><span data-stu-id="84db5-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="84db5-121">Inkoop</span><span class="sxs-lookup"><span data-stu-id="84db5-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="84db5-122">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="84db5-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
