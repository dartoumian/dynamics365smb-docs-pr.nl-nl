---
title: Standaardinkoop- en verkoopregels instellen
description: In Finance and Operations, Business edition kunt u opgeven hoe de standaardverkoop- of standaardinkoopcodes worden ingevoerd wanneer u de opgegeven verkoop- of inkoopdocumenten maakt.
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
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 421a0c35793489d49b64f10be02e315eade90565
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-standard-sales-or-purchase-lines"></a><span data-ttu-id="c132f-103">Standaardinkoop- of verkoopregels instellen</span><span class="sxs-lookup"><span data-stu-id="c132f-103">Set Up Standard Sales or Purchase Lines</span></span>
<span data-ttu-id="c132f-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] kunt u opgeven hoe de standaardverkoop- of standaardinkoopcodes worden ingevoerd wanneer u de opgegeven verkoop- of inkoopdocumenten maakt.</span><span class="sxs-lookup"><span data-stu-id="c132f-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can specify how the standard sales or purchase codes will be entered when you are creating the specified sales or purchase documents.</span></span>  

<span data-ttu-id="c132f-105">In de volgende procedure wordt beschreven hoe u een standaardverkoopregel instelt, maar u kunt dezelfde stappen gebruiken om standaardinkoopregels in te stellen in het venster **Inkoopinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="c132f-105">The following procedure describes how to set up a standard sales line, but the same steps apply to setting up standard purchase lines in the **Purchases & Payables Setup** window.</span></span>  

## <a name="to-set-up-a-standard-sales-line"></a><span data-ttu-id="c132f-106">Een standaardverkoopregel instellen</span><span class="sxs-lookup"><span data-stu-id="c132f-106">To set up a standard sales line</span></span>  

1.  <span data-ttu-id="c132f-107">Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Instellingen van verkoop en tegoeden** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c132f-107">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales & Receivables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c132f-108">Vul de velden in op het sneltabblad **Std.klantenverkoopcodes**, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="c132f-108">On the **Std. Customer Sales Codes** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="c132f-109">Veld</span><span class="sxs-lookup"><span data-stu-id="c132f-109">Field</span></span>|<span data-ttu-id="c132f-110">Description</span><span class="sxs-lookup"><span data-stu-id="c132f-110">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="c132f-111">**Standaardklantverkoopregels invoegen**</span><span class="sxs-lookup"><span data-stu-id="c132f-111">**Insert Std. Cust. Sales Lines**</span></span>|<span data-ttu-id="c132f-112">Geef de methode op om de standaardklantverkoopregels in te voegen.</span><span class="sxs-lookup"><span data-stu-id="c132f-112">Specify the method by which to insert the standard customer sales lines.</span></span><br /><br /> <span data-ttu-id="c132f-113">-   **Handmatig** - U moet u de standaardverkoopregels invoegen die u voor die klant instelt.</span><span class="sxs-lookup"><span data-stu-id="c132f-113">-   **Manual** - You must insert the standard sales lines that you set up for that customer.</span></span> <span data-ttu-id="c132f-114">Als u deze optie selecteert, kunt u de velden **Offertes**, **Orders**, **Facturen** of **Creditnota's** in het venster **Verkoopinstellingen** niet selecteren.</span><span class="sxs-lookup"><span data-stu-id="c132f-114">If you select this option, then you will not be able to select the **Quotes**, **Orders**, **Invoices**, or **Credit Memos** fields in the **Sales & Receivables Setup** window.</span></span><br /><span data-ttu-id="c132f-115">-   **Automatisch** - voegt automatisch standaardverkoopregels in verkoopdocumenten in die u voor een klant maakt.</span><span class="sxs-lookup"><span data-stu-id="c132f-115">-   **Automatic** - Automatically insert standard sales lines on sales documents that you create for a customer.</span></span><br /><span data-ttu-id="c132f-116">-   **Altijd vragen** - een venster openen met alle bestaande standaardverkoopcodes die u voor de klant instelt.</span><span class="sxs-lookup"><span data-stu-id="c132f-116">-   **Always Ask** - Display a window with all the existing standard sales codes that you set up for the customer.</span></span>|  
    |<span data-ttu-id="c132f-117">**Offertes**</span><span class="sxs-lookup"><span data-stu-id="c132f-117">**Quotes**</span></span>|<span data-ttu-id="c132f-118">Selecteren om standaardverkoopregels in te voegen in verkoopoffertes.</span><span class="sxs-lookup"><span data-stu-id="c132f-118">Select to insert standard sales lines on sales quotes.</span></span>|  
    |<span data-ttu-id="c132f-119">**Orders**</span><span class="sxs-lookup"><span data-stu-id="c132f-119">**Orders**</span></span>|<span data-ttu-id="c132f-120">Selecteren om standaardverkoopregels in te voegen in verkooporders.</span><span class="sxs-lookup"><span data-stu-id="c132f-120">Select to insert standard sales lines on sales orders.</span></span>|  
    |<span data-ttu-id="c132f-121">**Facturen**</span><span class="sxs-lookup"><span data-stu-id="c132f-121">**Invoices**</span></span>|<span data-ttu-id="c132f-122">Selecteren om standaardverkoopregels in te voegen in verkoopfacturen.</span><span class="sxs-lookup"><span data-stu-id="c132f-122">Select to insert standard sales lines on sales invoices.</span></span>|  
    |<span data-ttu-id="c132f-123">**Creditnota's**</span><span class="sxs-lookup"><span data-stu-id="c132f-123">**Credit Memos**</span></span>|<span data-ttu-id="c132f-124">Selecteren om standaardverkoopregels in te voegen in verkoopcreditnota's.</span><span class="sxs-lookup"><span data-stu-id="c132f-124">Select to insert standard sales lines on sales credit memos.</span></span>|  

3.  <span data-ttu-id="c132f-125">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="c132f-125">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c132f-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="c132f-126">See Also</span></span>  
[<span data-ttu-id="c132f-127">Periodieke verkoop- en inkoopregels maken</span><span class="sxs-lookup"><span data-stu-id="c132f-127">Create Recurring Sales and Purchase Lines</span></span>](../../sales-how-work-standard-lines.md)
