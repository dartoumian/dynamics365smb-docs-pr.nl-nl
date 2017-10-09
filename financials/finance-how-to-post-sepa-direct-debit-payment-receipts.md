---
title: SEPA-betalingen via automatische incasso boeken | Microsoft Docs
description: Wanneer een verzameling van automatische incasso wordt verwerkt door uw bank, kunt u doorgaan met het boeken van de ontvangst van de betaling voor de betrokken verkoopfacturen.
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 5beb5f6795bd7f4943a6ed9d8b691c05fc5ecb63
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-post-sepa-direct-debit-payment-receipts"></a><span data-ttu-id="3c62c-103">Procedure: SEPA-betalingsontvangsten via automatische incasso boeken</span><span class="sxs-lookup"><span data-stu-id="3c62c-103">How to: Post SEPA Direct Debit Payment Receipts</span></span>
<span data-ttu-id="3c62c-104">Wanneer een incasso-opdracht wordt verwerkt door uw bank, kunt u doorgaan met het boeken van de ontvangst van de betaling voor de betrokken verkoopfacturen.</span><span class="sxs-lookup"><span data-stu-id="3c62c-104">When a direct debit collection is successfully processed by your bank, you can proceed to post receipt of the payment for the involved sales invoices.</span></span> <span data-ttu-id="3c62c-105">Zie voor meer informatie [Procedure: SEPA-verzamelingsposten van automatische incasso maken en exporteren naar een bankbestand](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="3c62c-105">For more information, see [How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  

<span data-ttu-id="3c62c-106">U kunt de betalingsontvangst van het venster **Incasso-opdrachten** of het venster **Verzamelingsposten van incasso** direct boeken.</span><span class="sxs-lookup"><span data-stu-id="3c62c-106">You can post the payment receipt directly from the **Direct Debit Collections** window or the **Direct Debit Collect. Entries** window.</span></span> <span data-ttu-id="3c62c-107">U kunt ook het werk aan een andere gebruiker doorgeven door de dagboekregels voor te bereiden.</span><span class="sxs-lookup"><span data-stu-id="3c62c-107">Alternatively, you can relay the work to another user by preparing the related journal lines.</span></span>  

## <a name="to-post-a-direct-debit-payment-receipt-from-the-direct-debit-collections-window"></a><span data-ttu-id="3c62c-108">Een betalingsontvangst van een automatische incasso boeken vanuit het venster Verzamelingen van automatische incasso</span><span class="sxs-lookup"><span data-stu-id="3c62c-108">To post a direct-debit payment receipt from the Direct Debit Collections window</span></span>  
1. <span data-ttu-id="3c62c-109">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Incasso-opdrachten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="3c62c-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Direct Debit Collections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="3c62c-110">Selecteer een regel voor een verzameling automatische incasso die is geëxporteerd naar een bankbestand en verwerkt door de bank.</span><span class="sxs-lookup"><span data-stu-id="3c62c-110">Select a line for a direct debit collection that has been exported to a bank file and successfully processed by the bank.</span></span> <span data-ttu-id="3c62c-111">Zie voor meer informatie [Procedure: SEPA-verzamelingsposten van automatische incasso maken en exporteren naar een bankbestand](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span><span class="sxs-lookup"><span data-stu-id="3c62c-111">For more information, see [How to: Create SEPA Direct Debit Collection Entries and Export to a Bank File](finance-how-create-sepa-direct-debit-collection-entries-export-bank-file.md).</span></span>  
3. <span data-ttu-id="3c62c-112">Kies de actie **Betalingsontvangsten boeken**.</span><span class="sxs-lookup"><span data-stu-id="3c62c-112">Choose the **Post Payment Receipts** action.</span></span>  
4. <span data-ttu-id="3c62c-113">Vul in het venster **Incasso-opdracht boeken** de velden in, zoals is beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="3c62c-113">In the **Post Direct Debit Collection** window, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="3c62c-114">Veld</span><span class="sxs-lookup"><span data-stu-id="3c62c-114">Field</span></span>|<span data-ttu-id="3c62c-115">Description</span><span class="sxs-lookup"><span data-stu-id="3c62c-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="3c62c-116">**Incasso-opdrachtnr.**</span><span class="sxs-lookup"><span data-stu-id="3c62c-116">**Direct Debit Collection No.**</span></span>|<span data-ttu-id="3c62c-117">Geef de verzameling automatische incasso op waar u een betalingsontvangst voor wilt boeken.</span><span class="sxs-lookup"><span data-stu-id="3c62c-117">Specify the direct debit collection that you want to post payment receipt for.</span></span>|  
    |<span data-ttu-id="3c62c-118">**Algemeen dagboeksjabloon**</span><span class="sxs-lookup"><span data-stu-id="3c62c-118">**General Journal Template**</span></span>|<span data-ttu-id="3c62c-119">Geef op welk dagboeksjabloon te gebruiken voor het boeken van de betalingsontvangst, zoals de sjabloon voor ontvangsten.</span><span class="sxs-lookup"><span data-stu-id="3c62c-119">Specify which general journal template to use for posting the payment receipt, such as the template for cash receipts.</span></span>|  
    |<span data-ttu-id="3c62c-120">**Batchnaam financieel dagboek**</span><span class="sxs-lookup"><span data-stu-id="3c62c-120">**General Journal Batch Name**</span></span>|<span data-ttu-id="3c62c-121">Geef op welke dagboekbatch moet worden gebruikt voor het boeken van de betalingsontvangst.</span><span class="sxs-lookup"><span data-stu-id="3c62c-121">Specify which general journal batch to use for posting the payment receipt.</span></span>|  
    |<span data-ttu-id="3c62c-122">**Alleen dagboek aanmaken**</span><span class="sxs-lookup"><span data-stu-id="3c62c-122">**Create Journal Only**</span></span>|<span data-ttu-id="3c62c-123">Schakel dit selectievakje in als u niet de betalingsontvangst boeken wilt wanneer u de **OK** knop kiest.</span><span class="sxs-lookup"><span data-stu-id="3c62c-123">Select this check box if you do not want to post the payment receipt when you choose the **OK** button.</span></span> <span data-ttu-id="3c62c-124">De betalingsontvangst in het opgegeven dagboek wordt voorbereid en wordt niet geboekt totdat iemand de dagboekregels in kwestie boekt.</span><span class="sxs-lookup"><span data-stu-id="3c62c-124">The payment receipt will be prepared in the specified journal and will not be posted until someone posts the journal lines in question.</span></span>|  

5. <span data-ttu-id="3c62c-125">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="3c62c-125">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="3c62c-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="3c62c-126">See Also</span></span>  
 <span data-ttu-id="3c62c-127">[Betalingen verzamelen via automatische incasso van SEPA](finance-collect-payments-with-sepa-direct-debit.md) </span><span class="sxs-lookup"><span data-stu-id="3c62c-127">[Collect Payments with SEPA Direct Debit](finance-collect-payments-with-sepa-direct-debit.md) </span></span>  
 [<span data-ttu-id="3c62c-128">Verkoop</span><span class="sxs-lookup"><span data-stu-id="3c62c-128">Sales</span></span>](sales-manage-sales.md)
