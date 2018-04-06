---
title: Verkoopopportunities verwerken in verkoopcycli| Microsoft Docs
description: U kunt verkoopopportunities weergeven sluiten of verwijderen en u kunt ook offertes en verkooporders voor opportunity's maken en een opportunity verplaatsen door de fasen van een verkoopcyclus.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: c7c7dca1d59b407f119347345cbbdef3f730acbc
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="process-sales-opportunities"></a><span data-ttu-id="7bb2b-103">Verkoopopportunity's verwerken</span><span class="sxs-lookup"><span data-stu-id="7bb2b-103">Process Sales Opportunities</span></span>
<span data-ttu-id="7bb2b-104">Nadat u een opportunity hebt gemaakt, zijn er verschillende functies voor het beheren van de opportunity en het verplaatsen ervan naar voltooiing.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-104">After you create an opportunity, there are several features for managing the opportunity and moving it through to completion.</span></span>

## <a name="to-view-opportunities"></a><span data-ttu-id="7bb2b-105">Opportunities weergeven</span><span class="sxs-lookup"><span data-stu-id="7bb2b-105">To view opportunities</span></span>
<span data-ttu-id="7bb2b-106">De bestaande verkoopopportunities zijn beschikbaar in het venster **Opportunity-overzicht**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-106">The existing sale opportunities are available from the **Opportunity List** window.</span></span> <span data-ttu-id="7bb2b-107">Er zijn verschillende manieren om toegang tot dit venster te krijgen om verkoopopportunities te verwerken:</span><span class="sxs-lookup"><span data-stu-id="7bb2b-107">There are different ways to access this window for processing sales opportunities:</span></span>

| <span data-ttu-id="7bb2b-108">Opportunities weergeven voor</span><span class="sxs-lookup"><span data-stu-id="7bb2b-108">To view opportunities for</span></span> | <span data-ttu-id="7bb2b-109">Dan</span><span class="sxs-lookup"><span data-stu-id="7bb2b-109">Then</span></span> |
| --- | --- |
| <span data-ttu-id="7bb2b-110">Alle verkopers en contacten</span><span class="sxs-lookup"><span data-stu-id="7bb2b-110">All salespeople and contacts</span></span> |<span data-ttu-id="7bb2b-111">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Opportunity-overzicht** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Opportunity List**, and then choose the related link.</span></span> |
| <span data-ttu-id="7bb2b-112">Een bepaalde verkoper</span><span class="sxs-lookup"><span data-stu-id="7bb2b-112">A specific sales person</span></span> |<span data-ttu-id="7bb2b-113">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Verkopers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Salespeople**, and then choose the related link.</span></span> <span data-ttu-id="7bb2b-114">Selecteer de verkoper, kies de actie **Opportunities** en kies vervolgens de actie **Overzicht**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-114">Select the salesperson, choose the **Opportunities** action, and then choose the **List** action.</span></span> |
| <span data-ttu-id="7bb2b-115">Een bepaald contact</span><span class="sxs-lookup"><span data-stu-id="7bb2b-115">A specific contact</span></span> |<span data-ttu-id="7bb2b-116">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Contacten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contacts**, and then choose the related link.</span></span> <span data-ttu-id="7bb2b-117">Selecteer het contact in de lijst en kies vervolgens de actie **Opportunities**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-117">Select the contact from the list, and then choose the **Opportunities** action.</span></span> |

<span data-ttu-id="7bb2b-118">Al deze taken openen het venster **Opportunity-overzicht**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-118">Each of these tasks opens the **Opportunity List** window.</span></span>

## <a name="to-close-opportunities"></a><span data-ttu-id="7bb2b-119">Opportunities sluiten</span><span class="sxs-lookup"><span data-stu-id="7bb2b-119">To close opportunities</span></span>
<span data-ttu-id="7bb2b-120">U kunt opportunities afsluiten wanneer de onderhandelingen zijn afgerond.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-120">You can close opportunities when the negotiations are over.</span></span> <span data-ttu-id="7bb2b-121">Wanneer u een opportunity afsluit, kunt u opgeven of de opportunity is gewonnen of verloren en de redenen voor het afsluiten.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-121">When closing an opportunity, you can specify whether it was won or lost, and the reasons for closing it.</span></span> <span data-ttu-id="7bb2b-122">Als u een reden wilt opgeven, moet u codes voor gesloten opportunities instellen.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-122">To specify a reason, you must set up closed opportunity codes.</span></span>

1. <span data-ttu-id="7bb2b-123">Selecteer in het venster **Opportunity-overzicht** de opportunity en kies de actie **Sluiten**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-123">In the **Opportunity List** window, select the opportunity, and the choose the **Close** action.</span></span> <span data-ttu-id="7bb2b-124">Het venster **Opportunity afsluiten** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-124">The **Close Opportunity** window opens.</span></span>
2. <span data-ttu-id="7bb2b-125">Vul de relevante velden in en kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-125">Fill in the relevant fields, and then choose the **OK** button.</span></span>

   <span data-ttu-id="7bb2b-126">De velden **Opportunitycode afsluiten** en **Datum afgesloten** zijn vereiste velden en moeten worden ingevuld voordat u de knop **OK** kunt kiezen.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-126">The **Close Opportunity Code** and **Date Closed** fields are required fields and must be filled in before you can choose the **OK** button.</span></span>

   <span data-ttu-id="7bb2b-127">In het veld **Opportunitycode afsluiten** kunt u een van de bestaande codes voor het sluiten van opportunities kiezen of een nieuwe code toevoegen.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-127">In the **Close Opportunity Code** field, you can choose from one of the existing close opportunity codes or add a new code.</span></span> <span data-ttu-id="7bb2b-128">Als u een nieuwe code wilt toevoegen, kiest u in de vervolgkeuzelijst **Selecteren vanuit volledige lijst** en kiest u vervolgens **nieuw**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-128">To add a new code, from the drop-down list, choose **Select from full list**, and then choose **new**.</span></span> <span data-ttu-id="7bb2b-129">Vul op de nieuwe, lege regel de velden **Code**, **Soort** en **Omschrijving** in en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-129">On the new blank line, fill in the **Code**, **Type**, and **Description** fields, and then choose the **OK** button.</span></span>

## <a name="to-create-quotes-for-opportunities"></a><span data-ttu-id="7bb2b-130">Offertes maken voor opportunity's</span><span class="sxs-lookup"><span data-stu-id="7bb2b-130">To create quotes for opportunities</span></span>
<span data-ttu-id="7bb2b-131">U kunt verkoopoffertes maken voor contactpersonen die niet zijn geregistreerd als klant.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-131">You can create sales quotes for contacts that are not recorded as customers.</span></span>

1. <span data-ttu-id="7bb2b-132">Selecteer in het venster **Opportunity-overzicht** de opportunity en kies vervolgens de actie **Verkoopofferte toekennen**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-132">In the **Opportunity List** window, select the opportunity, and then choose the **Assign Sales Quote** action.</span></span> <span data-ttu-id="7bb2b-133">Het venster **Verkoopofferte** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-133">The **Sales Quote** window opens.</span></span>
2. <span data-ttu-id="7bb2b-134">Vul de betreffende velden in.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-134">Fill in the relevant fields.</span></span>

## <a name="to-create-sales-orders-for-opportunities"></a><span data-ttu-id="7bb2b-135">Verkooporders voor opportunity's maken</span><span class="sxs-lookup"><span data-stu-id="7bb2b-135">To create sales orders for opportunities</span></span>
<span data-ttu-id="7bb2b-136">U kunt verkooporders maken van de verkoopoffertes die u hebt gemaakt voor de opportunities.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-136">You can make sales orders from the sales quotes that you have created for your opportunities.</span></span> <span data-ttu-id="7bb2b-137">Voordat u verkooporders voor uw contacten kunt maken, moet u het contact eerst als klant maken.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-137">Before you can create sales orders for your contacts, you must create the contact as a customer.</span></span> <span data-ttu-id="7bb2b-138">Zie voor meer informatie [Een klant, leverancier of bankrekening maken van een contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="7bb2b-138">For more information, see [Create a Customer, Vendor, or Bank Account From a Contact](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).</span></span>

1. <span data-ttu-id="7bb2b-139">Zoek in het venster **Opportunity-overzicht** de opportunity waarvoor u een verkoopofferte hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-139">In the **Opportunity List** window, find the opportunity that you have created a sales quote for.</span></span>
2. <span data-ttu-id="7bb2b-140">Kies de actie **Verkoopofferte toekennen**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-140">Choose the **Assign Sales Quote** action.</span></span> <span data-ttu-id="7bb2b-141">Het venster **Verkoopofferte** wordt geopend met de verkoopofferte die u aan de opportunity hebt toegewezen.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-141">The **Sales Quote** window opens to show the sales quote that you have assigned to the opportunity.</span></span>
3. <span data-ttu-id="7bb2b-142">Vul de extra velden in en kies vervolgens de actie **Order maken**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-142">Fill in the additional fields, and then choose the **Make Order** action.</span></span>

<span data-ttu-id="7bb2b-143">Wanneer u verkoopopportunities verwerkt, moet u wellicht een offerte maken voor het contact aan wie de opportunity is gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-143">When handling sales opportunities, you may need to create a quote for the contact that the opportunity is linked to.</span></span>

## <a name="to-delete-opportunities"></a><span data-ttu-id="7bb2b-144">Opportunities verwijderen</span><span class="sxs-lookup"><span data-stu-id="7bb2b-144">To delete opportunities</span></span>
<span data-ttu-id="7bb2b-145">U kunt opportunities verwijderen, bijvoorbeeld nadat u een verkoop hebt afgesloten.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-145">You can delete opportunities, for example, after you have concluded a deal.</span></span> <span data-ttu-id="7bb2b-146">U kunt echter alleen gesloten opportunities verwijderen.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-146">However, you can only delete closed opportunities.</span></span> <span data-ttu-id="7bb2b-147">Er zijn twee manieren om afgesloten opportunities te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-147">There are two ways to delete closed opportunities.</span></span> <span data-ttu-id="7bb2b-148">U kunt individuele afgesloten opportunities verwijderen vanuit het venster **Opportunity-overzicht** of u kunt de batchverwerking **Afgesloten opportunities verwijderen** uitvoeren om meerdere opportunities te verwijderen op basis van een opgegeven criterium.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-148">You can delete individual closed opportunities from the **Opportunity List** window or you can run the **Delete Closed Opportunities** batch job to delete multiple opportunities based on a specified criteria.</span></span>

<span data-ttu-id="7bb2b-149">Als u gesloten afgesloten opportunities wilt verwijderen vanuit het venster **Opportunity-overzicht**, selecteert u de opportunity, en kiest u vervolgens de actie **Verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-149">To delete closed opportunities from the **Opportunity List** window, select the opportunity, and then choose the **Delete** action.</span></span>

<span data-ttu-id="7bb2b-150">Als u afgesloten opportunities wilt verwijderen met de batchverwerking **Afgesloten opportunities verwijderen**, volgt u deze stappen:</span><span class="sxs-lookup"><span data-stu-id="7bb2b-150">To delete closed opportunities by using the **Delete Closed Opportunities** batch job, follow these steps:</span></span>

1. <span data-ttu-id="7bb2b-151">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Opportunity's verwijderen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-151">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Delete Opportunities**, and then choose the related link.</span></span>
2. <span data-ttu-id="7bb2b-152">Stel in het gedeelte **Opportunity** de filters in die opgeven welke gesloten opportunities moeten worden verwijderd.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-152">In the **Opportunity** section, set up the filters that specify the closed opportunities to delete.</span></span>
3. <span data-ttu-id="7bb2b-153">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-153">Choose the **OK** button.</span></span>

<span data-ttu-id="7bb2b-154">Nadat u een opportunity hebt verwijderd, wordt de opportunity verwijderd uit het venster **Opportunity-overzicht**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-154">After you have deleted an opportunity, it is removed it from the **Opportunity List** window.</span></span>

## <a name="to-move-an-opportunity-through-sales-cycle-stages"></a><span data-ttu-id="7bb2b-155">Een opportunity verplaatsen door verkoopcyclifasen</span><span class="sxs-lookup"><span data-stu-id="7bb2b-155">To move an opportunity through sales cycle stages</span></span>
<span data-ttu-id="7bb2b-156">Als een opportunity een verkoopcyclus volgt, kunt u deze voorwaarts of achterwaarts door de verschillende fasen verplaatsen, bijvoorbeeld naar de volgende of vorige fase, en zelfs een fase overslaan.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-156">If an opportunity follows a sales cycle, you can move it forward or back through the different stages, such as moving the next or previous stage, and even skipping a stage.</span></span>

1. <span data-ttu-id="7bb2b-157">Kies in het venster **Opportunity-overzicht** de actie **Bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-157">In the **Opportunity List** window, choose the **Update** action.</span></span> <span data-ttu-id="7bb2b-158">De wizard **Opportunity bijwerken** wordt geopend.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-158">The **Update Opportunity** opens,</span></span>
2. <span data-ttu-id="7bb2b-159">Gebruik het **Actiesoort** om de opportunity door de verkoopcyclusfasen te verplaatsen:</span><span class="sxs-lookup"><span data-stu-id="7bb2b-159">Use the **Action Type** field to move the opportunity through the sales cycle stages:</span></span>
   * <span data-ttu-id="7bb2b-160">**Volgende** verplaatst de opportunity één fase.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-160">**Next** moves the opportunity forward one stage.</span></span>
   * <span data-ttu-id="7bb2b-161">Met **Overslaan** wordt de opportunity een of meer fasen voorwaarts verplaatst in de verkoopcyclus, wat u opgeeft in het veld **Presentatie**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-161">**Skip** moves the opportunity forward one or several stages in the sales cycle, which you specify in the **Presentation** field.</span></span> <span data-ttu-id="7bb2b-162">U kunt alleen fasen overslaan die alleen zijn ingesteld om overslaan toe te staan.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-162">You can only skip stages that have been set up to allow skipping.</span></span>
   * <span data-ttu-id="7bb2b-163">**Vorige** verplaatst de opportunity één fase terug.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-163">**Previous** moves the opportunity back one stage.</span></span>
   * <span data-ttu-id="7bb2b-164">Met **Springen** wordt de opportunity een of meer fasen terug verplaatst in de verkoopcyclus, wat u opgeeft in het veld **Presentatie**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-164">**Jump** moves the opportunity back one or several stages in the sales cycle, which you specify in the **Presentation** field.</span></span>
   * <span data-ttu-id="7bb2b-165">Met **Bijwerken** kunt u informatie wijzigen (bijvoorbeeld om de evaluatie van de slagingskans en de geschatte waarden te wijzigen) zonder te verplaatsen naar een andere fase.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-165">**Update** enables you to change information (such as to modify your evaluation of their chances of success and estimated values) without moving to another stage.</span></span>
3. <span data-ttu-id="7bb2b-166">Vul de overige velden desgewenst in en kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="7bb2b-166">Fill in the other fields as needed, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="7bb2b-167">Zie ook</span><span class="sxs-lookup"><span data-stu-id="7bb2b-167">See Also</span></span>
[<span data-ttu-id="7bb2b-168">Verkoop</span><span class="sxs-lookup"><span data-stu-id="7bb2b-168">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="7bb2b-169">Contactpersonen maken en beheren</span><span class="sxs-lookup"><span data-stu-id="7bb2b-169">Creating and Managing Contacts</span></span>](marketing-contacts.md)  
<span data-ttu-id="7bb2b-170">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7bb2b-170">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
