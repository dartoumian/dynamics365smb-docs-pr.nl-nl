---
title: "Een OHW-methode definiëren en projectvoortgang controleren| Microsoft Docs"
description: "Beschrijft hoe u een OHW-methode (onderhanden werk) kunt maken en OHW kunt berekenen om de financiële waarde van projecten in te schatten terwijl ze bezig zijn."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, KPI, work in process, work in progress
ms.date: 07/04/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 95a14b122c5e6b878ec8d7f8314c81de957853b7
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="monitor-job-progress-and-performance"></a><span data-ttu-id="e985d-103">Voortgang en prestaties van projecten bewaken</span><span class="sxs-lookup"><span data-stu-id="e985d-103">Monitor Job Progress and Performance</span></span>
<span data-ttu-id="e985d-104">Naarmate een project vordert, worden materialen, resources en overige zaken verbruikt en moeten hiervoor boekingen plaatsvinden op het project.</span><span class="sxs-lookup"><span data-stu-id="e985d-104">As a job progresses, materials, resources, and other expenses are consumed and must be posted to the job.</span></span> <span data-ttu-id="e985d-105">Onderhanden werk (OHW) is een functie waarmee u de financiële waarde van projecten in het grootboek kunt schatten gedurende de projecten.</span><span class="sxs-lookup"><span data-stu-id="e985d-105">Work in Process (WIP) is a feature that enables you to estimate the financial value of jobs in the general ledger while the jobs are ongoing.</span></span> <span data-ttu-id="e985d-106">In veel gevallen kunt u kosten voor een project boeken voordat u het project factureert.</span><span class="sxs-lookup"><span data-stu-id="e985d-106">In many cases, you might post expenses for a job before invoicing a job.</span></span> <span data-ttu-id="e985d-107">Wanneer alleen kosten zijn geboekt, klopt het financiële afschrift niet.</span><span class="sxs-lookup"><span data-stu-id="e985d-107">When only expenses have been posted, your financial statement will be inaccurate.</span></span> <span data-ttu-id="e985d-108">Zie [OHW-methoden](projects-understanding-wip.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e985d-108">For more information, see [Understanding WIP Methods](projects-understanding-wip.md).</span></span>

<span data-ttu-id="e985d-109">Als u de waarde in het grootboek wilt volgen, kunt u het OHW-bedrag berekenen en de waarde boeken in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="e985d-109">To track the value in the general ledger, you can calculate WIP and post the value to the general ledger.</span></span>

<span data-ttu-id="e985d-110">U kunt het OHW-bedrag berekenen op basis van de volgende zaken:</span><span class="sxs-lookup"><span data-stu-id="e985d-110">You can calculate WIP based on the following:</span></span>

* <span data-ttu-id="e985d-111">Kostprijs</span><span class="sxs-lookup"><span data-stu-id="e985d-111">Cost Value</span></span>
* <span data-ttu-id="e985d-112">Verkoopprijs</span><span class="sxs-lookup"><span data-stu-id="e985d-112">Sales Value</span></span>
* <span data-ttu-id="e985d-113">Kostprijs van omzet</span><span class="sxs-lookup"><span data-stu-id="e985d-113">Recognizable Cost</span></span>
* <span data-ttu-id="e985d-114">Percentage voltooid</span><span class="sxs-lookup"><span data-stu-id="e985d-114">Percentage of Completion</span></span>
* <span data-ttu-id="e985d-115">Contract voltooid</span><span class="sxs-lookup"><span data-stu-id="e985d-115">Completed Contract</span></span>

<span data-ttu-id="e985d-116">Als u het resultaat met een andere methode wilt bekijken, kunt u de methode wijzigen en het OHW-bedrag nogmaals berekenen.</span><span class="sxs-lookup"><span data-stu-id="e985d-116">If you want to view the result using a different method, you can change the method and calculate WIP again.</span></span> <span data-ttu-id="e985d-117">U kunt net zo vaak het OHW-bedrag berekenen als u wilt.</span><span class="sxs-lookup"><span data-stu-id="e985d-117">There is no limit to the number of times that you calculate WIP.</span></span> <span data-ttu-id="e985d-118">Het OHW-bedrag wordt alleen berekend en wordt niet geboekt in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="e985d-118">WIP is only calculated, it does not get posted to the general ledger.</span></span> <span data-ttu-id="e985d-119">Na het berekenen van het OHW-bedrag, kunt u het OHW-bedrag boeken in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="e985d-119">After you have calculated WIP, you can post to the general ledger.</span></span>

## <a name="to-create-a-job-wip-method"></a><span data-ttu-id="e985d-120">Een OHW-methode voor een project maken</span><span class="sxs-lookup"><span data-stu-id="e985d-120">To create a job WIP method</span></span>
<span data-ttu-id="e985d-121">U kunt een OHW-methode voor een project maken die de behoeften van uw organisatie weerspiegelt.</span><span class="sxs-lookup"><span data-stu-id="e985d-121">You can create a job WIP method that reflects the needs of your organization.</span></span> <span data-ttu-id="e985d-122">Nadat u deze methode hebt gemaakt, kunt u deze instellen als standaard OHW-berekeningsmethode voor een project die wordt gebruikt in uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="e985d-122">After you have created it, you can set it as the default job WIP calculation method that will be used in your organization.</span></span>  

> [!NOTE]
> <span data-ttu-id="e985d-123">Nadat u uw nieuwe methode hebt gebruikt om OHW-posten te maken, kunt u de methode niet meer verwijderen of wijzigen.</span><span class="sxs-lookup"><span data-stu-id="e985d-123">After you have used your new method to create WIP entries, you cannot delete the method or modify it.</span></span>  

1. <span data-ttu-id="e985d-124">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **OHW-methoden taak** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e985d-124">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job WIP Methods**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e985d-125">Kies de actie **Nieuw** en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="e985d-125">Choose the **New** action, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. <span data-ttu-id="e985d-126">Sluit het venster.</span><span class="sxs-lookup"><span data-stu-id="e985d-126">Close the window.</span></span>   
4. <span data-ttu-id="e985d-127">Als u van deze nieuwe methode de standaard wilt maken, kiest u het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voert u **Projectinstellingen** in en kiest u vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e985d-127">To make this new method the default, choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs Setup**, and then choose the related link.</span></span>  
5. <span data-ttu-id="e985d-128">Kies in het veld **Standaard OHW-methode** de methode uit de lijst.</span><span class="sxs-lookup"><span data-stu-id="e985d-128">In the **Default WIP Method** field, choose the method from the list.</span></span>

## <a name="to-define-a-wip-method-for-a-job"></a><span data-ttu-id="e985d-129">Een OHW-methode voor een project definiëren</span><span class="sxs-lookup"><span data-stu-id="e985d-129">To define a WIP method for a job</span></span>
<span data-ttu-id="e985d-130">Wanneer u een nieuw project maakt, moet u opgeven welke OHW-methode voor het project van toepassing is.</span><span class="sxs-lookup"><span data-stu-id="e985d-130">When you create a new job, you must specify which job WIP method that applies.</span></span> <span data-ttu-id="e985d-131">In sommige gevallen is de OHW-methode voor het project die u kunt gebruiken standaard voor u ingesteld.</span><span class="sxs-lookup"><span data-stu-id="e985d-131">In some cases, which Job WIP method that you can use has been set up for you as a default.</span></span>

1. <span data-ttu-id="e985d-132">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Projecten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e985d-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="e985d-133">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="e985d-133">Choose the **New** action.</span></span> <span data-ttu-id="e985d-134">Zie voor meer informatie [Projecten maken](projects-how-create-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="e985d-134">For more information, see [Create Jobs](projects-how-create-jobs.md).</span></span>  
3. <span data-ttu-id="e985d-135">Selecteer in het venster **Projectkaart** in het veld **OHW-methode** een OHW-methode uit de lijst.</span><span class="sxs-lookup"><span data-stu-id="e985d-135">In the **Job Card** window, in the **WIP Method** field, select a WIP method from the list.</span></span> <span data-ttu-id="e985d-136">Als een standaardmethode is gedefinieerd, kunt u indien nodig een andere optie selecteren.</span><span class="sxs-lookup"><span data-stu-id="e985d-136">If a default method has been defined, you can select another option if needed.</span></span>  

## <a name="to-calculate-wip"></a><span data-ttu-id="e985d-137">OHW berekenen</span><span class="sxs-lookup"><span data-stu-id="e985d-137">To calculate WIP</span></span>
<span data-ttu-id="e985d-138">U kunt het OHW-bedrag bepalen dat moet worden geboekt naar balansrekeningen voor eindrapportage van een periode.</span><span class="sxs-lookup"><span data-stu-id="e985d-138">You can determine the WIP amount that is to be posted to balance sheet accounts for the period end reporting.</span></span> <span data-ttu-id="e985d-139">U gebruikt hiervoor de batchverwerking **OHW voor project berekenen**.</span><span class="sxs-lookup"><span data-stu-id="e985d-139">You use the **Job Calculate WIP** batch job to do this.</span></span>  

1. <span data-ttu-id="e985d-140">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **OHW voor project berekenen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e985d-140">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Calculate WIP**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e985d-141">Kies de actie **OHW berekenen**.</span><span class="sxs-lookup"><span data-stu-id="e985d-141">Choose the **Calculate WIP** action.</span></span>
3. <span data-ttu-id="e985d-142">Vul in het venster **OHW voor project berekenen** indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="e985d-142">In the **Job Calculate WIP** window, fill in the fields as necessary.</span></span>
4. <span data-ttu-id="e985d-143">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="e985d-143">Choose the **OK** button.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="e985d-144">De batchverwerking berekent alleen het OHW.</span><span class="sxs-lookup"><span data-stu-id="e985d-144">The batch job only calculates the WIP.</span></span> <span data-ttu-id="e985d-145">Het wordt niet geboekt in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="e985d-145">It is not posted to the general ledger.</span></span> <span data-ttu-id="e985d-146">Hiervoor moet u de batchverwerking **OHW naar GB boeken** uitvoeren wanneer u het onderhanden werk hebt berekend.</span><span class="sxs-lookup"><span data-stu-id="e985d-146">To do so, you must run the **Post WIP to G/L** batch job when you have calculated the WIP.</span></span> <span data-ttu-id="e985d-147">Zie de volgende procedure voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e985d-147">For more information, see the following procedure.</span></span>

## <a name="to-post-wip"></a><span data-ttu-id="e985d-148">OHW boeken</span><span class="sxs-lookup"><span data-stu-id="e985d-148">To post WIP</span></span>
<span data-ttu-id="e985d-149">Wanneer u OHW hebt berekend, kunt u het boeken naar balansrekeningen voor de einddatumrapportage.</span><span class="sxs-lookup"><span data-stu-id="e985d-149">When you have calculated WIP, you can post it to balance sheet accounts for the period end reporting.</span></span> <span data-ttu-id="e985d-150">Hiervoor gebruikt u de batchverwerking **Project-OHW naar GB boeken**.</span><span class="sxs-lookup"><span data-stu-id="e985d-150">You use the **Job Post WIP to G/L** batch job to do this.</span></span>

1. <span data-ttu-id="e985d-151">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Project-OHW naar GB boeken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e985d-151">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Post WIP to G/L**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e985d-152">Vul in het venster **Project-OHW naar GB boeken** indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="e985d-152">In the **Job Post WIP to G/L** window, fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="e985d-153">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="e985d-153">Choose the **OK** button.</span></span>

## <a name="to-view-job-usage-estimates-and-post-updates"></a><span data-ttu-id="e985d-154">Projectgebruikschattingen weergeven en updates boeken</span><span class="sxs-lookup"><span data-stu-id="e985d-154">To view job usage estimates and post updates</span></span>
<span data-ttu-id="e985d-155">U kunt in één stap het projectgebruik tot aan de voltooiing van een project bekijken.</span><span class="sxs-lookup"><span data-stu-id="e985d-155">You can view job usage up to the completion of a project in one step.</span></span> <span data-ttu-id="e985d-156">Hiervoor gebruikt u de batchverwerking **Project - Resterend gebruik berekenen** voor alle taken tot en met het einde van een project.</span><span class="sxs-lookup"><span data-stu-id="e985d-156">To do so, you use the **Job Calc. Remaining Usage** batch job for all the tasks up to and including the end of a job.</span></span>  

<span data-ttu-id="e985d-157">Op deze manier kunt u uw oorspronkelijke schattingen volgen en vergelijken met de werkelijke resultaten en zo nodig wijzigingen aanbrengen of nieuwe posten maken.</span><span class="sxs-lookup"><span data-stu-id="e985d-157">This lets you track and compare your original estimates against actual results and make modifications or new entries as needed.</span></span> <span data-ttu-id="e985d-158">U hebt bijvoorbeeld mogelijk geschat dat een project 10 uur vereist en tot op heden zijn er al 15 uur aan besteed.</span><span class="sxs-lookup"><span data-stu-id="e985d-158">For example, you may have estimated that a job required 10 hours, and to date, it has taken 15 hours.</span></span> <span data-ttu-id="e985d-159">U kunt de extra vijf uur aan de bestaande dagboekregel toevoegen of een nieuwe dagboekregel maken om deze vijf uur als overuren te rapporteren. Dit is een ander werksoort.</span><span class="sxs-lookup"><span data-stu-id="e985d-159">You can add the extra five hours to the existing journal line or create a new journal line to report these five hours as overtime, which is another work type.</span></span> <span data-ttu-id="e985d-160">De juiste kosten en prijzen worden berekend die vervolgens naar het dagboek kunnen worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="e985d-160">The appropriate cost and price are calculated, and you can then post to the journal.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="e985d-161">Artikelposten maken artikeljournaalposten en verkleinen de voorraadhoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="e985d-161">Item entries create item ledger entries and reduce the inventory quantity.</span></span> <span data-ttu-id="e985d-162">De batchverwerking **Voorraadwaarde boeken** brengt de kosten van de voorraad over naar het grootboek.</span><span class="sxs-lookup"><span data-stu-id="e985d-162">The **Post Inventory Cost to G/L** batch job transfers the cost from inventory to the general ledger.</span></span> <span data-ttu-id="e985d-163">Resourceposten maken resourceposten.</span><span class="sxs-lookup"><span data-stu-id="e985d-163">Resource entries create resource ledger entries.</span></span>  

1. <span data-ttu-id="e985d-164">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Projectdagboeken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e985d-164">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e985d-165">Selecteer een relevant projectdagboek en kies vervolgens de actie **Resterend gebruik berekenen**.</span><span class="sxs-lookup"><span data-stu-id="e985d-165">Select a relevant job journal, and then choose the **Calc. Remaining Usage** action.</span></span>  
3. <span data-ttu-id="e985d-166">Voer in het venster **Project - Resterend gebruik berekenen** het documentnummer en de boekingsdatum in die in het dagboek moeten worden ingevoegd, en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="e985d-166">In the **Job Calc. Remaining Usage** window, enter the document number and posting date that is to be inserted in the journal, and then choose the **OK** button.</span></span>  
4. <span data-ttu-id="e985d-167">Werk het dagboek bij met eventuele wijzigingen die nodig zijn.</span><span class="sxs-lookup"><span data-stu-id="e985d-167">Update the journal with any modifications that may be needed.</span></span>  
5. <span data-ttu-id="e985d-168">Kies de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="e985d-168">Choose the **Post**.</span></span>

## <a name="to-view-job-ledger-entries"></a><span data-ttu-id="e985d-169">Projectposten bekijken</span><span class="sxs-lookup"><span data-stu-id="e985d-169">To view job ledger entries</span></span>
<span data-ttu-id="e985d-170">Alle posten met betrekking tot een project worden in projectjournalen opgeslagen en sequentieel genummerd, te beginnen met 1.</span><span class="sxs-lookup"><span data-stu-id="e985d-170">All job-related entries are recorded in job registers and are numbered sequentially, starting with 1.</span></span> <span data-ttu-id="e985d-171">Vanuit het projectjournaal hebt u een overzicht van alle projectposten.</span><span class="sxs-lookup"><span data-stu-id="e985d-171">From the job register, you can get an overview of all job ledger entries.</span></span>    

1. <span data-ttu-id="e985d-172">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Projectjournalen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e985d-172">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Registers**, and then choose the related link.</span></span>
2. <span data-ttu-id="e985d-173">Selecteer een relevant journaal en kies vervolgens de actie **Projectposten**.</span><span class="sxs-lookup"><span data-stu-id="e985d-173">Select a relevant register, and then choose **Job Ledger** action.</span></span>

<span data-ttu-id="e985d-174">Het venster **Projectposten** wordt geopend, waarin u de posten die zijn gekoppeld aan een project, kunt bekijken.</span><span class="sxs-lookup"><span data-stu-id="e985d-174">In the **Job Ledger Entries** window you can review the entries that are associated with any job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e985d-175">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e985d-175">See Also</span></span>
<span data-ttu-id="e985d-176">[Projecten beheren](projects-manage-projects.md)
[Voorraadkosten beheren](finance-manage-inventory-costs.md) </span><span class="sxs-lookup"><span data-stu-id="e985d-176">[Managing Projects](projects-manage-projects.md)
[Managing Inventory Costs](finance-manage-inventory-costs.md) </span></span>  
[<span data-ttu-id="e985d-177">Financiën</span><span class="sxs-lookup"><span data-stu-id="e985d-177">Finance</span></span>](finance.md)  
<span data-ttu-id="e985d-178">[Inkoop](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="e985d-178">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="e985d-179">[Verkoop](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="e985d-179">[Sales](sales-manage-sales.md)    </span></span>  
<span data-ttu-id="e985d-180">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e985d-180">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
