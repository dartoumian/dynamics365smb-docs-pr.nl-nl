---
title: Posten vereffenen in verschillende valuta's| Microsoft Docs
description: U kunt posten in meerdere valuta's vereffenen, bijvoorbeeld als u verkoopt in een bepaalde valuta en een betaling in een andere ontvangt.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 01/25/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 960ae581a3f933c6e9c2ed5183944ddf62ca5965
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="302b4-103">Vereffening van posten in verschillende valuta's inschakelen</span><span class="sxs-lookup"><span data-stu-id="302b4-103">Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="302b4-104">Als de betaling in een andere valuta dan de valuta van de inkoop wordt ingediend, kunt u de betaling met de inkoop vereffenen.</span><span class="sxs-lookup"><span data-stu-id="302b4-104">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="302b4-105">Als u aan een klant verkoopt in een bepaalde valuta en een betaling in een andere valuta ontvangt, kunt u de betaling ook vereffenen met de verkoopfactuur.</span><span class="sxs-lookup"><span data-stu-id="302b4-105">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="302b4-106">In de volgende procedure wordt beschreven hoe u dit instelt voor leveranciersposten in het venster **Inkoopinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="302b4-106">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span></span> <span data-ttu-id="302b4-107">De instelling is soortgelijk voor klantenposten in het venster **Verkoopinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="302b4-107">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="302b4-108">Vereffening van leveranciersposten in verschillende valuta's inschakelen</span><span class="sxs-lookup"><span data-stu-id="302b4-108">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="302b4-109">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopinstellingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="302b4-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="302b4-110">Selecteer een van de volgende opties in het veld **Valuta's vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="302b4-110">In the **Appln. between Currencies** field, select one of the following options.</span></span>

| <span data-ttu-id="302b4-111">Optie</span><span class="sxs-lookup"><span data-stu-id="302b4-111">Option</span></span> | <span data-ttu-id="302b4-112">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="302b4-112">Description</span></span> |
| --- | --- |
| <span data-ttu-id="302b4-113">Geen</span><span class="sxs-lookup"><span data-stu-id="302b4-113">None</span></span> |<span data-ttu-id="302b4-114">De vereffening tussen valuta's is niet toegestaan.</span><span class="sxs-lookup"><span data-stu-id="302b4-114">Application between currencies is not allowed.</span></span> |
| <span data-ttu-id="302b4-115">EMU</span><span class="sxs-lookup"><span data-stu-id="302b4-115">EMU</span></span> |<span data-ttu-id="302b4-116">De vereffening tussen EMU-valuta's is toegestaan.</span><span class="sxs-lookup"><span data-stu-id="302b4-116">Application between EMU currencies is allowed.</span></span> |
| <span data-ttu-id="302b4-117">Alle</span><span class="sxs-lookup"><span data-stu-id="302b4-117">All</span></span> |<span data-ttu-id="302b4-118">De vereffening tussen alle valuta's is toegestaan.</span><span class="sxs-lookup"><span data-stu-id="302b4-118">Application between all currencies is allowed.</span></span> |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a><span data-ttu-id="302b4-119">Grootboekrekeningen voor afrondingsverschillen bij valutaberekeningen instellen</span><span class="sxs-lookup"><span data-stu-id="302b4-119">To set up G/L accounts for currency application rounding differences</span></span>  
<span data-ttu-id="302b4-120">Als u posten in verschillende valuta's vereffent, moet u instellen naar welke grootboekrekening u de afrondingsverschillen wilt boeken.</span><span class="sxs-lookup"><span data-stu-id="302b4-120">If you apply entries in different currencies, you must set up the general ledger accounts to which you want to post rounding differences.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="302b4-121">U moet de grootboekrekeningen instellen voordat u de taak kunt voltooien.</span><span class="sxs-lookup"><span data-stu-id="302b4-121">You must set up the general ledger accounts before you complete the task.</span></span> <span data-ttu-id="302b4-122">Zie voor meer informatie [Het grootboek en het rekeningschema begrijpen](finance-general-ledger.md).</span><span class="sxs-lookup"><span data-stu-id="302b4-122">For more information, see [Understanding the General Ledger and the Chart of Accounts](finance-general-ledger.md).</span></span>

1. <span data-ttu-id="302b4-123">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Klantboekingsgroepen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="302b4-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Customer Posting Groups**, and then choose the related link.</span></span>  
2. <span data-ttu-id="302b4-124">In de velden **Afr.-rek. valutavereff. (Deb.)** en  **Afr.-rek. val.-vereff. (Cred.)** voert u de grootboekrekeningen waarnaar u de afrondingsverschillen wilt boeken in.</span><span class="sxs-lookup"><span data-stu-id="302b4-124">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  
3. <span data-ttu-id="302b4-125">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciersboekingsgroepen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="302b4-125">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendor Posting Groups**, and then choose the related link.</span></span>  
4. <span data-ttu-id="302b4-126">In de velden **Afr.-rek. valutavereff. (Deb.)** en  **Afr.-rek. val.-vereff. (Cred.)** voert u de grootboekrekeningen waarnaar u de afrondingsverschillen wilt boeken in.</span><span class="sxs-lookup"><span data-stu-id="302b4-126">In the **Debit Curr. Appln. Rndg. Acc.** and **Credit Curr. Appln. Rndg. Acc.** fields, enter the relevant general ledger accounts to post rounding differences.</span></span>  

## <a name="see-also"></a><span data-ttu-id="302b4-127">Zie ook</span><span class="sxs-lookup"><span data-stu-id="302b4-127">See Also</span></span>
[<span data-ttu-id="302b4-128">Betalingsverplichtingen beheren</span><span class="sxs-lookup"><span data-stu-id="302b4-128">Managing Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="302b4-129">Tegoeden beheren</span><span class="sxs-lookup"><span data-stu-id="302b4-129">Managing Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="302b4-130">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="302b4-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
