---
title: 'Procedure: Assemblageboeking ongedaan maken | Microsoft Docs'
description: Soms moet u mogelijk een geboekte assemblageorder verwijderen, zoals wanneer de order is geboekt met fouten die moeten worden gecorrigeerd of omdat deze niet geboekt had mogen worden en moet worden teruggedraaid.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: c6d15f43e2a308dc8107e7a58e64f4b98452b1db
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-undo-assembly-posting"></a><span data-ttu-id="a1a85-103">Procedure: boeken van assemblage ongedaan maken</span><span class="sxs-lookup"><span data-stu-id="a1a85-103">How to: Undo Assembly Posting</span></span>
<span data-ttu-id="a1a85-104">Soms moet u mogelijk een geboekte assemblageorder verwijderen, zoals wanneer de order is geboekt met fouten die moeten worden gecorrigeerd of omdat deze niet geboekt had mogen worden en moet worden teruggedraaid.</span><span class="sxs-lookup"><span data-stu-id="a1a85-104">Sometimes you may need to undo a posted assembly order, for example when the order was posted with mistakes that must be corrected, or because it should not have been posted in the first place and must be rolled back.</span></span>

<span data-ttu-id="a1a85-105">Wanneer u een geboekte assemblageorder ongedaan wilt maken, wordt er een set met corrigerende artikelposten gemaakt om de oorspronkelijke posten terug te draaien.</span><span class="sxs-lookup"><span data-stu-id="a1a85-105">When you undo a posted assembly order, a set of corrective item ledger entries is created to reverse the original entries.</span></span> <span data-ttu-id="a1a85-106">Elke positieve uitvoerpost voor het assemblageartikel wordt via een negatieve uitvoerpost teruggedraaid.</span><span class="sxs-lookup"><span data-stu-id="a1a85-106">Each positive output entry for the assembly item is reversed by a negative output entry.</span></span> <span data-ttu-id="a1a85-107">Elk negatieve verbruiksartikelpost voor een assemblagecomponent wordt via een positieve verbruikspost teruggedraaid.</span><span class="sxs-lookup"><span data-stu-id="a1a85-107">Each negative consumption entry for an assembly component is reversed by a positive consumption entry.</span></span> <span data-ttu-id="a1a85-108">Er wordt automatisch een vaste kostenvereffening gemaakt tussen de corrigerende en de oorspronkelijke posten om een exacte kostenterugboeking te garanderen.</span><span class="sxs-lookup"><span data-stu-id="a1a85-108">Fixed cost application is automatically created between the corrective and original entries to ensure exact cost reversal.</span></span>  

<span data-ttu-id="a1a85-109">Wanneer u een volledig geboekte assemblageorder ongedaan maakt, kunt u er vervolgens voor kiezen om de assemblageorder opnieuw te maken op basis van de oorspronkelijke staat, zodat u bijvoorbeeld correcties kunt aanbrengen voordat u deze opnieuw boekt.</span><span class="sxs-lookup"><span data-stu-id="a1a85-109">When you undo a fully posted assembly order, then you can choose to recreate the assembly order to its original state, for example to make corrections before reposting it.</span></span> <span data-ttu-id="a1a85-110">U kunt er ook voor kiezen om de assemblageorder niet opnieuw te maken.</span><span class="sxs-lookup"><span data-stu-id="a1a85-110">Alternatively, you can choose to not recreate the assembly order.</span></span>  

<span data-ttu-id="a1a85-111">Wanneer u een gedeeltelijk geboekte assemblageorder ongedaan maakt, worden vervolgens alle betrokken velden, zoals de velden **Geassembleerde hoeveelheid**, **Verbruikt aantal** en **Resterend aantal**, opnieuw ingesteld op de waarden die deze hadden voordat de desbetreffende boeking werd uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="a1a85-111">When you undo a partially posted assembly order, then all affected quantity fields, such as the **Assembled Quantity**, **Consumed Quantity**, and **Remaining Quantity** fields are restored to the values they had before the posting in question.</span></span>  

<span data-ttu-id="a1a85-112">Als u assemblageorders opnieuw wilt maken of wilt terugzetten, moeten het assemblage-artikel dat in de oorspronkelijke boeking is uitgevoerd, voldoen aan de volgende voorwaarden:</span><span class="sxs-lookup"><span data-stu-id="a1a85-112">To recreate or restore assembly orders, the following conditions must apply to the assembly item that was output in the original posting:</span></span>  

-   <span data-ttu-id="a1a85-113">Het artikel moet zich nog steeds in de voorraad bevinden, met andere woorden, het artikel mag niet zijn verkocht of anderszins zijn verbruikt ten behoeve van uitgaande transacties.</span><span class="sxs-lookup"><span data-stu-id="a1a85-113">It must still be in inventory, that is, it is not sold or otherwise consumed by outbound transactions.</span></span>  
-   <span data-ttu-id="a1a85-114">Het artikel mag niet gereserveerd zijn.</span><span class="sxs-lookup"><span data-stu-id="a1a85-114">It must not be reserved.</span></span>  
-   <span data-ttu-id="a1a85-115">Het artikel moet bestaan op de opslaglocatie waarnaar dit is uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="a1a85-115">It must exist in the bin that it was output to.</span></span>  

<span data-ttu-id="a1a85-116">Verder kunnen bestaande assemblageorders uitsluitend worden teruggedraaid als het aantal regels en de volgorde van de regels op de oorspronkelijke assemblageorder niet zijn gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="a1a85-116">In addition, existing assembly orders can only be restored if the number of lines and the sequence of lines on the original assembly order are not changed.</span></span>  

> [!TIP]  
>  <span data-ttu-id="a1a85-117">Als u conflicten ten gevolge van regelwijzigingen wilt oplossen, kunt de wijzigingen op de desbetreffende regels handmatig ongedaan maken voordat u de bijbehorende assemblageorder boekt.</span><span class="sxs-lookup"><span data-stu-id="a1a85-117">To solve conflicts due to line changes, you can manually revert the changes on the lines in question before undoing the related posted assembly order.</span></span> <span data-ttu-id="a1a85-118">U kunt de assemblageorder ook volledig boeken en er vervolgens voor kiezen om deze opnieuw te maken wanneer u de boeking ongedaan maakt.</span><span class="sxs-lookup"><span data-stu-id="a1a85-118">Alternatively, you can post the assembly order fully and then select to recreate it when undoing the posting.</span></span>  

<span data-ttu-id="a1a85-119">De volgende procedure beschrijft het ongedaan maken van geboekte assemblageorders waarvoor artikelen zijn geassembleerd voor voorraad.</span><span class="sxs-lookup"><span data-stu-id="a1a85-119">The following procedure describes how to undo posted assembly orders where the items were assembled to stock.</span></span> <span data-ttu-id="a1a85-120">Als u geboekte assemblageorders waarvoor artikelen zijn geassembleerd ten behoeve van een verkooporder ongedaan wilt maken, moet u de functie **Verzending ongedaan maken** gebruiken voor de geboekte verzending die betrekking heeft op de geboekte assemblageorder.</span><span class="sxs-lookup"><span data-stu-id="a1a85-120">If you want to undo posted assembly orders where the items were assembled to a sales order, then you must use the **Undo Shipment** function on the posted shipment that relates to the posted assembly order.</span></span> <span data-ttu-id="a1a85-121">Zie voor meer informatie [Procedure: Boekingen tegenboeken](finance-how-reverse-journal-posting.md).</span><span class="sxs-lookup"><span data-stu-id="a1a85-121">For more information, see [How to: Reverse Postings](finance-how-reverse-journal-posting.md).</span></span> <span data-ttu-id="a1a85-122">Het ongedaan het maken van de geboekte assemblageorder geschiedt vervolgens automatisch en op dezelfde wijze als in dit onderwerp is beschreven.</span><span class="sxs-lookup"><span data-stu-id="a1a85-122">The undoing of the posted assembly order then happens automatically in the same way as described in this topic.</span></span>  

## <a name="to-undo-posting-of-an-assembly-order"></a><span data-ttu-id="a1a85-123">Het boeken van een assemblageorder ongedaan maken</span><span class="sxs-lookup"><span data-stu-id="a1a85-123">To undo posting of an assembly order</span></span>  
1.  <span data-ttu-id="a1a85-124">Als u een volledig of gedeeltelijk geboekte assemblyorder ongedaan wilt maken, kiest u het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voert u **Geboekte assemblyorders** in en kiest u de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="a1a85-124">To undo a fully or partially posted assembly order, Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Assembly Orders**, and choose the related link.</span></span>  

    <span data-ttu-id="a1a85-125">Het venster **Geboekte assemblageorders** wordt geopend met een of meer assemblageorders die zijn geboekt voor de assemblageorder in kwestie.</span><span class="sxs-lookup"><span data-stu-id="a1a85-125">The **Posted Assembly Orders** window opens showing one or more posted assembly orders that are posted from the assembly order in question.</span></span> <span data-ttu-id="a1a85-126">Elke gedeeltelijke boeking leidt tot het maken van een afzonderlijk geboekte assemblageorder.</span><span class="sxs-lookup"><span data-stu-id="a1a85-126">Each partial posting creates a separate posted assembly order.</span></span>  
2.  <span data-ttu-id="a1a85-127">Open de geboekte assemblyorder die u ongedaan wilt maken en kies vervolgens de actie **Assemblage ongedaan maken**.</span><span class="sxs-lookup"><span data-stu-id="a1a85-127">Open the posted assembly order that you want to undo, and then choose the **Undo Assembly** action.</span></span>  

    <span data-ttu-id="a1a85-128">Als de geboekte assemblageorder die u ongedaan wilt maken betrekking heeft op een volledig geboekte assemblageorder die nu wordt verwijderd, hebt u de mogelijkheid om deze opnieuw te maken omdat u deze gewoonlijk opnieuw zult willen verwerken.</span><span class="sxs-lookup"><span data-stu-id="a1a85-128">If the posted assembly order that you want to undo relates to a fully posted assembly order that is now deleted, then you have the option to recreate it, typically because you want to reprocess it.</span></span>  
3.  <span data-ttu-id="a1a85-129">Klik op de knop **Ja** als u de assemblageorder opnieuw wilt maken.</span><span class="sxs-lookup"><span data-stu-id="a1a85-129">If you want to recreate the assembly order, choose the **Yes** button.</span></span> <span data-ttu-id="a1a85-130">Klik op de knop **Nee** als u de boeking ongedaan wilt maken zonder de bijbehorende assemblageorder opnieuw te maken.</span><span class="sxs-lookup"><span data-stu-id="a1a85-130">To undo the posting without recreating the related assembly order, choose the **No** button.</span></span>  

<span data-ttu-id="a1a85-131">Het veld **Tegengeboekt** in de assemblageorder verandert in **Ja**.</span><span class="sxs-lookup"><span data-stu-id="a1a85-131">The **Reversed** field on the assembly order header changes to **Yes**.</span></span> <span data-ttu-id="a1a85-132">De assemblageorderboeking is nu teruggedraaid en u kunt doorgaan met het verwerken van de gehele assemblageorder als u ervoor kiest om deze opnieuw te maken of om de assemblageorder die u in de oorspronkelijke hebt teruggezet, te openen.</span><span class="sxs-lookup"><span data-stu-id="a1a85-132">The assembly order posting is now reversed, and you can proceed to process the entire assembly order if you chose to recreate it or the open assembly order that you have restored to its original state.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="a1a85-133">Als u aantallen uit meerdere gedeeltelijke boekingen voor een assemblageorder wilt herstellen, moet u alle geboekte assemblageorders in kwestie ongedaan maken door voor elke geboekte assemblageorder de hiervoor beschreven stappen 1 tot en met 3 uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="a1a85-133">To restore quantities from multiple partial postings in an assembly order, you must undo all the posted assembly orders in question by following steps 1 through 3 above for each posted assembly order.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a1a85-134">Zie ook</span><span class="sxs-lookup"><span data-stu-id="a1a85-134">See Also</span></span>  
[<span data-ttu-id="a1a85-135">Assemblagebeheer</span><span class="sxs-lookup"><span data-stu-id="a1a85-135">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="a1a85-136">Procedure: boekingen tegenboeken</span><span class="sxs-lookup"><span data-stu-id="a1a85-136">How to: Reverse Postings</span></span>](finance-how-reverse-journal-posting.md)  
<span data-ttu-id="a1a85-137">[Procedure: Verkoopretouren of annuleringen verwerken](sales-how-process-sales-returns-cancellations.md)  </span><span class="sxs-lookup"><span data-stu-id="a1a85-137">[How to: Process Sales Returns or Cancellations](sales-how-process-sales-returns-cancellations.md)  </span></span>  
[<span data-ttu-id="a1a85-138">Procedure: Werken met stuklijsten</span><span class="sxs-lookup"><span data-stu-id="a1a85-138">How to: Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="a1a85-139">Voorraad</span><span class="sxs-lookup"><span data-stu-id="a1a85-139">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="a1a85-140">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="a1a85-140">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="a1a85-141">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a1a85-141">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
