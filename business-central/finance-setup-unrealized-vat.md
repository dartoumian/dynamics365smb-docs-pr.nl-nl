---
title: Ongerealiseerde btw instellen | Microsoft Docs
description: Als u op kas gebaseerde boekhouding gebruikt, kunt u opgeven hoe ongerealiseerde btw voor verkopen en inkopen moet worden verwerkt.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cash, VAT, unrealized, cash-based
ms.date: 09/08/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 5e21330cd7adc97da9023da7b18944a9f0450b8e
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---

# <a name="set-up-unrealized-vat-for-cash-based-accounting"></a><span data-ttu-id="7effd-103">Ongerealiseerde btw voor op kas gebaseerde boekhouding instellen</span><span class="sxs-lookup"><span data-stu-id="7effd-103">Set Up Unrealized VAT for Cash-Based Accounting</span></span>
<span data-ttu-id="7effd-104">Als u op kas gebaseerde boekhoudingsmethoden gebruikt, kunt u [!INCLUDE[d365fin](includes/d365fin_md.md)] instellen om ongerealiseerde btw te verwerken.</span><span class="sxs-lookup"><span data-stu-id="7effd-104">If you're using cash-based accounting methods, you can set up [!INCLUDE[d365fin](includes/d365fin_md.md)] to handle unrealized VAT.</span></span>

## <a name="to-use-general-ledger-accounts-for-unrealized-vat"></a><span data-ttu-id="7effd-105">Grootboekrekeningen gebruiken voor ongerealiseerde btw</span><span class="sxs-lookup"><span data-stu-id="7effd-105">To use general ledger accounts for unrealized VAT</span></span>
<span data-ttu-id="7effd-106">U kunt ervoor kiezen btw-bedragen te laten berekenen en boeken naar een tijdelijke grootboekrekening wanneer een factuur wordt geboekt. Vervolgens wordt de factuur geboekt naar de juiste grootboekrekening en opgenomen in btw-aangiften wanneer de werkelijke betaling van de factuur is geboekt.</span><span class="sxs-lookup"><span data-stu-id="7effd-106">You can choose to have VAT amounts calculated and posted to a temporary general ledger account when an invoice is posted, and then posted to the correct general ledger account and included in VAT statements when the actual payment of the invoice is posted.</span></span> <span data-ttu-id="7effd-107">Hiervoor moet u eerst de btw-boekingsinstellingen voltooien.</span><span class="sxs-lookup"><span data-stu-id="7effd-107">Before you can do this, you must complete the VAT posting setup.</span></span>

<span data-ttu-id="7effd-108">Ga als volgt te werk om rekeningen voor ongerealiseerde btw te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="7effd-108">To use accounts for unrealized VAT, follow these steps:</span></span>
1. <span data-ttu-id="7effd-109">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport") en voer **Grootboekinstellingen** in.</span><span class="sxs-lookup"><span data-stu-id="7effd-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, and enter **General Ledger Setup**.</span></span>
2. <span data-ttu-id="7effd-110">Kies op de pagina **Boekhoudinstellingen** op het sneltabblad **Algemeen** **Meer weergeven** en kies vervolgens het selectievakje **Ongerealiseerde btw**.</span><span class="sxs-lookup"><span data-stu-id="7effd-110">On the **General Ledger Setup** page, on the **General** FastTab, choose **Show More**, and then choose the **Unrealized VAT** check box.</span></span>
3. <span data-ttu-id="7effd-111">Sluit de pagina.</span><span class="sxs-lookup"><span data-stu-id="7effd-111">Close the page.</span></span>
4. <span data-ttu-id="7effd-112">Kies in de rechterbovenhoek het pictogram **Zoeken naar pagina of rapport** ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport") en voer **Btw-boekingsinstellingen** in.</span><span class="sxs-lookup"><span data-stu-id="7effd-112">choose the **Search for Page or Report** icon ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon"), and enter **VAT Posting Setup**.</span></span>
5. <span data-ttu-id="7effd-113">Op de pagina **Btw-boekingsinstellingen** kiest u de btw-boekingsgroep en vervolgens **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="7effd-113">On the **VAT Posting Setup** page, choose the VAT posting group, and then choose **Edit**.</span></span>
6. <span data-ttu-id="7effd-114">In het veld **Ongerealiseerde btw-soort** kiest u een optie om op te geven hoe u betalingen toewijst aan het factuurbedrag (zonder btw) en het btw-bedrag zelf, en hoe btw-bedragen van de ongerealiseerde btw-rekening moeten worden overgeboekt naar de gerealiseerde rekening.</span><span class="sxs-lookup"><span data-stu-id="7effd-114">In the **Unrealized VAT Type** field, choose an option to specify how to allocate payments to the invoice amount (excluding VAT) and the VAT amount itself, and how to transfer VAT amounts from the unrealized VAT account to the realized account.</span></span> <span data-ttu-id="7effd-115">De volgende tabel beschrijft de opties.</span><span class="sxs-lookup"><span data-stu-id="7effd-115">The following table describes the options.</span></span>

| <span data-ttu-id="7effd-116">Optie</span><span class="sxs-lookup"><span data-stu-id="7effd-116">Option</span></span> | <span data-ttu-id="7effd-117">Omschrijving</span><span class="sxs-lookup"><span data-stu-id="7effd-117">Description</span></span> |
| --- | --- |
| <span data-ttu-id="7effd-118">Leeg</span><span class="sxs-lookup"><span data-stu-id="7effd-118">Blank</span></span> | <span data-ttu-id="7effd-119">Kies deze optie als u de functie voor ongerealiseerde btw niet wilt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="7effd-119">Choose this option if you don't want to use the unrealized VAT feature.</span></span> |
| <span data-ttu-id="7effd-120">Percentage</span><span class="sxs-lookup"><span data-stu-id="7effd-120">Percentage</span></span> | <span data-ttu-id="7effd-121">Zowel het btw- als het factuurbedrag worden verrekend met de betalingen in verhouding tot het betalingspercentage van het resterende factuurbedrag.</span><span class="sxs-lookup"><span data-stu-id="7effd-121">Payments covers both VAT and the invoice amount in proportion to the payment's percentage of the remaining invoice amount.</span></span> <span data-ttu-id="7effd-122">Het betaalde btw-bedrag wordt van de ongerealiseerde btw-rekening overgeboekt naar de gerealiseerde btw-rekening.</span><span class="sxs-lookup"><span data-stu-id="7effd-122">The paid VAT amount is transferred from the unrealized VAT account to the realized VAT account.</span></span> |
| <span data-ttu-id="7effd-123">Eerste</span><span class="sxs-lookup"><span data-stu-id="7effd-123">First</span></span> | <span data-ttu-id="7effd-124">Eerst wordt het btw-bedrag verrekend met de betalingen en dan het factuurbedrag.</span><span class="sxs-lookup"><span data-stu-id="7effd-124">Payments cover VAT first and then invoice amounts.</span></span> <span data-ttu-id="7effd-125">Het bedrag dat van de ongerealiseerde btw-rekening wordt overgemaakt naar de btw-rekening, is dan gelijk aan het betalingsbedrag totdat de volledige btw is betaald.</span><span class="sxs-lookup"><span data-stu-id="7effd-125">In this case, the amount transferred from the unrealized VAT account to the VAT account will equal the amount of the payment until the total VAT has been paid.</span></span> |
| <span data-ttu-id="7effd-126">Laatste</span><span class="sxs-lookup"><span data-stu-id="7effd-126">Last</span></span> | <span data-ttu-id="7effd-127">Eerst wordt het factuurbedrag verrekend met de betalingen en dan het btw-bedrag.</span><span class="sxs-lookup"><span data-stu-id="7effd-127">Payments cover the invoice amount first and then VAT.</span></span> <span data-ttu-id="7effd-128">In dit geval wordt er alleen een bedrag van de ongerealiseerde btw-rekening overgeboekt naar de btw-rekening als het volledige factuurbedrag, exclusief de btw, is betaald.</span><span class="sxs-lookup"><span data-stu-id="7effd-128">In this case, no amount will be transferred from the unrealized VAT account to the VAT account until the total amount of the invoice, excluding VAT, has been paid.</span></span> |
| <span data-ttu-id="7effd-129">Eerste (Voll. bet.)</span><span class="sxs-lookup"><span data-stu-id="7effd-129">First (Fully Paid)</span></span> | <span data-ttu-id="7effd-130">Eerst wordt de btw verrekend met betalingen (zoals bij de optie _Eerste_), maar er wordt pas een bedrag naar de btw-rekening overgeboekt als het volledige btw-bedrag is betaald.</span><span class="sxs-lookup"><span data-stu-id="7effd-130">Payments will cover VAT first (like the _First_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span></span> |
| <span data-ttu-id="7effd-131">Laatste (Voll. bet.)</span><span class="sxs-lookup"><span data-stu-id="7effd-131">Last (Fully Paid)</span></span> | <span data-ttu-id="7effd-132">Eerst wordt het factuurbedrag verrekend met betalingen (zoals bij de optie _Laatste_), maar er wordt pas een bedrag naar de btw-rekening overgeboekt als het volledige btw-bedrag is betaald.</span><span class="sxs-lookup"><span data-stu-id="7effd-132">Payments will cover invoice amount first (like the _Last_ option), but no amount will be transferred to the VAT account until the full amount of VAT has been paid.</span></span> |

6. <span data-ttu-id="7effd-133">Kies in het veld **Ongerealiseerde verkoop-btw-rekening** de rekening voor ongerealiseerde verkoop-btw.</span><span class="sxs-lookup"><span data-stu-id="7effd-133">In the **Sales VAT Unreal. Account** field, choose the account for unrealized sales VAT.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="7effd-134">Het btw-bedrag wordt naar deze rekening geboekt en blijft daar tot de betaling van de klant is geboekt.</span><span class="sxs-lookup"><span data-stu-id="7effd-134">The VAT amount will be posted to this account, and stay there until the customer payment is posted.</span></span> <span data-ttu-id="7effd-135">Daarna wordt het bedrag overgeboekt naar de rekening voor verkoop-btw.</span><span class="sxs-lookup"><span data-stu-id="7effd-135">The amount is then transferred to the account for sales VAT.</span></span>
7. <span data-ttu-id="7effd-136">Voer in het veld **Ongereal. ink.-btw-rekening** de grootboekrekening voor ongerealiseerde inkoop-btw in.</span><span class="sxs-lookup"><span data-stu-id="7effd-136">In the **Purch. VAT Unreal. Account** field, enter the general ledger account for unrealized purchase VAT.</span></span>

    > [!NOTE]  
    >   <span data-ttu-id="7effd-137">Het btw-bedrag wordt naar deze rekening geboekt en blijft daar tot de betaling van de klant is geboekt.</span><span class="sxs-lookup"><span data-stu-id="7effd-137">The VAT amount will be posted to this account, and stay there until the customer payment is posted.</span></span> <span data-ttu-id="7effd-138">Daarna wordt het bedrag overgeboekt naar de rekening voor inkoop-btw.</span><span class="sxs-lookup"><span data-stu-id="7effd-138">The amount is then transferred to the account for purchase VAT.</span></span>

## <a name="see-also"></a><span data-ttu-id="7effd-139">Zie ook</span><span class="sxs-lookup"><span data-stu-id="7effd-139">See Also</span></span>
[<span data-ttu-id="7effd-140">Btw instellen</span><span class="sxs-lookup"><span data-stu-id="7effd-140">Setting Up Value Added Tax</span></span>](finance-setup-vat.md)
