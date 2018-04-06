---
title: Inkomende documenten maken van documenten| Microsoft Docs
description: U kunt records maken van inkomende documenten, zoals e-facturen, en OCR-taken, eCommerce en documentuitwisseling beheren.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 2f3613c352f163b751a88292a049c53c7d4ee16b
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="create-incoming-document-records-directly-from-documents-and-entries"></a><span data-ttu-id="8a50f-103">Inkomende documentrecords maken direct van documenten en posten</span><span class="sxs-lookup"><span data-stu-id="8a50f-103">Create Incoming Document Records Directly from Documents and Entries</span></span>
<span data-ttu-id="8a50f-104">U kunt externe bedrijfsdocumenten opslaan in [!INCLUDE[d365fin](includes/d365fin_md.md)] door de documentbestanden aan de gerelateerde inkomende documentrecords te koppelen.</span><span class="sxs-lookup"><span data-stu-id="8a50f-104">You can store external business documents in [!INCLUDE[d365fin](includes/d365fin_md.md)] by attaching the document files to the related incoming document records.</span></span> <span data-ttu-id="8a50f-105">Als het document, zoals een inkoopfactuur, niet is ontstaan als inkomende documentrecord, kunt u het later nog maken en koppelen aan een inkomende documentrecord.</span><span class="sxs-lookup"><span data-stu-id="8a50f-105">If the document, such as a purchase invoice, did not start its existence as an incoming document record, you can still create and connect an incoming document record to it later.</span></span> <span data-ttu-id="8a50f-106">U kunt inkomende documentbestanden ook koppelen aan geboekte inkoop- en verkoopdocumenten en aan leveranciers-, klant- en grootboekposten door het feitenblok **Inkomende documentbestanden** te gebruiken, bijvoorbeeld in het venster **Geboekte inkoopfacturen** en het venster **Leveranciersposten**.</span><span class="sxs-lookup"><span data-stu-id="8a50f-106">You can also attach incoming document files to posted purchase and sales documents and to vendor, customer, and general ledger entries by using the **Incoming Document Files** FactBox in, for example, the **Posted Purchase Invoices** and **Vendor Ledger Entries** windows.</span></span>

<span data-ttu-id="8a50f-107">Vanuit de vensters **Rekeningschema** en **Grootboekposten** kunt u zoeken naar grootboekposten voor geboekte inkoop- en verkoopdocumenten die geen inkomende documentrecords hebben, en deze centraal koppelen aan bestaande records of nieuwe records maken met gekoppelde documentbestanden.</span><span class="sxs-lookup"><span data-stu-id="8a50f-107">From the **Chart of Accounts** and **General Ledger Entries** windows, you can use a search function to find general ledger entries for posted purchase and sales documents that do not have incoming document records and then centrally link to existing records or create new ones with attached document files.</span></span> <span data-ttu-id="8a50f-108">Zie [Geboekte documenten zonder inkomende documentrecords zoeken](across-how-find-posted-documents-without-income-document-records.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="8a50f-108">For more information, see [Find Posted Documents without Incoming Document Records](across-how-find-posted-documents-without-income-document-records.md).</span></span>

<span data-ttu-id="8a50f-109">In de volgende procedures wordt beschreven hoe u een bestand koppelt aan een bestaande inkoopfactuur die niet van een inkomende documentrecord is gemaakt, en hoe u een bestand koppelt aan een leverancierspost.</span><span class="sxs-lookup"><span data-stu-id="8a50f-109">The following procedures show how to attach a file to an existing purchase invoice that was not created from an incoming document record and how to attach a file to a vendor ledger entry.</span></span> <span data-ttu-id="8a50f-110">Het koppelen van een bestand aan geboekte inkoop- of verkoopdocumenten werkt op dezelfde wijze.</span><span class="sxs-lookup"><span data-stu-id="8a50f-110">Attaching a file to posted purchase or sales documents works in a similar way.</span></span>

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a><span data-ttu-id="8a50f-111">Een inkomende documentrecord maken van een inkoopfactuur en koppelen</span><span class="sxs-lookup"><span data-stu-id="8a50f-111">To create and connect an incoming document record from a purchase invoice</span></span>
1. <span data-ttu-id="8a50f-112">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopfacturen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8a50f-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchase Invoices**, and then choose the related link.</span></span>
2. <span data-ttu-id="8a50f-113">Selecteer de regel voor een inkoopfactuur waaraan u een bestand wilt koppelen en kies vervolgens de actie **Inkomend document van bestand maken**.</span><span class="sxs-lookup"><span data-stu-id="8a50f-113">Select the line for a purchase invoice that you want to attach a file to, and then choose the **Create Incoming Document from File** action.</span></span>
3. <span data-ttu-id="8a50f-114">U kunt ook de regel voor een inkoopfactuur selecteren waaraan u een bestand wilt koppelen en vervolgens de actie **Bestand koppelen** kiezen.</span><span class="sxs-lookup"><span data-stu-id="8a50f-114">Alternatively, select the line for a purchase invoice that you want to attach a file to, and then choose the **Attach File** action.</span></span>
4. <span data-ttu-id="8a50f-115">In het venster **Bestand invoegen**, selecteert u het bestand dat het betreffende inkomende document vertegenwoordigt. Kies vervolgens de knop **Openen**.</span><span class="sxs-lookup"><span data-stu-id="8a50f-115">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a><span data-ttu-id="8a50f-116">Een inkomende documentrecord maken van een leverancierspost en koppelen</span><span class="sxs-lookup"><span data-stu-id="8a50f-116">To create and connect an incoming document record from a vendor ledger entry</span></span>
1. <span data-ttu-id="8a50f-117">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciersposten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8a50f-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Ledger Entries**, and then choose the related link.</span></span>
2. <span data-ttu-id="8a50f-118">Selecteer een regel voor een leverancierspost waaraan u een bestand wilt koppelen en kies vervolgens de actie **Inkomend document van bestand maken**.</span><span class="sxs-lookup"><span data-stu-id="8a50f-118">Select a line for a vendor ledger entry that you want to attach a file to, and then choose the **Create Incoming Document from File** action.</span></span>
3. <span data-ttu-id="8a50f-119">U kunt ook een regel voor een leverancierspost selecteren waaraan u een bestand wilt koppelen en vervolgens de actie **Bestand koppelen** kiezen.</span><span class="sxs-lookup"><span data-stu-id="8a50f-119">Alternatively, select a line for a vendor ledger entry that you want to attach a file to, and then choose the **Attach File** action.</span></span>
4. <span data-ttu-id="8a50f-120">In het venster **Bestand invoegen**, selecteert u het bestand dat het betreffende inkomende document vertegenwoordigt. Kies vervolgens de knop **Openen**.</span><span class="sxs-lookup"><span data-stu-id="8a50f-120">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a><span data-ttu-id="8a50f-121">De relatie van een inkomende documentrecord met een geboekt document verwijderen</span><span class="sxs-lookup"><span data-stu-id="8a50f-121">To remove a connection from an incoming document record to a posted document</span></span>
<span data-ttu-id="8a50f-122">U kunt bestandbijlagen van niet-geboekte documenten op elk moment verwijderen door de gerelateerde inkomende documentrecord te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8a50f-122">You can remove file attachments from non-posted documents at any time by deleting the related incoming document record.</span></span> <span data-ttu-id="8a50f-123">Als het document is geboekt, moet u eerst de relatie met de inkomende documentrecord verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8a50f-123">If the document is posted, then you must first remove the connection from the incoming document record.</span></span>

1. <span data-ttu-id="8a50f-124">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkomende documenten** en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8a50f-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="8a50f-125">Selecteer de regel voor een inkomende documentrecord die is verbonden met een geboekt document dat u wilt verwijderen en kies vervolgens de actie **Referentie naar record verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="8a50f-125">Select the line for an incoming document record connected to a posted document that you want to remove, and then choose the **Remove Reference to Record** action.</span></span>

<span data-ttu-id="8a50f-126">De verbinding met het geboekte document wordt verwijderd.</span><span class="sxs-lookup"><span data-stu-id="8a50f-126">The connection to the posted document is removed.</span></span> <span data-ttu-id="8a50f-127">U kunt nu doorgaan met het verbinden van een andere inkomende documentrecord met het geboekte document, zoals wordt beschreven in dit onderwerp.</span><span class="sxs-lookup"><span data-stu-id="8a50f-127">You can now proceed to connect another incoming document record to the posted document as described in this topic.</span></span>

## <a name="see-also"></a><span data-ttu-id="8a50f-128">Zie ook</span><span class="sxs-lookup"><span data-stu-id="8a50f-128">See Also</span></span>
[<span data-ttu-id="8a50f-129">Inkomende documenten verwerken</span><span class="sxs-lookup"><span data-stu-id="8a50f-129">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="8a50f-130">Inkomende documenten</span><span class="sxs-lookup"><span data-stu-id="8a50f-130">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="8a50f-131">Inkoop</span><span class="sxs-lookup"><span data-stu-id="8a50f-131">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="8a50f-132">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8a50f-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
