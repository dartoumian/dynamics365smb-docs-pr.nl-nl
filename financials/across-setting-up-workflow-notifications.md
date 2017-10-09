---
title: Werkstroomberichten instellen | Microsoft Docs
description: In veel werkstroomantwoorden wordt aan een gebruiker gemeld dat er een gebeurtenis is opgetreden waarop deze moet reageren. De gebeurtenis in een werkstroomstap kan bijvoorbeeld zijn dat Gebruiker 1 de goedkeuring van een nieuwe record aanvraagt, en het antwoord is dat er een bericht wordt verzonden naar Gebruiker 2, de fiatteur. In de volgende werkstroomstap kan de gebeurtenis zijn dat Gebruiker 2 de record goedkeurt, en het antwoord is dat er een bericht wordt verzonden naar Gebruiker 3, die een gerelateerde bewerking van de goedgekeurde record start. Voor werkstroomstappen die betrekking hebben op goedkeuring, is elk bericht gekoppeld aan een goedkeuringspost.
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
ms.openlocfilehash: 222056cc8b505d0ed027492d764ff4cde7f68795
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="setting-up-workflow-notifications"></a><span data-ttu-id="46dfd-106">Werkstroomberichten instellen</span><span class="sxs-lookup"><span data-stu-id="46dfd-106">Setting Up Workflow Notifications</span></span>
<span data-ttu-id="46dfd-107">In veel werkstroomantwoorden wordt aan een gebruiker gemeld dat er een gebeurtenis is opgetreden waarop deze moet reageren.</span><span class="sxs-lookup"><span data-stu-id="46dfd-107">Many workflow responses are about notifying a user that an event has occurred that they must act on.</span></span> <span data-ttu-id="46dfd-108">De gebeurtenis in een werkstroomstap kan bijvoorbeeld zijn dat Gebruiker 1 de goedkeuring van een nieuwe record aanvraagt, en het antwoord is dat er een bericht wordt verzonden naar Gebruiker 2, de fiatteur.</span><span class="sxs-lookup"><span data-stu-id="46dfd-108">For example, on one workflow step, the event can be that User 1 requests approval of a new record, and the response is that a notification is sent to User 2, the approver.</span></span> <span data-ttu-id="46dfd-109">In de volgende werkstroomstap kan de gebeurtenis zijn dat Gebruiker 2 de record goedkeurt, en het antwoord is dat er een bericht wordt verzonden naar Gebruiker 3, die een gerelateerde bewerking van de goedgekeurde record start.</span><span class="sxs-lookup"><span data-stu-id="46dfd-109">On the next workflow step, the event can be that User 2 approves the record, and the response is that a notification is sent to User 3 to start a related processing of the approved record.</span></span> <span data-ttu-id="46dfd-110">Voor werkstroomstappen die betrekking hebben op goedkeuring, is elk bericht gekoppeld aan een goedkeuringspost.</span><span class="sxs-lookup"><span data-stu-id="46dfd-110">For workflow steps that are about approval, each notification is tied to an approval entry.</span></span> <span data-ttu-id="46dfd-111">Zie [Werkstroom](across-workflow.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="46dfd-111">For more information, see [Workflow](across-workflow.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="46dfd-112">De algemene versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] ondersteunt berichten als e-mail en als interne opmerking.</span><span class="sxs-lookup"><span data-stu-id="46dfd-112">The generic version of [!INCLUDE[d365fin](includes/d365fin_md.md)] supports notifications as email and as internal notes.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="46dfd-113">Alle werkstroomberichten worden verzonden via een taakwachtrij.</span><span class="sxs-lookup"><span data-stu-id="46dfd-113">All workflow notifications are sent through a job queue.</span></span> <span data-ttu-id="46dfd-114">Zorg ervoor dat de verwerkingswachtrij in uw oplossing.</span><span class="sxs-lookup"><span data-stu-id="46dfd-114">Make sure that the job queue in your solution.</span></span> <span data-ttu-id="46dfd-115">Zie voor meer informatie [Gebruik van taakwachtrijen om taken te plannen](admin-job-queues-schedule-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="46dfd-115">For more information, see [Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md).</span></span>

<span data-ttu-id="46dfd-116">U stelt verschillende aspecten van werkstroomberichten op de volgende plaatsen in:</span><span class="sxs-lookup"><span data-stu-id="46dfd-116">You set up different aspects of workflow notifications in the following places:</span></span>  

1.  <span data-ttu-id="46dfd-117">Voor goedkeuringswerkstromen kunt u de ontvangers van werkstroomberichten instellen door in het venster **Gebruikersinstellingen voor goedkeuring** een regel in te vullen voor elke gebruiker die deelneemt aan de werkstroom.</span><span class="sxs-lookup"><span data-stu-id="46dfd-117">For approval workflows, you set up the recipients of workflow notifications by filling a line in the **Approval User Setup** window for each user that takes part in the workflow.</span></span> <span data-ttu-id="46dfd-118">Als bijvoorbeeld Gebruiker 2 wordt opgegeven in het veld **Fiatteur-id** op de regel voor Gebruiker 1, wordt het bericht over de goedkeuringsaanvraag verzonden naar Gebruiker 1.</span><span class="sxs-lookup"><span data-stu-id="46dfd-118">For example, if User 2 is specified in the **Approver ID** field on the line for User 1, then the approval request notification is sent to User 1.</span></span> <span data-ttu-id="46dfd-119">Zie voor meer informatie [Procedure: Goedkeuringsgebruikers instellen](across-how-to-set-up-approval-users.md).</span><span class="sxs-lookup"><span data-stu-id="46dfd-119">For more information, see [How to: Set Up Approval Users](across-how-to-set-up-approval-users.md).</span></span>  
2.  <span data-ttu-id="46dfd-120">U stelt in wanneer en hoe gebruikers werkstroomberichten ontvangen door het venster **Berichtplanning** in te vullen voor elke werkstroomgebruiker.</span><span class="sxs-lookup"><span data-stu-id="46dfd-120">You set when and how users receive workflow notifications by filling the **Notification Schedule** window for each workflow user.</span></span> <span data-ttu-id="46dfd-121">Zie voor meer informatie [Procedure: Vastleggen wanneer en hoe gebruikers berichten ontvangen](across-how-to-specify-when-and-how-to-receive-notifications.md).</span><span class="sxs-lookup"><span data-stu-id="46dfd-121">For more information, see [How to: Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md).</span></span>  
3.  <span data-ttu-id="46dfd-122">U stelt de algemene inhoud en opmaak van berichten in, inclusief berichten over achterstallige werkstroomantwoorden, door berichtsjablonen in te stellen in het venster **Berichtsjablonen**.</span><span class="sxs-lookup"><span data-stu-id="46dfd-122">You set up the general content and layout of notifications, including notifications about overdue workflow responses, by setting up notification templates in the **Notification Templates** window.</span></span> <span data-ttu-id="46dfd-123">U kunt de standaardsjablonen gebruiken die worden geleverd bij [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="46dfd-123">You can use the default templates provided with [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
4.  <span data-ttu-id="46dfd-124">U stelt specifieke inhoud en regels van een werkstroombericht in als u de betreffende werkstroom maakt.</span><span class="sxs-lookup"><span data-stu-id="46dfd-124">You set up specific content and rules of a workflow notification when you create the workflow in question.</span></span> <span data-ttu-id="46dfd-125">U doet dit door opties te selecteren in het **Opties werkstroomreactie** voor het werkstroomantwoord dat het bericht representeert.</span><span class="sxs-lookup"><span data-stu-id="46dfd-125">You do this by selecting options in the **Workflow Response Options** window for the workflow response that represents the notification.</span></span> <span data-ttu-id="46dfd-126">Zie voor meer informatie stap 9 in [Procedure: Werkstromen maken](across-how-to-create-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="46dfd-126">For more information, see step 9 in [How to: Create Workflows](across-how-to-create-workflows.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="46dfd-127">Zie ook</span><span class="sxs-lookup"><span data-stu-id="46dfd-127">See Also</span></span>  
 <span data-ttu-id="46dfd-128">[Procedure: Goedkeuringsgebruikers instellen](across-how-to-set-up-approval-users.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-128">[How to: Set Up Approval Users](across-how-to-set-up-approval-users.md) </span></span>  
 <span data-ttu-id="46dfd-129">[Procedure: Werkstroomgebruikers instellen](across-how-to-set-up-workflow-users.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-129">[How to: Set Up Workflow Users](across-how-to-set-up-workflow-users.md) </span></span>  
 <span data-ttu-id="46dfd-130">[Procedure: Vastleggen wanneer en hoe gebruikers berichten ontvangen](across-how-to-specify-when-and-how-to-receive-notifications.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-130">[How to: Specify When and How to Receive Notifications](across-how-to-specify-when-and-how-to-receive-notifications.md) </span></span>  
 <span data-ttu-id="46dfd-131">[Procedure: Werkstromen maken](across-how-to-create-workflows.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-131">[How to: Create Workflows](across-how-to-create-workflows.md) </span></span>  
 <span data-ttu-id="46dfd-132">[Procedure: Berichtsjablonen beheren](across-how-to-manage-notification-templates.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-132">[How to: Manage Notification Templates](across-how-to-manage-notification-templates.md) </span></span>  
 <span data-ttu-id="46dfd-133">[Gebruik van taakwachtrijen om taken te plannen](admin-job-queues-schedule-tasks.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-133">[Use Job Queues to Schedule Tasks](admin-job-queues-schedule-tasks.md) </span></span>  
 <span data-ttu-id="46dfd-134">[Procedure: E-mail instellen](madeira-how-setup-email.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-134">[How to: Set up Email](madeira-how-setup-email.md) </span></span>  
 <span data-ttu-id="46dfd-135">[Procedure: Een werkstroom voor inkoopgoedkeuring instellen en gebruiken](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span><span class="sxs-lookup"><span data-stu-id="46dfd-135">[Walkthrough: Setting Up and Using a Purchase Approval Workflow](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md) </span></span>  
 [<span data-ttu-id="46dfd-136">Werkstroom</span><span class="sxs-lookup"><span data-stu-id="46dfd-136">Workflow</span></span>](across-workflow.md)   
