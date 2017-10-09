---
title: Documenten beheren, verwijderen of comprimeren | Microsoft Docs
description: Bewaar of verwijder uw historische gegevens.
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 10524be6bcfdc99672496b54903e4f04c33108ce
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="manage-documents"></a><span data-ttu-id="99415-103">Documenten beheren</span><span class="sxs-lookup"><span data-stu-id="99415-103">Manage Documents</span></span>
<span data-ttu-id="99415-104">Een centrale rol, bijvoorbeeld de toepassingsbeheerder, moet regelmatig de verzamelde historische documenten verwijderen of comprimeren.</span><span class="sxs-lookup"><span data-stu-id="99415-104">A central role, such as the application administrator, must regularly deal with accumulating historic documents by deleting or compressing them.</span></span>  

## <a name="delete-documents"></a><span data-ttu-id="99415-105">Documenten verwijderen</span><span class="sxs-lookup"><span data-stu-id="99415-105">Delete Documents</span></span>
<span data-ttu-id="99415-106">Het kan voorkomen dat u gefactureerde inkooporders moet verwijderen die niet automatisch zijn verwijderd.</span><span class="sxs-lookup"><span data-stu-id="99415-106">In certain situations, you may need to delete invoiced purchase orders that have not been deleted.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="99415-107"> controleert of de verwijderde inkooporders volledig zijn gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="99415-107"> checks that you have fully invoiced the deleted purchase orders.</span></span> <span data-ttu-id="99415-108">U kunt geen orders verwijderen die u niet volledig hebt ontvangen en gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="99415-108">You cannot delete orders that you have not fully invoiced and received.</span></span>  

<span data-ttu-id="99415-109">Nadat retourorders zijn gefactureerd, worden deze doorgaans verwijderd.</span><span class="sxs-lookup"><span data-stu-id="99415-109">Return orders are usually deleted after they are invoiced.</span></span> <span data-ttu-id="99415-110">Wanneer u een factuur boekt, wordt deze overgebracht naar het venster **Geboekte inkoopcreditnota**.</span><span class="sxs-lookup"><span data-stu-id="99415-110">When you post an invoice, it is transferred to the **Posted Purchase Credit Memo** window.</span></span> <span data-ttu-id="99415-111">Als u het selectievakje **Retourzending op creditnota** hebt ingeschakeld in het venster **Inkoopinstellingen**, wordt de factuur overgebracht naar het venster **Geboekte retourverzending**.</span><span class="sxs-lookup"><span data-stu-id="99415-111">If you selected the **Return Shipment on Credit Memo** check box in the **Purchases & Payable Setup** window, then the invoice is transferred to the **Posted Return Shipment** window.</span></span> <span data-ttu-id="99415-112">U kunt de documenten verwijderen met behulp van de batchverwerking **Gef. ink.-retourorders verw.**.</span><span class="sxs-lookup"><span data-stu-id="99415-112">You can delete the documents using the **Delete Invd Purch. Ret. Orders** batch job.</span></span> <span data-ttu-id="99415-113">Voordat de verwijdering wordt uitgevoerd, controleert de batchverwerking of inkoopretourorders volledig zijn verzonden en gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="99415-113">Before deleting, the batch job checks if the purchase return orders are fully shipped and invoiced.</span></span>  

<span data-ttu-id="99415-114">Inkoopraamcontracten worden niet verwijderd nadat u alle bijbehorende inkooporders hebt verwerkt en gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="99415-114">Blanket purchase orders are not deleted after you have processed and invoiced all the related purchase orders.</span></span> <span data-ttu-id="99415-115">U kunt raamcontracten verwijderen met de batchverwerking **Gefact. inkoopraamcontracten verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="99415-115">You can delete blanket orders with the **Delete Invoiced Blanket Purchase Orders** batch job.</span></span>  

<span data-ttu-id="99415-116">Gefactureerde servicefacturen worden doorgaans automatisch verwijderd als ze volledig zijn gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="99415-116">Invoiced service orders are usually deleted automatically after having been fully invoiced.</span></span> <span data-ttu-id="99415-117">Wanneer een factuur wordt geboekt, wordt een bijbehorende post gemaakt in het venster **Geboekte servicefacturen**.</span><span class="sxs-lookup"><span data-stu-id="99415-117">When an invoice is posted, a corresponding entry is created in the **Posted Service Invoices** window.</span></span> <span data-ttu-id="99415-118">U kunt het geboekte document bekijken in het venster **Geboekte servicefactuur**.</span><span class="sxs-lookup"><span data-stu-id="99415-118">The posted document can be viewed in the **Posted Service Invoice** window.</span></span>  

<span data-ttu-id="99415-119">Serviceorders worden echter niet automatisch verwijderd als het totale aantal op de order niet vanuit de serviceorder zelf is geboekt, maar vanuit het venster **Servicefactuur**.</span><span class="sxs-lookup"><span data-stu-id="99415-119">Service orders are not deleted automatically, however, if the total quantity on the order has been posted not from the service order itself, but from the **Service Invoice** window.</span></span> <span data-ttu-id="99415-120">In dit geval zult u wellicht gefactureerde orders die niet zijn verwijderd, zelf moeten verwijderen.</span><span class="sxs-lookup"><span data-stu-id="99415-120">Then you may need to delete invoiced orders that were not deleted.</span></span> <span data-ttu-id="99415-121">Hiervoor kunt u de batchverwerking **Gefactureerde serviceorders verwijderen** uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="99415-121">You can do this by running the **Delete Invoiced Service Orders** batch job.</span></span>  

## <a name="see-also"></a><span data-ttu-id="99415-122">Zie ook</span><span class="sxs-lookup"><span data-stu-id="99415-122">See Also</span></span>  
[<span data-ttu-id="99415-123">Installatie en beheer in Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="99415-123">Setup and Administration in Dynamics 365 for Financials</span></span>](admin-setup-and-administration.md)  
