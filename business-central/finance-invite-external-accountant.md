---
title: Uw externe accountant toevoegen aan uw Financials | Microsoft Docs
description: Leer hoe u uw externe accountant kunt uitnodigen voor uw Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting
ms.date: 01/25/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: a252b967e910cb16179ef33fc9ec5e6b976056a7
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="inviting-your-external-accountant-to-your-included365finincludesd365finmdmd"></a><span data-ttu-id="60282-103">Uw externe accountant uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="60282-103">Inviting Your External Accountant to Your [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
<span data-ttu-id="60282-104">Als u een externe auditor gebruikt om uw boeken en financiële rapportage beheren, kunt u deze uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)], zodat hij of zij met u kan werken aan uw fiscale gegevens.</span><span class="sxs-lookup"><span data-stu-id="60282-104">If you use an external accountant to manage your books and financial reporting, you can invite them to your [!INCLUDE[d365fin](includes/d365fin_md.md)] so they can work with you on your fiscal data.</span></span>

<span data-ttu-id="60282-105">Als de accountant toegang heeft gekregen tot uw [!INCLUDE[d365fin](includes/d365fin_md.md)], kan hij of zij het rolcentrum **Accountant** gebruiken, dat eenvoudig toegang tot de meest relevante vensters voor hun werk biedt.</span><span class="sxs-lookup"><span data-stu-id="60282-105">Once your accountant has gained access to your [!INCLUDE[d365fin](includes/d365fin_md.md)], they can use the **Accountant** Role Center that gives easy access to the most relevant windows for their work.</span></span>  

## <a name="invite-your-accountant-to-your-included365finincludesd365finmdmd"></a><span data-ttu-id="60282-106">Uw accountant uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="60282-106">Invite Your Accountant to Your [!INCLUDE[d365fin](includes/d365fin_md.md)]</span></span>
<span data-ttu-id="60282-107">In de laatste versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] hebben we het voor u eenvoudig gemaakt om uw externe accountant uit te nodigen.</span><span class="sxs-lookup"><span data-stu-id="60282-107">In the latest version of [!INCLUDE[d365fin](includes/d365fin_md.md)], we have made it easy for you to invite your external accountant.</span></span> <span data-ttu-id="60282-108">Open gewoon het venster **Gebruikers** en kies de actie **Externe accountant uitnodigen** op het lint.</span><span class="sxs-lookup"><span data-stu-id="60282-108">Simply open the **Users** window, and then choose the **Invite External Accountant** action in the ribbon.</span></span> <span data-ttu-id="60282-109">Er wordt een e-mail voor u gemaakt. Voeg het werke-mailadres van uw accountant eraan toe en verzend de uitnodiging.</span><span class="sxs-lookup"><span data-stu-id="60282-109">An email is made ready for you, just add your accountant's work email, and send the invitation.</span></span>  

![Uw accountant uitnodigen](./media/finance-invite-accountant/invite-accountant.png)

> [!TIP]  
>  <span data-ttu-id="60282-111">Dit vereist dat u SMTP-e-mail hebt ingesteld.</span><span class="sxs-lookup"><span data-stu-id="60282-111">This requires that you have set up SMTP email.</span></span> <span data-ttu-id="60282-112">U kunt dit zelf doen of uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-partner vragen.</span><span class="sxs-lookup"><span data-stu-id="60282-112">You can do this yourself or ask your [!INCLUDE[d365fin](includes/d365fin_md.md)] partner.</span></span> <span data-ttu-id="60282-113">Daarnaast moet u als gebruikersbeheerder zijn aangemeld bij [!INCLUDE[d365fin](includes/d365fin_md.md)], niet als bedrijfeigenaar of een andere gebruiker.</span><span class="sxs-lookup"><span data-stu-id="60282-113">Also, you must be logged in to [!INCLUDE[d365fin](includes/d365fin_md.md)] as a user administrator, not as the business owner or other users.</span></span> <span data-ttu-id="60282-114">Ten slotte moet u het proefbedrijf hebben verlaten zodat u een Azure Active Directory Azure-beheerder hebt.</span><span class="sxs-lookup"><span data-stu-id="60282-114">Finally, you must have left the trial company so that you have an Azure Active Directory administrator.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="60282-115">Het e-mailadres van de accountant moet een werkadres op basis van Active Directory zijn.</span><span class="sxs-lookup"><span data-stu-id="60282-115">The accountant's email address must be a work address that is based an Active Directory.</span></span> <span data-ttu-id="60282-116">Als de accountant een ander type e-mail gebruikt, kan de uitnodiging niet worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="60282-116">If the accountant uses another type of email, then the invitation cannot be sent.</span></span>  

### <a name="separate-license"></a><span data-ttu-id="60282-117">Afzonderlijke licentie</span><span class="sxs-lookup"><span data-stu-id="60282-117">Separate License</span></span>
<span data-ttu-id="60282-118">Achter de schermen wordt de accountant toegevoegd aan uw Active Directory-tenant.</span><span class="sxs-lookup"><span data-stu-id="60282-118">Behind the scenes, the accountant is added to your Active Directory tenant.</span></span> <span data-ttu-id="60282-119">Uw beheerder kan controleren of de accountant de uitnodiging accepteert en de juiste licentie toegewezen krijgt.</span><span class="sxs-lookup"><span data-stu-id="60282-119">Your administrator can verify that the accountant accepts the invitation and is assigned the correct license.</span></span> <span data-ttu-id="60282-120">De stappen hiervoor zijn afhankelijk van het soort rekening in dat u hebt gebruikt toen u zich aanmeldde bij [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="60282-120">The steps for doing this depends on the type of account that you used when you signed up for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="60282-121">Dit onderwerp is gebaseerd op het gebruik van een Office 365-account dat Microsoft Azure Active Directory gebruikt.</span><span class="sxs-lookup"><span data-stu-id="60282-121">This topic is based on the use of an Office 365 account, which uses Microsoft Azure Active Directory.</span></span>  

<span data-ttu-id="60282-122">Als u uw abonnement op [!INCLUDE[d365fin](includes/d365fin_md.md)] hebt geactiveerd en het evaluatiebedrijf niet meer gebruikt, hebt u een Azure Active Directory-tenant.</span><span class="sxs-lookup"><span data-stu-id="60282-122">If you have activated your subscription of [!INCLUDE[d365fin](includes/d365fin_md.md)] and are no longer using the evaluation company, you have an Azure Active Directory tenant.</span></span> <span data-ttu-id="60282-123">De beheerder of [!INCLUDE[d365fin](includes/d365fin_md.md)]-partner beheert deze tenant in de [Azure-portal](https://portal.azure.com).</span><span class="sxs-lookup"><span data-stu-id="60282-123">Your administrator or [!INCLUDE[d365fin](includes/d365fin_md.md)] partner manages this tenant in the [Azure portal](https://portal.azure.com).</span></span> <span data-ttu-id="60282-124">Hier worden nieuwe gebruikers en toegevoegd en licenties toegepast en verwijderd.</span><span class="sxs-lookup"><span data-stu-id="60282-124">This is where new users are added and licenses are applied and removed.</span></span> <span data-ttu-id="60282-125">Zie voor meer informatie het [Microsoft Azure-portal - overzicht](https://docs.microsoft.com/en-us/azure/azure-portal-overview).</span><span class="sxs-lookup"><span data-stu-id="60282-125">For more information, see the [Microsoft Azure portal overview](https://docs.microsoft.com/en-us/azure/azure-portal-overview).</span></span>  

<span data-ttu-id="60282-126">Een van de licentiesoorten voor [!INCLUDE[d365fin](includes/d365fin_md.md)] is de *Externe accountant*-licentie.</span><span class="sxs-lookup"><span data-stu-id="60282-126">One of the license types for [!INCLUDE[d365fin](includes/d365fin_md.md)] is the *External Accountant* license.</span></span> <span data-ttu-id="60282-127">Dit licentiesoort is bedoeld voor gebruik door gebruikers zoals externe accountants.</span><span class="sxs-lookup"><span data-stu-id="60282-127">This license type is intended for use by users such as external accountants.</span></span> <span data-ttu-id="60282-128">Dit betekent dat u geen extra seat in uw huidige Active Directory hoeft te kopen of een van uw bestaande [!INCLUDE[d365fin](includes/d365fin_md.md)]-gebruikersaccounts voor uw externe accountant hoeft te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="60282-128">This means that you do not have to buy an extra seat in your current Active Directory or use one of your existing [!INCLUDE[d365fin](includes/d365fin_md.md)] user accounts on your external accountant.</span></span> <span data-ttu-id="60282-129">Als uw huidige Office 365-abonnement bijvoorbeeld 10 gebruikers bevat voor [!INCLUDE[d365fin](includes/d365fin_md.md)] en u momenteel 10 *Volwaardige gebruiker*-licenties gebruikt, kan uw beheerder gewoon uw externe accountant als gastgebruiker toevoegen in de Azure-portal en aan deze gebruiker zonder extra kosten de *Externe accountant*-licentie toewijzen.</span><span class="sxs-lookup"><span data-stu-id="60282-129">For example, if your current Office 365 subscription includes 10 users for [!INCLUDE[d365fin](includes/d365fin_md.md)], and you are currently using 10 *Full User* licenses, your administrator can simply add your external accountant as a guest user in the Azure portal and assign this user the *External Accountant* license at no additional cost.</span></span> <span data-ttu-id="60282-130">U kunt echter maar één gebruiker met de *Externe accountant*-licentie hebben.</span><span class="sxs-lookup"><span data-stu-id="60282-130">However, you can only have one user with the *External Accountant* license.</span></span> <span data-ttu-id="60282-131">Als u meer gebruikers wilt toevoegen, moet u uw Office 365-abonnement bijwerken.</span><span class="sxs-lookup"><span data-stu-id="60282-131">If you want to add more users, you must update your Office 365 subscription accordingly.</span></span>  

## <a name="see-also"></a><span data-ttu-id="60282-132">Zie ook</span><span class="sxs-lookup"><span data-stu-id="60282-132">See Also</span></span>
[<span data-ttu-id="60282-133">Financiën</span><span class="sxs-lookup"><span data-stu-id="60282-133">Finance</span></span>](finance.md)  
[<span data-ttu-id="60282-134">E-mail handmatig instellen of de begeleide instelling gebruiken</span><span class="sxs-lookup"><span data-stu-id="60282-134">Set Up Email Manually or Using the Assisted Setup</span></span>](admin-how-setup-email.md)  
[<span data-ttu-id="60282-135">Accountantervaringen in Business Central</span><span class="sxs-lookup"><span data-stu-id="60282-135">Accountant Experiences in Business Central </span></span>](finance-accounting.md)  
[<span data-ttu-id="60282-136">Business Central voor Accountants op Microsoft.com</span><span class="sxs-lookup"><span data-stu-id="60282-136">Business Central for Accountants on Microsoft.com</span></span>](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  
