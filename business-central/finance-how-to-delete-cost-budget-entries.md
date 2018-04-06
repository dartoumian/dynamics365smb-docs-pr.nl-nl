---
title: 'Procedure: kostenbudgetposten verwijderen | Microsoft Docs'
description: Door middel van de batchtaak **Kostenbudgetposten verwijderen** annuleert u kostenbegrotingsposten uit het kostenbudgetregister.
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
ms.openlocfilehash: acd8e0f25a3909ceab3dd63e04509ab48a300bb6
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="delete-cost-budget-entries"></a><span data-ttu-id="5dee8-103">Kostenbudgetposten verwijderen</span><span class="sxs-lookup"><span data-stu-id="5dee8-103">Delete Cost Budget Entries</span></span>
<span data-ttu-id="5dee8-104">Door middel van de batchtaak **Kostenbudgetposten verwijderen** annuleert u kostenbegrotingsposten uit het kostenbudgetregister.</span><span class="sxs-lookup"><span data-stu-id="5dee8-104">You use the **Delete Cost Budget Entries** batch job to cancel cost budget entries from the cost budget register.</span></span>  

<span data-ttu-id="5dee8-105">Om hiaten in de kostenbudgetposten en kostenregisterposten te voorkomen, kunt u één enkele post of een reeks posten middenin een lijst met registerposten niet verwijderen.</span><span class="sxs-lookup"><span data-stu-id="5dee8-105">To prevent any gaps in the cost budget entries and cost register entries, you cannot delete a single entry or a batch of entries in the middle of the list of register entries.</span></span>  

### <a name="to-delete-a-cost-budget-entry"></a><span data-ttu-id="5dee8-106">Kostenbudgetposten verwijderen</span><span class="sxs-lookup"><span data-stu-id="5dee8-106">To delete a cost budget entry</span></span>  

1.  <span data-ttu-id="5dee8-107">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Kostenbudgetposten verwijderen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="5dee8-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Cost Budget Entries**, and then choose the related link.</span></span>  

    <span data-ttu-id="5dee8-108">Het veld **Naar journaalnr.**</span><span class="sxs-lookup"><span data-stu-id="5dee8-108">The **To Register No.**</span></span> <span data-ttu-id="5dee8-109">bevat het nummer van de laatste journaalpost en kan niet worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="5dee8-109">field contains the last register entry number and cannot be changed.</span></span>  

    <span data-ttu-id="5dee8-110">U kunt het veld **Van journaalnr.** gebruiken</span><span class="sxs-lookup"><span data-stu-id="5dee8-110">You can use the **From Register No.**</span></span> <span data-ttu-id="5dee8-111">om een nummer voor een journaalpost te selecteren waar de verwijdering moet beginnen.</span><span class="sxs-lookup"><span data-stu-id="5dee8-111">field to select a register entry number from which the deletion should begin.</span></span>  
2.  <span data-ttu-id="5dee8-112">Kies de knop **OK** om de geselecteerde kostenbegrotingsposten te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="5dee8-112">Choose the **OK** button to delete the selected cost budget entries.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="5dee8-113">Om te voorkomen dat kostenbegrotingsposten onbedoeld worden verwijderd, kunt u journaalposten sluiten door de regels als **gesloten** te markeren in het veld **Gesloten** in het venster **Kostenbudgetregisters**.</span><span class="sxs-lookup"><span data-stu-id="5dee8-113">To avoid an accidental deletion of cost budget entries, you can close register entries by marking the lines as **Closed** in the **Closed** field in the **Cost Budget Registers** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5dee8-114">Zie ook</span><span class="sxs-lookup"><span data-stu-id="5dee8-114">See Also</span></span>  
<span data-ttu-id="5dee8-115">[Kosten verantwoorden](finance-manage-cost-accounting.md)
[Kostenbudgetten maken](finance-create-cost-budgets.md)</span><span class="sxs-lookup"><span data-stu-id="5dee8-115">[Accounting for Costs](finance-manage-cost-accounting.md)
[Creating Cost Budgets](finance-create-cost-budgets.md)</span></span>  
<span data-ttu-id="5dee8-116">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5dee8-116">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
