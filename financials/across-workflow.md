---
title: Werkstroom | Microsoft Docs
description: U kunt werkstromen instellen en gebruiken om bedrijfsprocestaken te verbinden die door verschillende gebruikers worden uitgevoerd. Systeemtaken, zoals automatische boekingen, kunnen als stappen in werkstromen worden opgenomen, die worden voorafgegaan of gevolgd door gebruikerstaken. Het aanvragen en verlenen van goedkeuringen om nieuwe records te maken, zijn voorbeelden van veelvoorkomende werkstroomstappen.
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
ms.openlocfilehash: f65c0e577e839928809f7afda3dbdb4c9b7702c8
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="workflow"></a><span data-ttu-id="da94f-105">Werkstroom</span><span class="sxs-lookup"><span data-stu-id="da94f-105">Workflow</span></span>
<span data-ttu-id="da94f-106">U kunt werkstromen instellen en gebruiken om bedrijfsprocestaken te verbinden die door verschillende gebruikers worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="da94f-106">You can set up and use workflows that connect business-process tasks performed by different users.</span></span> <span data-ttu-id="da94f-107">Systeemtaken, zoals automatische boekingen, kunnen als stappen in werkstromen worden opgenomen, die worden voorafgegaan of gevolgd door gebruikerstaken.</span><span class="sxs-lookup"><span data-stu-id="da94f-107">System tasks, such as automatic posting, can be included as steps in workflows, preceded or followed by user tasks.</span></span> <span data-ttu-id="da94f-108">Het aanvragen en verlenen van goedkeuringen om nieuwe records te maken, zijn voorbeelden van veelvoorkomende werkstroomstappen.</span><span class="sxs-lookup"><span data-stu-id="da94f-108">Requesting and granting approval to create new records are typical workflow steps.</span></span>  

 <span data-ttu-id="da94f-109">In het venster **Werkstroom** kunt u een werkstroom maken door de betrokken stappen te vermelden op de regels.</span><span class="sxs-lookup"><span data-stu-id="da94f-109">In the **Workflow** window, you create a workflow by listing the involved steps on the lines.</span></span> <span data-ttu-id="da94f-110">Elke stap bestaat uit een werkstroomgebeurtenis, aangepast door gebeurtenistoestanden, en een werkstroomantwoord, aangepast door antwoordopties.</span><span class="sxs-lookup"><span data-stu-id="da94f-110">Each step consists of a workflow event, moderated by event conditions, and a workflow response, moderated by response options.</span></span> <span data-ttu-id="da94f-111">U definieert werkstroomregels door velden op werkstroomregels te vullen vanuit lijsten met vaste gebeurtenis- en reactiewaarden die scenario's vertegenwoordigen die worden ondersteund door de toepassingscode.</span><span class="sxs-lookup"><span data-stu-id="da94f-111">You define workflow steps by filling fields on workflow lines from fixed lists of event and response values representing scenarios that are supported by the application code.</span></span>  

 <span data-ttu-id="da94f-112">De algemene versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] bevat een aantal vooraf geconfigureerde werkstromen die worden vertegenwoordigd door werkstroomsjablonen die u kunt kopiëren om werkstromen te maken.</span><span class="sxs-lookup"><span data-stu-id="da94f-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] includes a number of preconfigured workflows represented by workflow templates that you can copy to create workflows.</span></span> <span data-ttu-id="da94f-113">De code voor werkstroomsjablonen die door Microsoft worden toegevoegd, heeft het voorvoegsel "MS-".</span><span class="sxs-lookup"><span data-stu-id="da94f-113">The code for workflow templates that are added by Microsoft are prefixed with “MS-“.</span></span> <span data-ttu-id="da94f-114">Zie voor meer informatie de lijst met werkstroomsjablonen in het venster Werkstroomsjablonen venster.</span><span class="sxs-lookup"><span data-stu-id="da94f-114">For more information, see the list of workflow templates in the Workflow Templates window.</span></span>  

 <span data-ttu-id="da94f-115">Als een bedrijfsscenario een werkstroomgebeurtenis of -reactie vereist die niet wordt ondersteund, moet een Microsoft-partner ze implementeren door de toepassingscode aan te passen.</span><span class="sxs-lookup"><span data-stu-id="da94f-115">If a business scenario requires a workflow event or response that is not supported, a Microsoft partner must implement them by customizing the application code.</span></span> <span data-ttu-id="da94f-116">Zie voor meer informatie [Procedure: Nieuwe werkstroomgebeurtenissen en -responsen implementeren](https://msdn.microsoft.com/en-us/library/mt574349.aspx) op MSDN.</span><span class="sxs-lookup"><span data-stu-id="da94f-116">For more information, see [Walkthrough: Implementing New Workflow Events and Responses](https://msdn.microsoft.com/en-us/library/mt574349.aspx) on MSDN.</span></span>  

 <span data-ttu-id="da94f-117">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="da94f-117">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>  

|<span data-ttu-id="da94f-118">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="da94f-118">**To**</span></span>|<span data-ttu-id="da94f-119">**Onderwerp**</span><span class="sxs-lookup"><span data-stu-id="da94f-119">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="da94f-120">Gebruikers van werkstromen instellen, opgeven hoe gebruikers berichten krijgen en nieuwe werkstromen maken.</span><span class="sxs-lookup"><span data-stu-id="da94f-120">Set up workflow users, specify how users get notified, and create new workflows.</span></span> <span data-ttu-id="da94f-121">Voor nieuwe werkstromen voor niet-ondersteunde scenario's implementeert u de vereiste workflowelementen door de toepassingcode aan te passen.</span><span class="sxs-lookup"><span data-stu-id="da94f-121">For new workflows for unsupported scenarios, implement the required workflow elements by customizing the application code.</span></span>|[<span data-ttu-id="da94f-122">Werkstromen instellen</span><span class="sxs-lookup"><span data-stu-id="da94f-122">Setting Up Workflows</span></span>](across-set-up-workflows.md)|  
|<span data-ttu-id="da94f-123">Werkstromen inschakelen, reageren op werkstroomberichten, inclusief goedkeuringen aanvragen en aanvragen goedkeuren om een werkstroomstap uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="da94f-123">Enable workflows, act on workflow notifications, including request approvals and approve requests to perform a workflow step.</span></span> <span data-ttu-id="da94f-124">Werkstromen archiveren en verwijderen.</span><span class="sxs-lookup"><span data-stu-id="da94f-124">Archive and delete workflows.</span></span>|[<span data-ttu-id="da94f-125">Werkstromen gebruiken</span><span class="sxs-lookup"><span data-stu-id="da94f-125">Using Workflows</span></span>](across-use-workflows.md)|  

## <a name="see-also"></a><span data-ttu-id="da94f-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="da94f-126">See Also</span></span>  
[<span data-ttu-id="da94f-127">Verkoop</span><span class="sxs-lookup"><span data-stu-id="da94f-127">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="da94f-128">Inkoop</span><span class="sxs-lookup"><span data-stu-id="da94f-128">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="da94f-129">Projecten beheren</span><span class="sxs-lookup"><span data-stu-id="da94f-129">Managing Projects</span></span>](projects-manage-projects.md)  
<span data-ttu-id="da94f-130">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="da94f-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
