---
title: Serviceoffertes maken | Microsoft Docs
description: In het venster **Serviceofferte** kunt u documenten maken waarin u op aanvraag van de klant voor serviceartikelen gegevens invoert over een service, bijvoorbeeld herstel en onderhoud. U kunt een serviceofferte gebruiken als voorlopig ontwerp voor een serviceorder en de offerte vervolgens omzetten in een serviceorder.
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
ms.openlocfilehash: d5348e7b15eb0337f2a5f829c871dadcf3133b86
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-create-service-quotes"></a><span data-ttu-id="610ee-104">Procedure: Serviceoffertes maken</span><span class="sxs-lookup"><span data-stu-id="610ee-104">How to: Create Service Quotes</span></span>
<span data-ttu-id="610ee-105">U kunt serviceoffertes als de basis voor serviceorders zien.</span><span class="sxs-lookup"><span data-stu-id="610ee-105">You can think of service quotes as the basis for service orders.</span></span> <span data-ttu-id="610ee-106">Ze zijn zelfs vrijwel identiek.</span><span class="sxs-lookup"><span data-stu-id="610ee-106">In fact, they are almost identical.</span></span> <span data-ttu-id="610ee-107">Ze bevatten beide informatie, bijvoorbeeld over wie de klant is, het soort order, het artikel dat service vereist, facturerings- en verzendingsgegevens, en informatie over het werkelijke servicewerk.</span><span class="sxs-lookup"><span data-stu-id="610ee-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span></span>
 
<span data-ttu-id="610ee-108">U kunt een serviceofferte gebruiken als voorlopig ontwerp voor een serviceorder en de offerte vervolgens omzetten in een serviceorder.</span><span class="sxs-lookup"><span data-stu-id="610ee-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span></span>  
  
## <a name="to-create-a-service-quote"></a><span data-ttu-id="610ee-109">Serviceoffertes maken</span><span class="sxs-lookup"><span data-stu-id="610ee-109">To create a service quote</span></span>  
1. <span data-ttu-id="610ee-110">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Serviceoffertes** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="610ee-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="610ee-111">Een nieuwe serviceofferte maken.</span><span class="sxs-lookup"><span data-stu-id="610ee-111">Create a new service quote.</span></span>  
3. <span data-ttu-id="610ee-112">Selecteer in het veld **Nr.**</span><span class="sxs-lookup"><span data-stu-id="610ee-112">In the **No.**</span></span> <span data-ttu-id="610ee-113">een nummer op voor de serviceofferte.</span><span class="sxs-lookup"><span data-stu-id="610ee-113">field, enter a number for the service quote.</span></span> <span data-ttu-id="610ee-114">Als u in het venster **Servicebeheerinstellingen** nummerreeksen voor serviceoffertes hebt ingesteld, kunt u ook op Enter drukken om het eerstvolgende beschikbare serviceoffertenummer in te voeren.</span><span class="sxs-lookup"><span data-stu-id="610ee-114">Alternatively, if you have set up a number series for service quotes in the **Service Mgt. Setup** window, you can press Enter to select the next available service quote number.</span></span>  
4. <span data-ttu-id="610ee-115">Voer in het veld **Klantnr.**</span><span class="sxs-lookup"><span data-stu-id="610ee-115">In the **Customer No.**</span></span>  <span data-ttu-id="610ee-116">de betreffende klant uit de lijst.</span><span class="sxs-lookup"><span data-stu-id="610ee-116">field, select the relevant customer from the list.</span></span>  

  > [!Note]  
  >  <span data-ttu-id="610ee-117">De klantvelden worden automatisch ingevuld met gegevens uit de **Klantenkaart**.</span><span class="sxs-lookup"><span data-stu-id="610ee-117">The customer fields are filled in automatically with information from the **Customer** card.</span></span> <span data-ttu-id="610ee-118">Als er geen **klantenkaart** bestaat voor de klant en u een klantensjabloon hebt ingesteld, kunt u de klant vanuit de serviceofferte maken.</span><span class="sxs-lookup"><span data-stu-id="610ee-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span></span> <span data-ttu-id="610ee-119">Vul de relevante velden in en kies de actie **Klant maken**.</span><span class="sxs-lookup"><span data-stu-id="610ee-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span></span>  
  
5. <span data-ttu-id="610ee-120">Afhankelijk van de instellingen op het sneltabblad **Verplichte velden** in het venster **CRM - Service-instellingen** moet u wellicht het veld **Serviceordersoort** en het veld **Verkoper** invullen.</span><span class="sxs-lookup"><span data-stu-id="610ee-120">Depending on the settings on the **Mandatory Fields** FastTab in the **Service Mgt. Setup** window, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="610ee-121">Vul de serviceartikelregels in.</span><span class="sxs-lookup"><span data-stu-id="610ee-121">Fill in the service item lines.</span></span>  
7. <span data-ttu-id="610ee-122">Registreer de geschatte kosten op de serviceregels.</span><span class="sxs-lookup"><span data-stu-id="610ee-122">Register estimated costs on the service lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="610ee-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="610ee-123">See Also</span></span>  
[<span data-ttu-id="610ee-124">Procedure: Serviceorders maken</span><span class="sxs-lookup"><span data-stu-id="610ee-124">How to: Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
[<span data-ttu-id="610ee-125">Procedure: Werken aan servicetaken</span><span class="sxs-lookup"><span data-stu-id="610ee-125">How to: Work on Service tasks</span></span>](service-how-to-work-on-service-tasks.md)  

 