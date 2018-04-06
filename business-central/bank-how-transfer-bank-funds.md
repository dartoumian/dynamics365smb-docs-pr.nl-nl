---
title: Bankfondsen overboeken| Microsoft Docs
description: U kunt bedragen overbrengen van de ene naar de andere bankrekening, inclusief andere valuta's, door de transactie in het dagboek te boeken.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bank account transfer, multiple currencies
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 54e8a7bf7ca8761d6317b57d45e64f9ee628f4b8
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="transfer-bank-funds"></a><span data-ttu-id="305b1-103">Bankfondsen overboeken</span><span class="sxs-lookup"><span data-stu-id="305b1-103">Transfer Bank Funds</span></span>
<span data-ttu-id="305b1-104">Soms moet u een transfer van een bedrag van de ene naar de andere bankrekening boeken.</span><span class="sxs-lookup"><span data-stu-id="305b1-104">You may sometimes need to transfer an amount from one bank account to another.</span></span> <span data-ttu-id="305b1-105">Als u dit wilt doen, moet u een transactie boeken in het dagboek.</span><span class="sxs-lookup"><span data-stu-id="305b1-105">To do this, you must post the a transaction in the general journal.</span></span> <span data-ttu-id="305b1-106">De taak verschilt afhankelijk van of de bankrekeningen dezelfde valuta gebruiken of niet.</span><span class="sxs-lookup"><span data-stu-id="305b1-106">The task varies depending on whether the bank accounts use the same currency or different currencies.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a><span data-ttu-id="305b1-107">Een transfer boeken tussen bankrekeningen met dezelfde valutacode</span><span class="sxs-lookup"><span data-stu-id="305b1-107">To post a transfer between bank accounts with the same currency code</span></span>
1. <span data-ttu-id="305b1-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Diversendagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="305b1-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="305b1-109">Vul op een dagboekregel de velden **Boekingsdatum** en **Documentnr.** in.</span><span class="sxs-lookup"><span data-stu-id="305b1-109">On a journal line, fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="305b1-110">Selecteer in het veld **Rekeningsoort** de optie **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="305b1-110">In the **Account Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="305b1-111">Selecteer in het veld **Rekeningnr.** de bankrekening waarvan u de fondsen wilt overbrengen.</span><span class="sxs-lookup"><span data-stu-id="305b1-111">In the **Account No.** field, select the bank from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="305b1-112">Voer in het veld **Bedrag** het bedrag in dat u wilt overbrengen.</span><span class="sxs-lookup"><span data-stu-id="305b1-112">In the **Amount** field, enter the amount to be transferred.</span></span>
6. <span data-ttu-id="305b1-113">Selecteer in het veld **Tegenrekeningtype** **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="305b1-113">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="305b1-114">Selecteer in het veld **Tegenrekeningnr.** de bankrekening waarnaar u de fondsen wilt overbrengen.</span><span class="sxs-lookup"><span data-stu-id="305b1-114">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="305b1-115">Boek het dagboek.</span><span class="sxs-lookup"><span data-stu-id="305b1-115">Post the journal.</span></span>

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a><span data-ttu-id="305b1-116">Transfers boeken tussen bankrekeningen met verschillende valutacodes</span><span class="sxs-lookup"><span data-stu-id="305b1-116">To post a transfer between bank accounts with different currency codes</span></span>
<span data-ttu-id="305b1-117">Als u gelden wilt overbrengen tussen bankrekeningen die verschillende valuta's gebruiken, moet u twee dagboekregels boeken.</span><span class="sxs-lookup"><span data-stu-id="305b1-117">To transfer funds between bank accounts that use different currencies, you must post two general journal lines.</span></span>

1. <span data-ttu-id="305b1-118">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Diversendagboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="305b1-118">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="305b1-119">Maak twee dagboekregels en vul de velden **Boekingsdatum** en **Documentnr.** in.</span><span class="sxs-lookup"><span data-stu-id="305b1-119">Create two journal lines, and fill in the **Posting Date** and **Document No.** fields.</span></span>
3. <span data-ttu-id="305b1-120">Selecteer op de eerste dagboekregel **Bankrekening** in het veld **Soort**.</span><span class="sxs-lookup"><span data-stu-id="305b1-120">On the first journal line, in the **Type** field, select **Bank Account**.</span></span>
4. <span data-ttu-id="305b1-121">Selecteer in het veld **Rekeningnr.** de bankrekening waarvan u de fondsen wilt overbrengen.</span><span class="sxs-lookup"><span data-stu-id="305b1-121">In the **Account No.** field, select the bank account from which you want to transfer the funds.</span></span>
5. <span data-ttu-id="305b1-122">Voer in het veld **Bedrag** het bedrag in de valuta van de bankrekening in.</span><span class="sxs-lookup"><span data-stu-id="305b1-122">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="305b1-123">Voer creditbedragen met een minteken in.</span><span class="sxs-lookup"><span data-stu-id="305b1-123">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="305b1-124">Voer debetbedragen zonder een minteken in.</span><span class="sxs-lookup"><span data-stu-id="305b1-124">Enter debit amounts without a minus sign.</span></span>
6. <span data-ttu-id="305b1-125">Selecteer in het veld **Tegenrekeningtype** **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="305b1-125">In the **Bal. Account Type** field, select **Bank Account**.</span></span>
7. <span data-ttu-id="305b1-126">Selecteer in het veld **Tegenrekeningnr.** de bankrekening waarnaar u de fondsen wilt overbrengen.</span><span class="sxs-lookup"><span data-stu-id="305b1-126">In the **Bal. Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
8. <span data-ttu-id="305b1-127">Selecteer op de tweede dagboekregel **Bankrekening** in het veld **Soort**.</span><span class="sxs-lookup"><span data-stu-id="305b1-127">On the second journal line, in the **Type** field, select **Bank Account**.</span></span>
9. <span data-ttu-id="305b1-128">Selecteer in het veld **Rekeningnr.** de bankrekening waarnaar u de fondsen wilt overbrengen.</span><span class="sxs-lookup"><span data-stu-id="305b1-128">In the **Account No.** field, select the bank account to which you want to transfer the funds.</span></span>
10. <span data-ttu-id="305b1-129">Voer in het veld **Bedrag** het bedrag in de valuta van de bankrekening in.</span><span class="sxs-lookup"><span data-stu-id="305b1-129">In the **Amount** field, enter the amount in the currency of the bank account.</span></span> <span data-ttu-id="305b1-130">Voer creditbedragen met een minteken in.</span><span class="sxs-lookup"><span data-stu-id="305b1-130">Enter credit amounts with a minus sign.</span></span> <span data-ttu-id="305b1-131">Voer debetbedragen zonder een minteken in.</span><span class="sxs-lookup"><span data-stu-id="305b1-131">Enter debit amounts without a minus sign.</span></span>
11. <span data-ttu-id="305b1-132">Selecteer in het veld **Tegenrekeningtype** **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="305b1-132">In the **Bal. Account Type** field, select **Bank Account**.</span></span>  
12. <span data-ttu-id="305b1-133">Selecteer in het veld **Tegenrekeningnr.** de bankrekening waarvan u de fondsen wilt overbrengen.</span><span class="sxs-lookup"><span data-stu-id="305b1-133">In the **Bal. Account No.** field, select the bank account from which you want to transfer the funds.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="305b1-134">Als de gebruikte wisselkoersen in het dagboek verschillen van de wisselkoersen in het venster **Valutawisselkoersen**, voert u een derde regel in voor de wisselkoerswinsten of -verliezen.</span><span class="sxs-lookup"><span data-stu-id="305b1-134">If the exchange rates used in the journal are different than the exchange rates in the **Currency Exchange Rates** window, enter a third line for the exchange rate gain or loss.</span></span> <span data-ttu-id="305b1-135">Geef **Grootboekrekening** op in het veld **Rekeningsoort**.</span><span class="sxs-lookup"><span data-stu-id="305b1-135">Enter **G/L Account** in the **Account Type** field.</span></span> <span data-ttu-id="305b1-136">Voer in het veld **Rekeningnr.** het grootboekrekeningnummer voor wisselkoerswinst of -verlies in.</span><span class="sxs-lookup"><span data-stu-id="305b1-136">Enter the G/L account number for exchange rate gain or loss in the **Account No.** field.</span></span> <span data-ttu-id="305b1-137">Voer de wisselkoerswinst of - verlies in het veld **Bedrag** in met of zonder een minteken voor respectievelijk debet- en creditbedragen.</span><span class="sxs-lookup"><span data-stu-id="305b1-137">Enter the exchange rate gain or loss in the **Amount** field with or without a minus sign for credits and debits respectively.</span></span>
13. <span data-ttu-id="305b1-138">Boek het dagboek.</span><span class="sxs-lookup"><span data-stu-id="305b1-138">Post the journal.</span></span>

## <a name="see-also"></a><span data-ttu-id="305b1-139">Zie ook</span><span class="sxs-lookup"><span data-stu-id="305b1-139">See Also</span></span>
[<span data-ttu-id="305b1-140">Bankrekeningen beheren</span><span class="sxs-lookup"><span data-stu-id="305b1-140">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="305b1-141">Bankieren instellen</span><span class="sxs-lookup"><span data-stu-id="305b1-141">Setting Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="305b1-142">Werken met diversendagboeken</span><span class="sxs-lookup"><span data-stu-id="305b1-142">Working with General Journals</span></span>](ui-work-general-journals.md)  
<span data-ttu-id="305b1-143">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="305b1-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
