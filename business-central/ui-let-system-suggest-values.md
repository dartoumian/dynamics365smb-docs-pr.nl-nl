---
title: Voorgestelde veldwaarden instellen | Microsoft Docs
description: Als u handmatige berekeningen wilt voorkomen en taken snel en accuraat wilt voltooien, kunt u automatische gegevensinvoer instellen, zodat Business Central geselecteerde velden invult.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 08/15/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 916b18e94415d34ec1d61330243a3658cfea6947
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="letting-included365finincludesd365finmdmd-suggest-values"></a><span data-ttu-id="4c37a-103">[!INCLUDE[d365fin](includes/d365fin_md.md)] waarden laten voorstellen</span><span class="sxs-lookup"><span data-stu-id="4c37a-103">Letting [!INCLUDE[d365fin](includes/d365fin_md.md)] Suggest Values</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="4c37a-104"> kan u helpen taken sneller en correcter te voltooien door velden vooraf te vullen of regels te vullen met gegevens die u anders zelf moet berekenen en invoeren.</span><span class="sxs-lookup"><span data-stu-id="4c37a-104"> can help you complete tasks quicker and more correctly by prefilling fields or complete lines with data that you would otherwise have to calculate and enter yourself.</span></span> <span data-ttu-id="4c37a-105">Hoewel dergelijke automatische gegevensinvoer altijd correct is, kunt u deze later wijzigen als u wilt.</span><span class="sxs-lookup"><span data-stu-id="4c37a-105">Although such automatic data entry is always correct, you can change it afterwards if you want to.</span></span>

<span data-ttu-id="4c37a-106">De functionaliteit waarmee veldwaarden voor u worden ingevoerd, wordt meestal aangeboden voor taken waarin u grote volumes transactiegegevens invoert en fouten wilt voorkomen en tijd wilt besparen.</span><span class="sxs-lookup"><span data-stu-id="4c37a-106">Functionality that enters field values for you is typically offered for tasks where you enter large volumes of transactional data and want to avoid errors and save time.</span></span> <span data-ttu-id="4c37a-107">Dit onderwerp bevat een selectie van deze functionaliteit.</span><span class="sxs-lookup"><span data-stu-id="4c37a-107">This topic contains a selection of such functionality.</span></span> <span data-ttu-id="4c37a-108">In toekomstige updates van [!INCLUDE[d365fin](includes/d365fin_md.md)] worden meer secties toegevoegd.</span><span class="sxs-lookup"><span data-stu-id="4c37a-108">More sections will be added in future updates of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="the-suggest-balancing-amount-check-box-in-the-general-journal-batches-window"></a><span data-ttu-id="4c37a-109">Het selectievakje **Salderingsbedrag voorstellen** in het venster **Fin. dagboekbatches**</span><span class="sxs-lookup"><span data-stu-id="4c37a-109">The **Suggest Balancing Amount** check box in the **General Journal Batches** window</span></span>
<span data-ttu-id="4c37a-110">Wanneer u bijvoorbeeld dagboekregels invoert voor meerdere uitgaven die allemaal naar dezelfde bankrekening moeten worden geboekt, kunt u telkens als u een nieuwe dagboekregel voor een uitgave invoert, het veld **Bedrag** op de bankrekeningregel automatisch laten bijwerken in het bedrag waarmee de uitgaven sluitend worden gemaakt.</span><span class="sxs-lookup"><span data-stu-id="4c37a-110">When, for example, you are entering general journal lines for multiple expenses that must all be posted to the same bank account, then each time you enter a new journal line for an expense, you can have the **Amount** field on the bank account line automatically updated to the amount that balances the expenses.</span></span> <span data-ttu-id="4c37a-111">Zie [Werken met diversendagboeken](ui-work-general-journals.md) voor meer informatie over het werken met diversendagboeken.</span><span class="sxs-lookup"><span data-stu-id="4c37a-111">For more information about working with general journals, see [Working with General Journals](ui-work-general-journals.md).</span></span>

### <a name="to-have-the-amount-field-on-balancing-general-journal-lines-filled-automatically"></a><span data-ttu-id="4c37a-112">Het veld **Bedrag** op salderingsdagboekregels automatisch laten invullen</span><span class="sxs-lookup"><span data-stu-id="4c37a-112">To have the **Amount** field on balancing general journal lines filled automatically</span></span>
1. <span data-ttu-id="4c37a-113">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Dagboeken** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4c37a-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="4c37a-114">Op de regel voor de dagboekbatch van uw voorkeur kiest u het selectievakje **Salderingsbedrag voorstellen**.</span><span class="sxs-lookup"><span data-stu-id="4c37a-114">On the line for your preferred general journal batch, choose the **Suggest Balancing Amount** check box.</span></span>
3. <span data-ttu-id="4c37a-115">Open het dagboek en ga door met het registreren en boeken van transacties met de beschreven functie voor automatische invoer van een veldwaarde.</span><span class="sxs-lookup"><span data-stu-id="4c37a-115">Open the general journal and proceed to register and post transactions using the described functionality for automatic entry of a field value.</span></span>       

<span data-ttu-id="4c37a-116">Zie [Werken met diversendagboeken](ui-work-general-journals.md) voor meer informatie over het instellen van een persoonlijke dagboekbatch, bijvoorbeeld voor de verwerking van uitgaven.</span><span class="sxs-lookup"><span data-stu-id="4c37a-116">For information about how to set up a personal general journal batch, for example, for expense handling, see [Working with General Journals](ui-work-general-journals.md).</span></span>

## <a name="the-automatically-fill-date-received-field-in-the-payment-registration-window"></a><span data-ttu-id="4c37a-117">Het veld **Ontvangstdatum automatisch invullen** in het venster **Betalingsregistratie**</span><span class="sxs-lookup"><span data-stu-id="4c37a-117">The **Automatically Fill Date Received** field in the **Payment Registration** window</span></span>
<span data-ttu-id="4c37a-118">Het venster **Betalingsregistratie** bevat openstaande inkomende betalingen als regels die geboekte verkoopdocumenten vertegenwoordigen waar een betalingstermijn voor een bedrag is verstreken.</span><span class="sxs-lookup"><span data-stu-id="4c37a-118">The **Payment Registration** window shows outstanding incoming payments as lines that represent sales documents where an amount is due for payment.</span></span> <span data-ttu-id="4c37a-119">Zie [Klantbetalingen van een lijst met onbetaalde verkoopdocumenten handmatig reconciliëren](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md) voor meer informatie over het vereffenen van klantbetalingen.</span><span class="sxs-lookup"><span data-stu-id="4c37a-119">For more information about applying customer payments, see [Reconcile Customer Payments Manually From a List of Unpaid Sales Documents](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md).</span></span>

<span data-ttu-id="4c37a-120">Uw hoofdacties in het venster bestaan eruit het selectievakje **Is betaald** en het veld **Ontvangen op** in te vullen.</span><span class="sxs-lookup"><span data-stu-id="4c37a-120">You main actions in the window are to fill in the **Payment Made** check box and the **Date Received** field.</span></span> <span data-ttu-id="4c37a-121">U kunt [!INCLUDE[d365fin](includes/d365fin_md.md)] zo instellen dat automatisch een werkdatum in het veld **Ontvangen op** wordt ingevoerd wanneer u het selectievakje **Is betaald** inschakelt.</span><span class="sxs-lookup"><span data-stu-id="4c37a-121">You can set [!INCLUDE[d365fin](includes/d365fin_md.md)] up to automatically enter work date in the **Date Received** field when you select the **Payment Made** check box.</span></span>

### <a name="to-have-the-date-received-field-in-the-payment-registration-window-filled-automatically"></a><span data-ttu-id="4c37a-122">Het veld **Ontvangen op** in het venster **Betalingsregistratie** automatisch laten invullen</span><span class="sxs-lookup"><span data-stu-id="4c37a-122">To have the **Date Received** field in the **Payment Registration** window filled automatically</span></span>
1. <span data-ttu-id="4c37a-123">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Instellingen van betalingsregistratie** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4c37a-123">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Registration Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="4c37a-124">Schakel het selectievakje **Ontvangstdatum automatisch invullen** in.</span><span class="sxs-lookup"><span data-stu-id="4c37a-124">Select the **Automatically Fill Date Received** check box.</span></span>
3. <span data-ttu-id="4c37a-125">Open het venster **Betalingregistratie** en ga door met het verwerken van inkomende klantbetalingen met de beschreven functie voor automatische invoer van een veldwaarde.</span><span class="sxs-lookup"><span data-stu-id="4c37a-125">Open the **Payment Registration** window and proceed to process incoming customer payments using the described functionality for automatic entry of a field value.</span></span>

## <a name="see-also"></a><span data-ttu-id="4c37a-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4c37a-126">See Also</span></span>
<span data-ttu-id="4c37a-127">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4c37a-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="4c37a-128">Financiën</span><span class="sxs-lookup"><span data-stu-id="4c37a-128">Finance</span></span>](finance.md)
