---
title: Rapportage voor Business Central instellen in Power BI | Microsoft Docs
description: U kunt uw Financials-gegevens als gegevensbron in Power BI beschikbaar maken en krachtige rapporten maken van de status van uw bedrijf.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: business intelligence, KPI, Odata, Power App, SOAP, analysis
ms.date: 12/21/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 42939e97d121bd3a2abff91671d9f9571faffbfd
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="using-included365finincludesd365finmdmd-as-power-bi-data-source-for-building-reports"></a><span data-ttu-id="919f2-103">[!INCLUDE[d365fin](includes/d365fin_md.md)] gebruiken als Power BI-gegevensbron voor het maken van rapporten</span><span class="sxs-lookup"><span data-stu-id="919f2-103">Using [!INCLUDE[d365fin](includes/d365fin_md.md)] as Power BI Data Source for Building Reports</span></span>
<span data-ttu-id="919f2-104">U kunt uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens als gegevensbron in Power BI beschikbaar maken en krachtige rapporten maken van de status van uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="919f2-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in Power BI and build powerful reports of the state of your business.</span></span>  

> [!NOTE]  
> <span data-ttu-id="919f2-105">U moet een geldig account bij [!INCLUDE[d365fin](includes/d365fin_md.md)] en Power BI hebben.</span><span class="sxs-lookup"><span data-stu-id="919f2-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Power BI.</span></span> <span data-ttu-id="919f2-106">Ook moet u [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) downloaden.</span><span class="sxs-lookup"><span data-stu-id="919f2-106">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/).</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-power-bi-desktop"></a><span data-ttu-id="919f2-107">[!INCLUDE[d365fin](includes/d365fin_md.md)] als gegevensbron in Power BI Desktop toevoegen</span><span class="sxs-lookup"><span data-stu-id="919f2-107">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in Power BI Desktop</span></span>
1. <span data-ttu-id="919f2-108">Kies in Power BI Desktop in het linkernavigatievenster **Gegevens ophalen**.</span><span class="sxs-lookup"><span data-stu-id="919f2-108">In Power BI Desktop, in the left navigation pane, choose **Get Data**.</span></span>
2. <span data-ttu-id="919f2-109">Kies in het venster **Gegevens ophalen** achtereenvolgens **Online Services**, **Dynamics 365 Business Central** en de knop **Verbinden**.</span><span class="sxs-lookup"><span data-stu-id="919f2-109">In the **Get Data** window, choose **Online Services**, choose **Dynamics 365 Business Central**, and then choose the **Connect** button.</span></span>
3. <span data-ttu-id="919f2-110">Power BI geeft een wizard weer die u door het [verbindingsproces](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md) begeleidt.</span><span class="sxs-lookup"><span data-stu-id="919f2-110">Power BI displays a wizard that will guide you through the [connection process](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md).</span></span> <span data-ttu-id="919f2-111">De eerste stap is u aan te melden voor de service.</span><span class="sxs-lookup"><span data-stu-id="919f2-111">The first step will be to sign into the service.</span></span> <span data-ttu-id="919f2-112">Selecteer **Aanmelden** en kies het account waaronder u zich wilt aanmelden.</span><span class="sxs-lookup"><span data-stu-id="919f2-112">Select **Sign in** and choose the account you would like to sign in as.</span></span> <span data-ttu-id="919f2-113">Dit moet hetzelfde account zijn als waarmee u zich aanmeldt bij [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="919f2-113">This should be the same account you sign into [!INCLUDE[d365fin](includes/d365fin_md.md)] with.</span></span>
4. <span data-ttu-id="919f2-114">Kies de knop **Verbinding maken** om door te gaan.</span><span class="sxs-lookup"><span data-stu-id="919f2-114">Choose the **Connect** button to continue.</span></span> <span data-ttu-id="919f2-115">De Power BI-wizard bevat een lijst met [!INCLUDE[d365fin](includes/d365fin_md.md)]-bedrijven en -gegevensbronnen.</span><span class="sxs-lookup"><span data-stu-id="919f2-115">The Power BI wizard shows a list of [!INCLUDE[d365fin](includes/d365fin_md.md)] companies and data sources.</span></span> <span data-ttu-id="919f2-116">Met deze gegevensbron worden alle webservices vertegenwoordigd die u hebt gepubliceerd vanuit elk bedrijf in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="919f2-116">These data source represent all the web services that you have published from each company in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>
5. <span data-ttu-id="919f2-117">U kunt ook een nieuwe webservice-URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] maken met behulp van de actie **Gegevensset maken** op de pagina **Webservices** met de begeleide instelling **Rapportage instellen** of door de actie **Bewerken in Excel** in de lijsten te kiezen.</span><span class="sxs-lookup"><span data-stu-id="919f2-117">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>
6. <span data-ttu-id="919f2-118">Geef de gegevens op die u aan uw gegevensmodel wilt toevoegen en kies vervolgens de knop **Laden**.</span><span class="sxs-lookup"><span data-stu-id="919f2-118">Specify the data you want to add to your data model, and then choose the **Load** button.</span></span>
7. <span data-ttu-id="919f2-119">Herhaal de vorige stappen om aanvullende [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens aan uw Power BI-gegevensmodel toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="919f2-119">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span></span>

> [!NOTE]  
> <span data-ttu-id="919f2-120">Zodra u met succes verbinding hebt gemaakt met [!INCLUDE[d365fin](includes/d365fin_md.md)], wordt u niet opnieuw gevraagd zich aan te melden.</span><span class="sxs-lookup"><span data-stu-id="919f2-120">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again to sign in.</span></span>

<span data-ttu-id="919f2-121">Zodra de gegevens zijn geladen, worden deze in de rechternavigatie op de pagina weergegeven.</span><span class="sxs-lookup"><span data-stu-id="919f2-121">Once the data is loaded it will appear in the right navigation on the page.</span></span> <span data-ttu-id="919f2-122">Nu hebt u met succes een verbinding gemaakt met uw Business Central-gegevens en kunt u uw Power BI-rapport gaan maken.</span><span class="sxs-lookup"><span data-stu-id="919f2-122">At this point, you have successfully connected to your Business Central data and are ready to begin building your Power BI report.</span></span> <span data-ttu-id="919f2-123">Zie de [Power BI-documentatie](https://powerbi.microsoft.com/documentation/powerbi-landing-page/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="919f2-123">For more information, see the [Power BI documentation](https://powerbi.microsoft.com/documentation/powerbi-landing-page/).</span></span>

## <a name="see-also"></a><span data-ttu-id="919f2-124">Zie ook</span><span class="sxs-lookup"><span data-stu-id="919f2-124">See Also</span></span>
[<span data-ttu-id="919f2-125">Bedrijfsinformatie</span><span class="sxs-lookup"><span data-stu-id="919f2-125">Business Intelligence</span></span>](bi.md)  
<span data-ttu-id="919f2-126">[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="919f2-126">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="919f2-127">Bedrijfsgegevens importeren uit andere financiële systemen</span><span class="sxs-lookup"><span data-stu-id="919f2-127">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="919f2-128">[Instellen [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md) </span><span class="sxs-lookup"><span data-stu-id="919f2-128">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md) </span></span>  
[<span data-ttu-id="919f2-129">Financiën</span><span class="sxs-lookup"><span data-stu-id="919f2-129">Finance</span></span>](finance.md)  
<span data-ttu-id="919f2-130">[Power BI verbinden met [!INCLUDE[d365fin](includes/d365fin_md.md)]](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md)</span><span class="sxs-lookup"><span data-stu-id="919f2-130">[Connecting Power BI to [!INCLUDE[d365fin](includes/d365fin_md.md)]](across-how-to-connect-powerbi-dynamics-365-content-packs-help.md)</span></span>  
