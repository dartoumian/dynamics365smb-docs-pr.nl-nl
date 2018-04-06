---
title: Een prioriteitsniveau toewijzen aan een leverancier | Microsoft Docs
description: U kunt nummers toewijzen aan uw leveranciers om deze te prioriteren en betalingsvoorstellen in Business Central te vergemakkelijken.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f7834f0f99b775125425eb7209c3c648de4ccd1f
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="prioritize-vendors"></a><span data-ttu-id="6ea11-103">De prioriteit van leveranciers bepalen</span><span class="sxs-lookup"><span data-stu-id="6ea11-103">Prioritize Vendors</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="6ea11-104"> heeft een functie die voorstellen kan doen voor betalingen aan leveranciers, bijvoorbeeld bij betalingen die binnenkort moeten worden betaald, of als voor een betaling een korting mogelijk is.</span><span class="sxs-lookup"><span data-stu-id="6ea11-104"> can suggest various payments to vendors, for example, payments that will be due soon or payments where a discount is available.</span></span> <span data-ttu-id="6ea11-105">Zie voor meer informatie [Leveranciersbetalingen voorstellen](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="6ea11-105">For more information, see [Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>

<span data-ttu-id="6ea11-106">Eerst moet u aan uw leveranciers eerst een prioriteit toewijzen door nummers aan hen toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="6ea11-106">First, you must prioritize your vendors by assigning numbers to them.</span></span>

## <a name="to-prioritize-vendors"></a><span data-ttu-id="6ea11-107">Leveranciers in een prioriteitsvolgorde plaatsen</span><span class="sxs-lookup"><span data-stu-id="6ea11-107">To prioritize vendors</span></span>
1. <span data-ttu-id="6ea11-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6ea11-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="6ea11-109">Selecteer de relevante leverancier en kies **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="6ea11-109">Select the relevant vendor, and then choose **Edit**.</span></span>
3. <span data-ttu-id="6ea11-110">Voer in het veld **Prioriteit** een nummer in.</span><span class="sxs-lookup"><span data-stu-id="6ea11-110">In the **Priority** field, enter a number.</span></span>

<span data-ttu-id="6ea11-111">In [!INCLUDE[d365fin](includes/d365fin_md.md)] heeft het laagste nummer, 0 uitgezonderd, de hoogste prioriteit.</span><span class="sxs-lookup"><span data-stu-id="6ea11-111">[!INCLUDE[d365fin](includes/d365fin_md.md)] considers the lowest number, except 0, to have the highest priority.</span></span> <span data-ttu-id="6ea11-112">Als u bijvoorbeeld de nummers 1, 2 en 3 toewijst, heeft nummer 1 de hoogste prioriteit.</span><span class="sxs-lookup"><span data-stu-id="6ea11-112">So, for example, if you use 1, 2, and 3, then 1 will have the highest priority.</span></span>

<span data-ttu-id="6ea11-113">Als u geen prioriteitsnummer wilt toekennen aan een leverancier, laat u het veld **Prioriteit** leeg.</span><span class="sxs-lookup"><span data-stu-id="6ea11-113">If you do not want to prioritize a vendor, leave the **Priority** field blank.</span></span> <span data-ttu-id="6ea11-114">Die leverancier wordt onder alle leveranciers met prioriteitsnummers geplaatst wanneer u betalingsvoorstellen in het programma inschakelt.</span><span class="sxs-lookup"><span data-stu-id="6ea11-114">Then, if you use the payment suggestion feature, the vendor will be listed after all the vendors that have a priority number.</span></span> <span data-ttu-id="6ea11-115">U kunt zo veel prioriteitsniveaus invoeren als er nodig zijn.</span><span class="sxs-lookup"><span data-stu-id="6ea11-115">You can enter as many priority levels as necessary.</span></span>

## <a name="see-also"></a><span data-ttu-id="6ea11-116">Zie ook</span><span class="sxs-lookup"><span data-stu-id="6ea11-116">See Also</span></span>
[<span data-ttu-id="6ea11-117">Inkoop instellen</span><span class="sxs-lookup"><span data-stu-id="6ea11-117">Setting Up Purchasing</span></span>](purchasing-setup-purchasing.md)  
[<span data-ttu-id="6ea11-118">Betalingsverplichtingen beheren</span><span class="sxs-lookup"><span data-stu-id="6ea11-118">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="6ea11-119">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="6ea11-119">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
