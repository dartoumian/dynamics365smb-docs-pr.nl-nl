---
title: Werkstromen instellen | Microsoft Docs
description: U kunt werkstromen instellen en gebruiken om bedrijfsprocestaken te verbinden die door verschillende gebruikers worden uitgevoerd. Systeemtaken, zoals automatische boekingen, kunnen als stappen in werkstromen worden opgenomen, die worden voorafgegaan of gevolgd door gebruikerstaken. Het aanvragen en verlenen van goedkeuringen om nieuwe records te maken, zijn voorbeelden van veelvoorkomende werkstroomstappen.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 02/20/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: d2301b31308c1300961d78478ce1ada807eddeab
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="setting-up-workflows"></a><span data-ttu-id="b2fbb-105">Werkstromen instellen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-105">Setting Up Workflows</span></span>
<span data-ttu-id="b2fbb-106">U kunt werkstromen instellen en gebruiken om bedrijfsprocestaken te verbinden die door verschillende gebruikers worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="b2fbb-107">Systeemtaken, zoals automatische boekingen, kunnen als stappen in werkstromen worden opgenomen, die worden voorafgegaan of gevolgd door gebruikerstaken.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="b2fbb-108">Het aanvragen en verlenen van goedkeuringen om nieuwe records te maken, zijn voorbeelden van veelvoorkomende werkstroomstappen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-108">Requesting and granting approval to create new records are typical workflow steps.</span></span> <span data-ttu-id="b2fbb-109">Zie voor meer informatie [Werkstromen gebruiken](across-use-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="b2fbb-109">For more information, see [Using Workflows](across-use-workflows.md).</span></span>  

 <span data-ttu-id="b2fbb-110">Voordat u kunt beginnen met werkstromen gebruiken, moet u de werkstroomgebruikers en goedkeuringgebruikers instellen, opgeven hoe gebruikers berichten ontvangen over werkstroomstappen, mogelijk de code aanpassen en vervolgens de werkstromen maken.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-110">Before you begin to use workflows, you must set up workflow users and approval users, specify how users receive notifications about workflow steps, and then create the workflows, potentially preceded by code customization.</span></span>  

 <span data-ttu-id="b2fbb-111">In het venster **Werkstroom** kunt u een werkstroom maken door de betrokken stappen te vermelden op de regels.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-111">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="b2fbb-112">Elke stap bestaat uit een werkstroomgebeurtenis, aangepast door gebeurtenistoestanden, en een werkstroomantwoord, aangepast door antwoordopties.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-112">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="b2fbb-113">U definieert werkstroomregels door velden op werkstroomregels te vullen vanuit lijsten met vaste gebeurtenis- en reactiewaarden die scenario's vertegenwoordigen die worden ondersteund door de toepassingscode.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-113">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="b2fbb-114">Als een bedrijfsscenario een werkstroomgebeurtenis of -reactie vereist die niet wordt ondersteund, moet een Microsoft-partner ze implementeren door de toepassingscode aan te passen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-114">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="b2fbb-115">Raadpleeg [Procedure: Nieuwe werkstroomgebeurtenissen en -reacties implementeren](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in de Help voor ontwikkelaars en IT-professionals voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-115">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses) in the developer and IT-pro help.</span></span>

 <span data-ttu-id="b2fbb-116">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-116">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="b2fbb-117">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="b2fbb-117">**To**</span></span>|<span data-ttu-id="b2fbb-118">**Onderwerp**</span><span class="sxs-lookup"><span data-stu-id="b2fbb-118">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="b2fbb-119">Werkstroomgebruikers en gebruikersgroepen instellen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-119">Set up workflow users and user groups.</span></span>|[<span data-ttu-id="b2fbb-120">Werkstroomgebruikers instellen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-120">Set Up Workflow Users</span></span>](across-how-to-set-up-workflow-users.md)|  
|<span data-ttu-id="b2fbb-121">Werkstroomgebruikers die deelnemen aan werkstromen voor goedkeuring, instellen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-121">Set up workflow users who take part in approval workflows.</span></span>|[<span data-ttu-id="b2fbb-122">Goedkeuringsgebruikers instellen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-122">Set Up Approval Users</span></span>](across-how-to-set-up-approval-users.md)|  
|<span data-ttu-id="b2fbb-123">Aangeven hoe werkstroomgebruikers op hoogte worden gebracht van werkstroomstappen, inclusief goedkeuringsaanvragen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-123">Specify how workflow users are notified of workflow steps, including approval requests.</span></span>|[<span data-ttu-id="b2fbb-124">Werkstroomberichten instellen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-124">Setting Up Workflow Notifications</span></span>](across-setting-up-workflow-notifications.md)|  
|<span data-ttu-id="b2fbb-125">Geef op wanneer gebruikers berichten ontvangen en of berichten in een periode moeten worden geaggregeerd om het aantal berichten zo klein mogelijk te maken.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-125">Specify when users receive notifications and whether to aggregate notifications in a period to minimize the number of notifications.</span></span>|[<span data-ttu-id="b2fbb-126">Opgeven wanneer en hoe gebruikers berichten ontvangen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-126">Specify When and How to Receive Notifications</span></span>](across-how-to-specify-when-and-how-to-receive-notifications.md)|  
|<span data-ttu-id="b2fbb-127">De lay-out en algemene inhoud van nieuwe e-mails voor werkstroomberichten instellen, of bestaande sjablonen exporteren, wijzigen en weer importeren.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-127">Set up the layout and general content of new workflow notifications emails, or export, modify, and reimport existing templates.</span></span>|[<span data-ttu-id="b2fbb-128">Berichtsjablonen beheren</span><span class="sxs-lookup"><span data-stu-id="b2fbb-128">Manage Notification Templates</span></span>](across-how-to-manage-notification-templates.md)|  
|<span data-ttu-id="b2fbb-129">Stel een SMTP-server in om communicatie per e-mail in en vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)] in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-129">Set up an SMTP server to enable email communication in and out of [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>|[<span data-ttu-id="b2fbb-130">E-mail instellen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-130">Set up Email</span></span>](admin-how-setup-email.md)|
|<span data-ttu-id="b2fbb-131">De verschillende stappen van een werkstroom opgeven door werkstroomgebeurtenissen te koppelen aan werkstroomantwoorden.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-131">Specify the different steps of a workflow by connection workflow events with workflow responses.</span></span>|[<span data-ttu-id="b2fbb-132">Werkstromen maken</span><span class="sxs-lookup"><span data-stu-id="b2fbb-132">Create Workflows</span></span>](across-how-to-create-workflows.md)|  
|<span data-ttu-id="b2fbb-133">Gebruik werkstroomsjablonen om nieuwe werkstromen te maken.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-133">Use workflow templates to create new workflows.</span></span>|[<span data-ttu-id="b2fbb-134">Werkstromen maken van werkstroomsjablonen</span><span class="sxs-lookup"><span data-stu-id="b2fbb-134">Create Workflows from Workflow Templates</span></span>](across-how-to-create-workflows-from-workflow-templates.md)|  
|<span data-ttu-id="b2fbb-135">Werkstromen delen met andere [!INCLUDE[d365fin](includes/d365fin_md.md)]-databases.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-135">Share workflows with other [!INCLUDE[d365fin](includes/d365fin_md.md)] databases.</span></span>|[<span data-ttu-id="b2fbb-136">Werkstromen exporteren en importeren</span><span class="sxs-lookup"><span data-stu-id="b2fbb-136">Export and Import Workflows</span></span>](across-how-to-export-and-import-workflows.md)|  
|<span data-ttu-id="b2fbb-137">Lees meer informatie over het instellen van een werkstroom voor de goedkeuring van verkoopdocumenten door een end-to-end procedure te volgen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-137">Learn how to set up a workflow for approving sales documents by following an end-to-end procedure.</span></span>|[<span data-ttu-id="b2fbb-138">Procedure: Een werkstroom voor inkoopgoedkeuring instellen en gebruiken</span><span class="sxs-lookup"><span data-stu-id="b2fbb-138">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span></span>](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)|  
|<span data-ttu-id="b2fbb-139">Voeg ondersteuning toe voor een bedrijfsscenario dat nieuwe werkstroomgebeurtenissen of -antwoorden vereist, door de toepassingscode aan te passen.</span><span class="sxs-lookup"><span data-stu-id="b2fbb-139">Add support for a business scenario that requires new workflow events or responses by customizing the application code.</span></span>|[<span data-ttu-id="b2fbb-140">Procedure: Nieuwe werkstroomgebeurtenissen en -reacties implementeren</span><span class="sxs-lookup"><span data-stu-id="b2fbb-140">Walkthrough: Implementing New Workflow Events and Responses</span></span>](/dynamics-nav/Walkthrough--Implementing-New-Workflow-Events-and-Responses)|  

## <a name="see-also"></a><span data-ttu-id="b2fbb-141">Zie ook</span><span class="sxs-lookup"><span data-stu-id="b2fbb-141">See Also</span></span>  
 <span data-ttu-id="b2fbb-142">[Werkstromen gebruiken](across-use-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="b2fbb-142">[Using Workflows](across-use-workflows.md) </span></span>  
 <span data-ttu-id="b2fbb-143">[Werkstroom](across-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="b2fbb-143">[Workflow](across-workflow.md) </span></span>  
 [<span data-ttu-id="b2fbb-144">Procedure: Een werkstroom voor inkoopgoedkeuring instellen en gebruiken</span><span class="sxs-lookup"><span data-stu-id="b2fbb-144">Walkthrough: Setting Up and Using a Purchase Approval Workflow</span></span>](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)  
 [<span data-ttu-id="b2fbb-145">Werken met Financials</span><span class="sxs-lookup"><span data-stu-id="b2fbb-145">Working with Financials</span></span>](ui-work-product.md)
