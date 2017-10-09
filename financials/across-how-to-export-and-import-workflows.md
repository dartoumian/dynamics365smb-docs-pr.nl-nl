---
title: Werkstromen exporteren en importeren | Microsoft Docs
description: Als u werkstromen wilt overbrengen naar andere [!INCLUDE[d365fin](includes/d365fin_md.md)]-databases, bijvoorbeeld om tijd te besparen wanneer u nieuwe werkstromen maakt, kunt u werkstromen exporteren en importeren.
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
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 8126d3850103819e885d9d131ca3074f1b7cfda1
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-export-and-import-workflows"></a><span data-ttu-id="72424-103">Procedure: Werkstromen exporteren en importeren</span><span class="sxs-lookup"><span data-stu-id="72424-103">How to: Export and Import Workflows</span></span>
<span data-ttu-id="72424-104">Als u werkstromen wilt overbrengen naar andere [!INCLUDE[d365fin](includes/d365fin_md.md)]-databases, bijvoorbeeld om tijd te besparen wanneer u nieuwe werkstromen maakt, kunt u werkstromen exporteren en importeren.</span><span class="sxs-lookup"><span data-stu-id="72424-104">To transfer workflows to other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases, for example to save time when creating new workflows, you can export and import workflows.</span></span>  

 <span data-ttu-id="72424-105">Een andere manier om werkstromen snel te maken is werkstromen te maken van werkstroomsjablonen.</span><span class="sxs-lookup"><span data-stu-id="72424-105">Another way to quickly create workflows is to create workflows from workflow templates.</span></span> <span data-ttu-id="72424-106">Zie voor meer informatie [Procedure: Werkstromen maken van werkstroomsjablonen](across-how-to-create-workflows-from-workflow-templates.md).</span><span class="sxs-lookup"><span data-stu-id="72424-106">For more information, see [How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md).</span></span>  

 <span data-ttu-id="72424-107">In het venster **Werkstroom** kunt u een werkstroom maken door de betrokken stappen te vermelden op de regels.</span><span class="sxs-lookup"><span data-stu-id="72424-107">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="72424-108">Elke stap bestaat uit een werkstroomgebeurtenis, aangepast door gebeurtenistoestanden, en een werkstroomantwoord, aangepast door antwoordopties.</span><span class="sxs-lookup"><span data-stu-id="72424-108">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="72424-109">U definieert werkstroomregels door velden op werkstroomregels te vullen vanuit lijsten met vaste gebeurtenis- en reactiewaarden die scenario's vertegenwoordigen die worden ondersteund door de toepassingscode.</span><span class="sxs-lookup"><span data-stu-id="72424-109">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span> <span data-ttu-id="72424-110">Zie voor meer informatie [Procedure: Werkstromen maken](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="72424-110">For more information, see [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="to-export-a-workflow"></a><span data-ttu-id="72424-111">Een werkstroom exporteren</span><span class="sxs-lookup"><span data-stu-id="72424-111">To export a workflow</span></span>  
1.  <span data-ttu-id="72424-112">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Werkstromen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="72424-112">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="72424-113">Selecteer een werkstroom en kies de actie **Exporteren naar bestand**.</span><span class="sxs-lookup"><span data-stu-id="72424-113">Select a workflow, and then choose the **Export to File** action.</span></span>  
3.  <span data-ttu-id="72424-114">Kies in het venster **Bestand exporteren** de knop **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="72424-114">In the **Export File** window, choose the **Save** button.</span></span>  
4.  <span data-ttu-id="72424-115">Selecteer in het venster **Exporteren** een bestandslocatie en kies vervolgens de knop **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="72424-115">In the **Export** window, select a file location, and then choose the **Save** button.</span></span>  

## <a name="to-import-a-workflow"></a><span data-ttu-id="72424-116">Een werkstroom importeren</span><span class="sxs-lookup"><span data-stu-id="72424-116">To import a workflow</span></span>  
1.  <span data-ttu-id="72424-117">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Werkstromen** in en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="72424-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Workflows**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="72424-118">Kies de actie **Importeren uit bestand**.</span><span class="sxs-lookup"><span data-stu-id="72424-118">Choose the **Import from File** action.</span></span>  
3.  <span data-ttu-id="72424-119">Selecteer in het venster **Importeren** het XML-bestand dat de werkstroom bevat, en klik vervolgens op **Openen**.</span><span class="sxs-lookup"><span data-stu-id="72424-119">In the **Import** window, choose the XML file that contains the workflow, and then choose the **Open** button.</span></span>  

> [!CAUTION]  
>  <span data-ttu-id="72424-120">Als de werkstroomcode al in de database bestaat, worden de werkstroomstappen overschreven door de stappen in de geïmporteerde werkstroom.</span><span class="sxs-lookup"><span data-stu-id="72424-120">If the workflow code already exists in the database, the workflow steps will be overwritten with the steps in the imported workflow.</span></span>  

## <a name="see-also"></a><span data-ttu-id="72424-121">Zie ook</span><span class="sxs-lookup"><span data-stu-id="72424-121">See Also</span></span>  
 <span data-ttu-id="72424-122">[Procedure: Werkstromen maken](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="72424-122">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="72424-123">[Procedure: Werkstromen maken van werkstroomsjablonen](across-how-to-create-workflows-from-workflow-templates.md) </span><span class="sxs-lookup"><span data-stu-id="72424-123">[How to: Create Workflows from Workflow Templates](across-how-to-create-workflows-from-workflow-templates.md) </span></span>  
 <span data-ttu-id="72424-124">[Procedure: Gearchiveerde instanties van werkstroomstappen bekijken](across-how-to-view-archived-workflow-step-instances.md) </span><span class="sxs-lookup"><span data-stu-id="72424-124">[How to: View Archived Workflow Step Instances](across-how-to-view-archived-workflow-step-instances.md) </span></span>  
 <span data-ttu-id="72424-125">[Procedure: Werkstromen verwijderen](across-how-to-delete-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="72424-125">[How to: Delete Workflows](across-how-to-delete-workflows.md) </span></span>  
 <span data-ttu-id="72424-126">[Procedure: Een werkstroom voor inkoopgoedkeuring instellen en gebruiken](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="72424-126">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 <span data-ttu-id="72424-127">[Werkstromen instellen](across-set-up-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="72424-127">[Setting Up Workflows](across-set-up-workflows.md) </span></span>  
 <span data-ttu-id="72424-128">[Werkstromen gebruiken](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="72424-128">[Using Workflows](across-use-workflows.md) </span></span>  
 [<span data-ttu-id="72424-129">Werkstroom</span><span class="sxs-lookup"><span data-stu-id="72424-129">Workflow</span></span>](across-workflow.md)   
