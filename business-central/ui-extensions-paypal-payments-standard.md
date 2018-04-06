---
title: De PayPal-extensie Payments Standard gebruiken | Microsoft Docs
description: >-
  Beschrijft hoe u de extensie gebruikt om klanten de mogelijkheid te bieden betalingen te doen met PayPal

  .
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 356f01706f40bdb8fd46871e3dbde73577a78117
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="the-paypal-payments-standard-extension-to-business-central"></a><span data-ttu-id="2aa31-103">De extensie PayPal Payments Standard voor Business Central</span><span class="sxs-lookup"><span data-stu-id="2aa31-103">The PayPal Payments Standard Extension to Business Central</span></span> 
<span data-ttu-id="2aa31-104">Klanten stellen steeds meer eisen aan de klantenservice, zowel met betrekking tot productkwaliteit als met betrekking tot betalings- en leveringsmogelijkheden.</span><span class="sxs-lookup"><span data-stu-id="2aa31-104">Customers continuously require higher customer service, both in terms of product quality but also in terms of delivery and payment options.</span></span> <span data-ttu-id="2aa31-105">De service PayPal-betalingsstandaard helpt u uw klantenservice te verbeteren.</span><span class="sxs-lookup"><span data-stu-id="2aa31-105">The PayPal Payments Standard service helps you increase your customer service.</span></span>

<span data-ttu-id="2aa31-106">Als alternatief voor het innen van betalingen door middel van bankoverschrijving of creditcards kunt u klanten aanbieden met hun PayPal-rekening te betalen.</span><span class="sxs-lookup"><span data-stu-id="2aa31-106">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span> <span data-ttu-id="2aa31-107">Wanneer u een verkoopfactuur of verkooporder verzendt per e-mail, is er een PayPal-koppeling in de e-mailhoofdtekst en in het gekoppelde PDF-document aanwezig.</span><span class="sxs-lookup"><span data-stu-id="2aa31-107">When you send a sales invoice or sales order by email, there is a PayPal link in the email body and in the attached PDF document.</span></span> <span data-ttu-id="2aa31-108">Wanneer klanten de koppeling kiezen, wordt de servicepagina van hun PayPal-account geopend waarin de betalingsdetails voor de verkoop worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="2aa31-108">When the customer chooses the link, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="2aa31-109">De klant kan de factuur vervolgens als elke andere PayPal-betaling betalen.</span><span class="sxs-lookup"><span data-stu-id="2aa31-109">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="2aa31-110">De service PayPal-betalingsstandaard biedt de volgende voordelen:</span><span class="sxs-lookup"><span data-stu-id="2aa31-110">The PayPal Payments Standard service provides the following benefits:</span></span>

* <span data-ttu-id="2aa31-111">Klantbetalingen komen sneller op uw bankrekening binnen.</span><span class="sxs-lookup"><span data-stu-id="2aa31-111">Customer payments arrive faster in your bank account.</span></span>
* <span data-ttu-id="2aa31-112">Klanten kunnen op meer manieren facturen betalen.</span><span class="sxs-lookup"><span data-stu-id="2aa31-112">Customers have more ways to pay invoices.</span></span>
* <span data-ttu-id="2aa31-113">PayPal biedt een betrouwbare betalingsservice, die klanten liever gebruiken dan dat ze creditcardinformatie op websites invoeren.</span><span class="sxs-lookup"><span data-stu-id="2aa31-113">PayPal offers a trustworthy payment service, which customers prefer to entering credit card information on web sites.</span></span>
* <span data-ttu-id="2aa31-114">PayPal biedt meerdere manieren om betalingen te verwerken, inclusief creditcardverwerking, PayPal-rekeningen en andere bronnen.</span><span class="sxs-lookup"><span data-stu-id="2aa31-114">PayPal offers multiple ways of handling payments, including credit card processing, PayPal accounts, and other sources.</span></span>
* <span data-ttu-id="2aa31-115">De PayPal-koppeling kan automatisch aan verkoopdocumenten worden toegevoegd of handmatig door de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="2aa31-115">The PayPal link can be added automatically to sales documents or manually by the user.</span></span>
* <span data-ttu-id="2aa31-116">Met de service PayPal-betalingsstandaard bent u geen maandelijkse kosten of installatiekosten kwijt.</span><span class="sxs-lookup"><span data-stu-id="2aa31-116">The PayPal Payments Standard service does not involve monthly fees or setup fees.</span></span>
* <span data-ttu-id="2aa31-117">Omdat het een extensie is, kunt u de PayPal-betalingsstandaard gemakkelijk inschakelen wanneer en als uw bedrijf het nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="2aa31-117">Because it is an extension, you can easily enable the PayPal Payment Standard service when and if your business requires it.</span></span>  

<span data-ttu-id="2aa31-118">Zie [Klantbetalingen via PayPal inschakelen](sales-how-enable-payment-service-extensions.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2aa31-118">For more information, see [Enable Customer Payment Through PayPal](sales-how-enable-payment-service-extensions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="2aa31-119">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2aa31-119">See Also</span></span>
<span data-ttu-id="2aa31-120">[[!INCLUDE[d365fin](includes/d365fin_md.md)] aanpassen met behulp van extensies](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="2aa31-120">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="2aa31-121">Verkopen instellen</span><span class="sxs-lookup"><span data-stu-id="2aa31-121">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="2aa31-122">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2aa31-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
