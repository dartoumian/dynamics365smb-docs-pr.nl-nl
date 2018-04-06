---
title: De lay-out opgeven van een cheque| Microsoft Docs
description: U kunt uw cheques ontwerpen en afdrukken in verschillende indelingen, om te voldoen aan standaards.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: print check, customize
ms.date: 06/15/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: d48b7954402b96c1bb5d3a2a63c70f48c6a4f9d7
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="define-check-layouts"></a><span data-ttu-id="4b3e9-103">Cheque-indelingen definiëren</span><span class="sxs-lookup"><span data-stu-id="4b3e9-103">Define Check Layouts</span></span>
<span data-ttu-id="4b3e9-104">U kunt uw eigen cheques ontwerpen in overeenstemming met de standaards die zijn ingesteld door de plaatselijke autoriteiten.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-104">You can design your checks to conform with the standards set by the local authorities.</span></span> <span data-ttu-id="4b3e9-105">Chequeafbeeldingen kunnen worden afgedrukt in het Engels, Frans of Spaans.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-105">Check images can be printed in English, French, or Spanish.</span></span>

<span data-ttu-id="4b3e9-106">Cheques worden ontworpen om te worden afgedrukt in zowel Amerikaanse als Canadese chequeafbeeldingsindelingen, in een cheque-strook-cheque indeling of een strook-strook-cheque indeling.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-106">Checks are designed to print in both the United States and Canadian check image formats in either a check-stub-check format or a stub-stub-check format.</span></span>

## <a name="to-define-check-layouts"></a><span data-ttu-id="4b3e9-107">Cheque-indelingen definiëren</span><span class="sxs-lookup"><span data-stu-id="4b3e9-107">To define check layouts</span></span>
1. <span data-ttu-id="4b3e9-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Zoeken naar pagina of rapport"), voer **Rapportselecties bankrekening** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Report Selections Bank Account**, and then choose the related link.</span></span>
2. <span data-ttu-id="4b3e9-109">Selecteer in het venster **Rapportselectie - Bank** in het veld **Gebruik** de optie **Cheque**.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-109">In the **Report Selection - Bank Acc.** window, in the **Usage** field, select **Check**.</span></span>
3. <span data-ttu-id="4b3e9-110">Selecteer een van de volgende rapport-id's.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-110">Select one of the following report IDs.</span></span>

| <span data-ttu-id="4b3e9-111">Rapport-id</span><span class="sxs-lookup"><span data-stu-id="4b3e9-111">Report ID</span></span> | <span data-ttu-id="4b3e9-112">Rapportnaam</span><span class="sxs-lookup"><span data-stu-id="4b3e9-112">Report Name</span></span> | <span data-ttu-id="4b3e9-113">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="4b3e9-113">Description</span></span> |
| --- | --- | --- |
| <span data-ttu-id="4b3e9-114">1401</span><span class="sxs-lookup"><span data-stu-id="4b3e9-114">1401</span></span> |<span data-ttu-id="4b3e9-115">Cheque</span><span class="sxs-lookup"><span data-stu-id="4b3e9-115">Check</span></span> |<span data-ttu-id="4b3e9-116">Dit is het standaardrapport.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-116">This is the default report.</span></span> |
| <span data-ttu-id="4b3e9-117">10401</span><span class="sxs-lookup"><span data-stu-id="4b3e9-117">10401</span></span> |<span data-ttu-id="4b3e9-118">Cheque (strook/strook/cheque)</span><span class="sxs-lookup"><span data-stu-id="4b3e9-118">Check (Stub/Stub/Check)</span></span> |<span data-ttu-id="4b3e9-119">Dit rapport is ontworpen om cheques af te drukken in de indeling strook/strook/cheque.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-119">This report is designed to print checks in a stub/stub/check format.</span></span> |
| <span data-ttu-id="4b3e9-120">10411</span><span class="sxs-lookup"><span data-stu-id="4b3e9-120">10411</span></span> |<span data-ttu-id="4b3e9-121">Cheque (strook/cheque/strook)</span><span class="sxs-lookup"><span data-stu-id="4b3e9-121">Check (Stub/Check/Stub)</span></span> |<span data-ttu-id="4b3e9-122">Dit rapport is ontworpen om cheques af te drukken in de indeling cheque/strook/cheque.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-122">This report is designed to print checks in a check/stub/check format.</span></span> |

<span data-ttu-id="4b3e9-123">Wanneer u de cheque-indelingen hebt ingesteld, kunt u cheques afdrukken vanuit het venster **Betalingsdagboek**.</span><span class="sxs-lookup"><span data-stu-id="4b3e9-123">When you have set up check layouts, you can print checks from the **Payment Journal** window.</span></span> <span data-ttu-id="4b3e9-124">Zie voor meer informatie [Werken met cheques](payables-how-work-checks.md).</span><span class="sxs-lookup"><span data-stu-id="4b3e9-124">For more information, see [Work with Checks](payables-how-work-checks.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="4b3e9-125">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4b3e9-125">See Also</span></span>
[<span data-ttu-id="4b3e9-126">Betalingsverplichtingen beheren</span><span class="sxs-lookup"><span data-stu-id="4b3e9-126">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="4b3e9-127">[Bankrekeningen beheren](bank-manage-bank-accounts.md) </span><span class="sxs-lookup"><span data-stu-id="4b3e9-127">[Managing Bank Accounts](bank-manage-bank-accounts.md) </span></span>  
[<span data-ttu-id="4b3e9-128">Periodeafsluitingsprocessen voltooien</span><span class="sxs-lookup"><span data-stu-id="4b3e9-128">Completing Period-End Processes</span></span>](year-how-complete-period-end-processes.md)  
<span data-ttu-id="4b3e9-129">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4b3e9-129">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="4b3e9-130">Algemene bedrijfsfunctionaliteit</span><span class="sxs-lookup"><span data-stu-id="4b3e9-130">General Business Functionality</span></span>](ui-across-business-areas.md)
