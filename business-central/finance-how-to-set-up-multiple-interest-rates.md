---
title: Meerdere rentetarieven instellen
description: "U kunt rentefacturen berekenen met meerdere rentepercentages voor een bepaalde periode. De renteberekening is voor alle financiële kosten soortgelijk, met alleen variatie alleen in het rentepercentage voor een specifieke periode."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 12/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 0af01fe46f6b7df1149825c35a9fc0cc19482403
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-multiple-interest-rates"></a><span data-ttu-id="81214-104">Meerdere rentetarieven instellen</span><span class="sxs-lookup"><span data-stu-id="81214-104">Set Up Multiple Interest Rates</span></span>
<span data-ttu-id="81214-105">Meerdere rentepercentages worden gebruikt voor verschillende perioden voor vertraagde betalingen in handelstransacties.</span><span class="sxs-lookup"><span data-stu-id="81214-105">Multiple interest rates are used for different periods for delayed payments in trade transactions.</span></span> <span data-ttu-id="81214-106">Bijvoorbeeld, een overheid specificeert de maximumrente die voor een klant mag worden gerekend.</span><span class="sxs-lookup"><span data-stu-id="81214-106">For example, a government specifies the maximum interest to be levied for a consumer.</span></span> <span data-ttu-id="81214-107">Het rentepercentage kan twee keer per jaar op 1 januari en 1 juli worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="81214-107">This interest rate can be changed twice a year on 01 January and 01 July.</span></span> <span data-ttu-id="81214-108">Het rentepercentage tussen bedrijven (B2B) is overeengekomen door de partijen en er is geen limiet aan die klantgroep.</span><span class="sxs-lookup"><span data-stu-id="81214-108">The interest rate between businesses (B2B) is agreed by the parties and there is no limit to that customer group.</span></span> <span data-ttu-id="81214-109">Het aangekondigde tarief is gewoonlijk vier procent boven de normale bankrente.</span><span class="sxs-lookup"><span data-stu-id="81214-109">The announced rate is usually four percent more than the normal bank interest.</span></span>

<span data-ttu-id="81214-110">Wanneer u rentefactuurcondities maakt en aanmaningscondities, als sanctie voor vertraagde betaling, kunt u meerdere rentepercentages opgeven zodat de sanctietoeslag wordt berekend op basis van verschillende rentepercentages in verschillende perioden.</span><span class="sxs-lookup"><span data-stu-id="81214-110">When you create finance charge terms and reminder terms, for delayed payment penalty, you can specify multiple interest rates so that the penalty fee is calculated from different interest rates in different periods.</span></span> <span data-ttu-id="81214-111">Zie voor meer informatie [Openstaande saldi innen](receivables-collect-outstanding-balances.md).</span><span class="sxs-lookup"><span data-stu-id="81214-111">For more information, see [Collect Outstanding Balances](receivables-collect-outstanding-balances.md).</span></span>

## <a name="to-set-up-multiple-interest-rates"></a><span data-ttu-id="81214-112">Meerdere rentetarieven instellen</span><span class="sxs-lookup"><span data-stu-id="81214-112">To set up multiple interest rates</span></span>  
1.  <span data-ttu-id="81214-113">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Rentefactuurcondities** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="81214-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Finance Charge Terms**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="81214-114">Selecteer in het venster **Rentefactuurcondities** de gewenste rentefactuurconditie en kies de actie **Rentepercentages**.</span><span class="sxs-lookup"><span data-stu-id="81214-114">In the **Finance Charge Terms** window, select the required finance term, and then choose the **Interest Rates** action.</span></span>  
3.  <span data-ttu-id="81214-115">Vul de benodigde velden in.</span><span class="sxs-lookup"><span data-stu-id="81214-115">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  <span data-ttu-id="81214-116">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="81214-116">Choose the **OK** button.</span></span>  
5.  <span data-ttu-id="81214-117">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Aanmaningscondities** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="81214-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Reminder Terms**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="81214-118">Selecteer in het venster **Aanmaningscondities** de gewenste aanmaningsconditie en kies de actie **Niveaus**.</span><span class="sxs-lookup"><span data-stu-id="81214-118">In the **Reminder Terms** window, select the required reminder term, and then choose the **Levels** action.</span></span>  
7.  <span data-ttu-id="81214-119">Selecteer in het venster **Aanmaningsniveaus** het veld **Rente berekenen**.</span><span class="sxs-lookup"><span data-stu-id="81214-119">In the **Reminder Levels** window, select the **Calculate Interest** field.</span></span>  

<span data-ttu-id="81214-120">Wanneer u een rentefactuur verzendt, bevat de factuur de rentefacturen met meerdere rentepercentages in een bepaalde periode.</span><span class="sxs-lookup"><span data-stu-id="81214-120">When you issue a finance charge memo, the memo shows the finance charges with multiple interest rates for a specific time period.</span></span> <span data-ttu-id="81214-121">De factuur bevat ook de contactgegevens van de klant, het bedrijf dat de factuur verzendt, het extra bedrag en het totale bedrag.</span><span class="sxs-lookup"><span data-stu-id="81214-121">The memo also contains the contact details of the customer, the company issuing the memo, the additional amount, and the total amount.</span></span> <span data-ttu-id="81214-122">De openingspost op de factuur wordt vet weergegeven.</span><span class="sxs-lookup"><span data-stu-id="81214-122">The opening entry on the memo is displayed in bold.</span></span> <span data-ttu-id="81214-123">De rentefacturen worden berekend met meerdere rentepercentages voor een bepaalde periode en worden afgedrukt na de openingspost van de factuur.</span><span class="sxs-lookup"><span data-stu-id="81214-123">The finance charges are calculated with multiple interest rates for a specific time period and are printed after the opening entry of the memo.</span></span>  

## <a name="see-also"></a><span data-ttu-id="81214-124">Zie ook</span><span class="sxs-lookup"><span data-stu-id="81214-124">See Also</span></span>  
[<span data-ttu-id="81214-125">Openstaande saldi innen</span><span class="sxs-lookup"><span data-stu-id="81214-125">Collect Outstanding Balances</span></span>](receivables-collect-outstanding-balances.md)  
[<span data-ttu-id="81214-126">Financiën instellen</span><span class="sxs-lookup"><span data-stu-id="81214-126">Setting Up Finance</span></span>](finance-setup-finance.md)
