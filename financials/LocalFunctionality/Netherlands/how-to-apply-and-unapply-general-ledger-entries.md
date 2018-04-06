---
title: Grootboekposten vereffenen en de vereffening ervan ongedaan maken
description: Door tijdelijke grootboekposten te vereffenen kunnen bedrijven werken met tijdelijke rekeningen en transferrekeningen in het grootboek. Tijdelijke en transferrekeningen worden gebruikt om tijdelijke posten op te slaan die op verdere verwerking in het grootboek wachten.
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
ms.openlocfilehash: 41f3eb9bc373759daf8bb025502b167c6494d978
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="apply-and-unapply-general-ledger-entries"></a><span data-ttu-id="f134b-104">Grootboekposten vereffenen en de vereffening ervan ongedaan maken</span><span class="sxs-lookup"><span data-stu-id="f134b-104">Apply and Unapply General Ledger Entries</span></span>
<span data-ttu-id="f134b-105">Door tijdelijke grootboekposten te vereffenen kunnen bedrijven werken met tijdelijke rekeningen en transferrekeningen in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="f134b-105">Applying temporary general ledger entries allows companies to work with temporary and transfer accounts in the general ledger.</span></span> <span data-ttu-id="f134b-106">Tijdelijke en transferrekeningen worden gebruikt om tijdelijke posten op te slaan die op verdere verwerking in het grootboek wachten.</span><span class="sxs-lookup"><span data-stu-id="f134b-106">Temporary and transfer accounts are used to store temporary ledger entries that are waiting for further processing into the general ledger.</span></span>  

<span data-ttu-id="f134b-107">U kunt tijdelijke rekeningen gebruiken voor:</span><span class="sxs-lookup"><span data-stu-id="f134b-107">You can use temporary accounts for:</span></span>  

- <span data-ttu-id="f134b-108">Geldtransfers van de ene naar de andere bankrekening.</span><span class="sxs-lookup"><span data-stu-id="f134b-108">Money transfers from one bank account to another.</span></span>  
- <span data-ttu-id="f134b-109">Financiële transactietransfers van het ene systeem naar het andere, waarbij een deel van de gegevens tijdelijk op het oorspronkelijke systeem staat.</span><span class="sxs-lookup"><span data-stu-id="f134b-109">Financial transaction transfers from one system to another in which part of the information temporarily resides on the original system.</span></span>  
- <span data-ttu-id="f134b-110">Transacties waarvoor u een verkoopfactuur hebt verzonden naar een klant maar nog niet de bijbehorende inkoopfactuur van de leverancier hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="f134b-110">Transactions for which you have issued a sales invoice to a customer but have not yet received the corresponding purchase invoice from the vendor.</span></span>  

<span data-ttu-id="f134b-111">Nadat de posten zijn verwerkt, kunt u de functie voor postenvereffening gebruiken om de geboekte posten en het boekingsrekeningsoort bij te werken.</span><span class="sxs-lookup"><span data-stu-id="f134b-111">When the ledger entries have been processed, you can use the apply entries function to update the posted ledger entries and the posting account type.</span></span>  

<span data-ttu-id="f134b-112">U kunt de vereffening van de vereffende grootboekposten ongedaan maken en vervolgens de gesloten posten openen om wijzigingen aan te brengen.</span><span class="sxs-lookup"><span data-stu-id="f134b-112">You can unapply the applied general ledger entries and then open the closed entries to make changes.</span></span>  

## <a name="to-apply-general-ledger-entries"></a><span data-ttu-id="f134b-113">Grootboekposten vereffenen</span><span class="sxs-lookup"><span data-stu-id="f134b-113">To apply general ledger entries</span></span>  

1.  <span data-ttu-id="f134b-114">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Grootboekjournalen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="f134b-114">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f134b-115">Selecteer een grootboekjournaal en kies vervolgens de actie **Grootboek**.</span><span class="sxs-lookup"><span data-stu-id="f134b-115">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="f134b-116">Kies in het venster **Grootboekposten** de actie **Posten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="f134b-116">In the **General Ledger Entries** window, choose the **Apply Entries** action.</span></span>  

    <span data-ttu-id="f134b-117">Alle openstaande posten voor de grootboekrekening worden weergegeven in het venster **Grootboekposten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="f134b-117">All open ledger entries for the general ledger account are displayed in the **Apply General Ledger Entries** window.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="f134b-118">Standaard wordt het veld **Posten opnemen** ingesteld op **Open**.</span><span class="sxs-lookup"><span data-stu-id="f134b-118">By default, the **Include Entries** field is set to **Open**.</span></span> <span data-ttu-id="f134b-119">U kunt de waarde van het veld **Posten opnemen** wijzigen in **Alle** of **Afgesloten**.</span><span class="sxs-lookup"><span data-stu-id="f134b-119">You can change the value of the **Include Entries** field to **All** or **Closed**.</span></span> <span data-ttu-id="f134b-120">U kunt alleen grootboekposten vereffenen die **open** zijn.</span><span class="sxs-lookup"><span data-stu-id="f134b-120">You can only apply general ledger entries that are **Open**.</span></span>  

4.  <span data-ttu-id="f134b-121">Selecteer de betreffende grootboekpost en kies de actie **Vereffenings-id instellen**.</span><span class="sxs-lookup"><span data-stu-id="f134b-121">Select the relevant general ledger entry, and then choose the **Set Applies-to ID** action.</span></span>  

    <span data-ttu-id="f134b-122">Het veld **Vereffenings-id** wordt bijgewerkt met de gebruikers-id.</span><span class="sxs-lookup"><span data-stu-id="f134b-122">The **Applies-to ID** field is updated with the user ID.</span></span> <span data-ttu-id="f134b-123">Het restbedrag wordt weergegeven in het veld **Saldo** in het venster **Grootboekposten vereffenen**.</span><span class="sxs-lookup"><span data-stu-id="f134b-123">The remaining amount is displayed in the **Balance** field in the **Apply General Ledger Entries** window.</span></span>  
5.  <span data-ttu-id="f134b-124">Kies de actie **Vereffening boeken**.</span><span class="sxs-lookup"><span data-stu-id="f134b-124">Choose the **Post Application** action.</span></span>  

    <span data-ttu-id="f134b-125">U kunt de vereffening boeken zelfs wanneer het saldobedrag gelijk is aan 0.</span><span class="sxs-lookup"><span data-stu-id="f134b-125">You can post the application even if the balance amount is equal to 0.</span></span> <span data-ttu-id="f134b-126">Wanneer wordt geboekt, wordt het veld **Restbedrag** als volgt beïnvloed:</span><span class="sxs-lookup"><span data-stu-id="f134b-126">When posted, the **Remaining Amount** field is affected as follows:</span></span>  

    - <span data-ttu-id="f134b-127">Als het veld **Saldo** gelijk is aan 0, wordt het veld **Restbedrag** bij alle grootboekposten op 0 gezet.</span><span class="sxs-lookup"><span data-stu-id="f134b-127">If the **Balance** is equal to 0, then the **Remaining Amount** field on all ledger entries is set to 0.</span></span>  

    - <span data-ttu-id="f134b-128">Als het veld **Saldo** niet gelijk is aan 0, wordt het bedrag in het veld **Saldo** overgebracht naar het veld **Restbedrag** van de grootboekpost die was geselecteerd toen u de vereffening boekte.</span><span class="sxs-lookup"><span data-stu-id="f134b-128">If the **Balance** is not equal to 0, then the amount in the **Balance** field is transferred to the **Remaining Amount** field for the general ledger entry that was selected when you posted the application.</span></span>  

    - <span data-ttu-id="f134b-129">Voor alle overige grootboekposten wordt het veld **Restbedrag** op 0 gezet en worden de velden **Open**, **Afgesloten door volgnr.**, **Afgesloten met bedrag** en **Afgesloten op** bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="f134b-129">For all other general ledger entries, the **Remaining Amount** field is set to 0 and the **Open**, **Closed by Entry No.**, **Closed by Amount**, and **Closed at Date** fields are updated.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="f134b-130">Wanneer wordt geboekt, worden de grootboekposten die het veld **Vereffenings-id** bijwerken, verwijderd.</span><span class="sxs-lookup"><span data-stu-id="f134b-130">When posted, the general ledger entries which update the **Applies-to ID** field are deleted.</span></span>  

6.  <span data-ttu-id="f134b-131">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f134b-131">Choose the **OK** button.</span></span>  

## <a name="to-view-the-applied-general-ledger-entries"></a><span data-ttu-id="f134b-132">De vereffende grootboekposten weergeven</span><span class="sxs-lookup"><span data-stu-id="f134b-132">To view the applied general ledger entries</span></span>  

1.  <span data-ttu-id="f134b-133">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Grootboekjournalen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="f134b-133">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f134b-134">Selecteer een grootboekjournaal en kies vervolgens de actie **Grootboek**.</span><span class="sxs-lookup"><span data-stu-id="f134b-134">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="f134b-135">Selecteer de betreffende grootboekpost en kies de actie **Vereffende posten**.</span><span class="sxs-lookup"><span data-stu-id="f134b-135">Select the relevant general ledger entry, and then choose the **Applied Entries** action.</span></span>  

    <span data-ttu-id="f134b-136">U kunt alle vereffende grootboekposten weergeven.</span><span class="sxs-lookup"><span data-stu-id="f134b-136">You can view all the applied general ledger entries.</span></span>  

4.  <span data-ttu-id="f134b-137">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f134b-137">Choose the **OK** button.</span></span>  

## <a name="to-unapply-general-ledger-entries"></a><span data-ttu-id="f134b-138">De vereffening van grootboekposten ongedaan maken</span><span class="sxs-lookup"><span data-stu-id="f134b-138">To unapply general ledger entries</span></span>  

1.  <span data-ttu-id="f134b-139">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Grootboekjournalen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="f134b-139">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Registers**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="f134b-140">Selecteer een grootboekjournaal en kies vervolgens de actie **Grootboek**.</span><span class="sxs-lookup"><span data-stu-id="f134b-140">Select a general ledger register, and then choose the **General Ledger** action.</span></span>  
3.  <span data-ttu-id="f134b-141">Selecteer de grootboekpost waarvan u de vereffening ongedaan wilt maken en kies vervolgens de actie **Vereffening ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="f134b-141">Select the general ledger entry that you want to unapply, and then choose the **Undo Application** action.</span></span>  

    <span data-ttu-id="f134b-142">De vereffening van de vereffende grootboekposten wordt ongedaan gemaakt.</span><span class="sxs-lookup"><span data-stu-id="f134b-142">The applied general ledger entries are unapplied.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="f134b-143">Als een post is vereffend met meer dan één vereffeningspost, moet u de vereffening van de laatste vereffeningspost het eerst ongedaan maken.</span><span class="sxs-lookup"><span data-stu-id="f134b-143">If an entry is applied to more than one application entry, you must unapply the latest application entry first.</span></span> <span data-ttu-id="f134b-144">Standaard wordt de laatste post weergegeven.</span><span class="sxs-lookup"><span data-stu-id="f134b-144">By default, the latest entry is displayed.</span></span>  

4.  <span data-ttu-id="f134b-145">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f134b-145">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f134b-146">Zie ook</span><span class="sxs-lookup"><span data-stu-id="f134b-146">See Also</span></span>  
[<span data-ttu-id="f134b-147">Grootboek</span><span class="sxs-lookup"><span data-stu-id="f134b-147">General Ledger</span></span>](general-ledger.md)
