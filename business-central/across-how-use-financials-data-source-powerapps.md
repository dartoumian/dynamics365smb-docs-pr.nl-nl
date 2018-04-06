---
title: Gebruik uw gegevens om een app te maken| Microsoft Docs
description: U kunt uw Financials-gegevens als gegevensbron beschikbaar maken en een OData-URL van uw webservices opgeven om een bedrijfsapp te maken met PowerApps.
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Odata, Power App, SOAP
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 8db67d30ba18e9f7dba14b93ddf7b4de6e2b6444
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="connecting-to-your-financials-data-to-build-a-business-app-using-powerapps"></a><span data-ttu-id="b1a54-103">Verbinding met uw Financials-gegevens maken om een bedrijfsapp te maken met PowerApps</span><span class="sxs-lookup"><span data-stu-id="b1a54-103">Connecting to Your Financials Data to Build a Business App Using PowerApps</span></span>
<span data-ttu-id="b1a54-104">U kunt uw gegevens [!INCLUDE[d365fin](includes/d365fin_md.md)] als gegevensbron beschikbaar maken in PowerApps.</span><span class="sxs-lookup"><span data-stu-id="b1a54-104">You can make your [!INCLUDE[d365fin](includes/d365fin_md.md)] data available as a data source in PowerApps.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="b1a54-105">U moet een geldig account bij [!INCLUDE[d365fin](includes/d365fin_md.md)] en PowerApps hebben.</span><span class="sxs-lookup"><span data-stu-id="b1a54-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with PowerApps.</span></span>  

## <a name="to-add-included365finincludesd365finmdmd-as-a-data-source-in-powerapps"></a><span data-ttu-id="b1a54-106">[!INCLUDE[d365fin](includes/d365fin_md.md)] als gegevensbron in PowerApps toevoegen</span><span class="sxs-lookup"><span data-stu-id="b1a54-106">To add [!INCLUDE[d365fin](includes/d365fin_md.md)] as a data source in PowerApps</span></span>
1. <span data-ttu-id="b1a54-107">Navigeer in de browser naar [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/) en meld u aan.</span><span class="sxs-lookup"><span data-stu-id="b1a54-107">In your browser, navigate to [powerapps.microsoft.com](https://powerapps.microsoft.com/en-us/), and then sign in.</span></span>
2. <span data-ttu-id="b1a54-108">Kies in het linkernavigatievenster de optie **Nieuwe app**.</span><span class="sxs-lookup"><span data-stu-id="b1a54-108">In the left navigation pane, choose **New App**.</span></span>
3. <span data-ttu-id="b1a54-109">Kies uw editor, PowerApps Studio for Windows of PowerApps Studio for Web.</span><span class="sxs-lookup"><span data-stu-id="b1a54-109">Choose your editor, PowerApps Studio for Windows or PowerApps Studio for Web.</span></span>

   <span data-ttu-id="b1a54-110">PowerApps Studio for Windows is een bureaubladtoepassing die wordt gebruikt om PowerApps te maken en te publiceren.</span><span class="sxs-lookup"><span data-stu-id="b1a54-110">PowerApps Studio for Windows is a desktop application used to create and publish PowerApps.</span></span> <span data-ttu-id="b1a54-111">PowerApps Studio for Web is de online oplossing die wordt gebruikt om PowerApps te maken en te publiceren.</span><span class="sxs-lookup"><span data-stu-id="b1a54-111">The PowerApps Studio for Web is the online solution used to create and publish PowerApps.</span></span>
4. <span data-ttu-id="b1a54-112">De volgende stap om een PowerApp te maken bestaat eruit uw gegevens te selecteren.</span><span class="sxs-lookup"><span data-stu-id="b1a54-112">The next step to create a PowerApp is to select your data.</span></span> <span data-ttu-id="b1a54-113">Kies het pijlpictogram en kies vervolgens de optie **Nieuwe verbinding** linksboven in de pagina.</span><span class="sxs-lookup"><span data-stu-id="b1a54-113">Choose the Arrow icon then choose the **New connection** option in the upper left side of the page.</span></span>
5. <span data-ttu-id="b1a54-114">In de lijst met beschikbare verbindingen kiest u **Dynamics 365 Business Central**.</span><span class="sxs-lookup"><span data-stu-id="b1a54-114">In the list of available connections, choose **Dynamics 365 Business Central**.</span></span>
6. <span data-ttu-id="b1a54-115">Met PowerApps wordt een verbindingspagina weergegeven waarin u wordt gevraagd om de gegevens die zijn vereist om verbinding te maken met uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens.</span><span class="sxs-lookup"><span data-stu-id="b1a54-115">PowerApps will display a connection page that prompts you for the information that is required to connect to your [!INCLUDE[d365fin](includes/d365fin_md.md)] data.</span></span> <span data-ttu-id="b1a54-116">Als u verbinding wilt maken, moet u een URL, gebruikersnaam, wachtwoord en bedrijfsnaam voor OData opgeven.</span><span class="sxs-lookup"><span data-stu-id="b1a54-116">To connect, you must specify an OData URL, username, password, and company name.</span></span>

   <span data-ttu-id="b1a54-117">Voor de *OData-URL* kunt u de URL van OData V4 kopiëren van een van de webservices die worden weergegeven op de pagina **Webservices** in [!INCLUDE[d365fin](includes/d365fin_md.md)], zoals `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span><span class="sxs-lookup"><span data-stu-id="b1a54-117">For the *OData URL*, you can copy the OData V4 URL of any of the web services that are listed in the **Web Services** page in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `https://mycompany.financials.dynamics.com:7048/MS/ODataV4/`.</span></span>  

   <span data-ttu-id="b1a54-118">Voor *Bedrijfsnaam* gebruikt u de naam van het veld **Naam** in het venster **Bedrijfsgegevens** in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b1a54-118">For the *Company Name*, use the name that is shown in the **Name** field in the **Company Information** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b1a54-119">Als [!INCLUDE[d365fin](includes/d365fin_md.md)] meerdere bedrijven bevat, kies u de relevante bedrijfsnaam in de lijst van het venster **Bedrijven**.</span><span class="sxs-lookup"><span data-stu-id="b1a54-119">If your [!INCLUDE[d365fin](includes/d365fin_md.md)] contains multiple companies, choose the relevant company name from the list in the **Companies** window.</span></span> <span data-ttu-id="b1a54-120">In beide gevallen moet u ervoor zorgen dat de naam die u in de PowerApps-wizard opgeeft, exact overeenkomt met de tekst die in [!INCLUDE[d365fin](includes/d365fin_md.md)] wordt weergegeven, zoals `My Company`.</span><span class="sxs-lookup"><span data-stu-id="b1a54-120">In both cases, make sure that the name that you specify in the PowerApps wizard matches exactly the text shown in [!INCLUDE[d365fin](includes/d365fin_md.md)], such as `My Company`.</span></span>

   <span data-ttu-id="b1a54-121">Voor de gebruikersnaam en het wachtwoord gebruikt u de naam en de toegangssleutel van de webservice die voor uw account worden weergegeven in het venster **Gebruikers** in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b1a54-121">For the username and password, use the name and web service access key that are specified for your account in the **Users** window in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b1a54-122">Uw gebruikersnaam is bijvoorbeeld *ADMIN* en de webservicetoegangssleutel die dient als uw wachtwoord, is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span><span class="sxs-lookup"><span data-stu-id="b1a54-122">For example, your username is *ADMIN*, and the web service access key that serves as your password is *EgzeUFQ9Uv0o5O0lUMyqCzo1ueUW9yRF3SsLU=*.</span></span>
7. <span data-ttu-id="b1a54-123">Kies de knop **Verbinding** om door te gaan.</span><span class="sxs-lookup"><span data-stu-id="b1a54-123">Choose the **Connection** button to continue.</span></span> <span data-ttu-id="b1a54-124">Met PowerApps wordt een standaardgegevensset weergegeven voor [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b1a54-124">PowerApps will display a default dataset for [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b1a54-125">Kies de gegevensset **Standaard**.</span><span class="sxs-lookup"><span data-stu-id="b1a54-125">Choose the **Default** dataset.</span></span>

   <span data-ttu-id="b1a54-126">Met PowerApps wordt een lijst met tabellen weergegeven die beschikbaar zijn in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b1a54-126">PowerApps will display a list of tables that are available from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="b1a54-127">Met deze tabellen, of eindpunten, worden alle webservices vertegenwoordigd die u hebt gepubliceerd vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b1a54-127">These tables, or end points,  represent all the web services you have published from [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

   <span data-ttu-id="b1a54-128">U kunt ook een nieuwe webservice-URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] maken met behulp van de actie **Gegevensset maken** op de pagina **Webservices** met de begeleide instelling **Rapportage instellen** of door de actie **Bewerken in Excel** in de lijsten te kiezen.</span><span class="sxs-lookup"><span data-stu-id="b1a54-128">Alternatively, create a new web service URL in [!INCLUDE[d365fin](includes/d365fin_md.md)] by using the **Create Data Set** action in the **Web Services** page, using the **Set Up Reporting** Assisted Setup guide, or by choosing the **Edit in Excel** action in any lists.</span></span>
8. <span data-ttu-id="b1a54-129">Kies de tabel die u voor uw PowerApp wilt gebruiken en kies de knop **Verbinding maken**.</span><span class="sxs-lookup"><span data-stu-id="b1a54-129">Choose the table that you want to use for your PowerApp, and then choose the **Connect** button.</span></span>
9. <span data-ttu-id="b1a54-130">Herhaal de vorige stappen om aanvullende [!INCLUDE[d365fin](includes/d365fin_md.md)]-gegevens aan uw Power BI-gegevensmodel toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="b1a54-130">Repeat the previous steps to add additional [!INCLUDE[d365fin](includes/d365fin_md.md)] data to your Power BI data model.</span></span>

   > [!NOTE]  
>    <span data-ttu-id="b1a54-131">Zodra u verbinding hebt gemaakt met [!INCLUDE[d365fin](includes/d365fin_md.md)], wordt u niet weer gevraagd om de URL, gebruikersnaam of het wachtwoord van OData.</span><span class="sxs-lookup"><span data-stu-id="b1a54-131">Once you have successfully connected to [!INCLUDE[d365fin](includes/d365fin_md.md)], you will not be prompted again for the OData URL, username, or password.</span></span>

<span data-ttu-id="b1a54-132">Nu hebt u met succes een verbinding gemaakt met uw Business Central-gegevens en kunt u uw PowerApp gaan maken.</span><span class="sxs-lookup"><span data-stu-id="b1a54-132">At this point, you have successfully connected to your Business Central data and are ready to begin building your PowerApp.</span></span> <span data-ttu-id="b1a54-133">Zie de [PowerApps-documentatie](https://powerapps.microsoft.com/tutorials/getting-started/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b1a54-133">For more information, see the [PowerApps documentation](https://powerapps.microsoft.com/tutorials/getting-started/).</span></span>

## <a name="see-also"></a><span data-ttu-id="b1a54-134">Zie ook</span><span class="sxs-lookup"><span data-stu-id="b1a54-134">See Also</span></span>
<span data-ttu-id="b1a54-135">[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="b1a54-135">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
[<span data-ttu-id="b1a54-136">Bedrijfsgegevens importeren uit andere financiële systemen</span><span class="sxs-lookup"><span data-stu-id="b1a54-136">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
<span data-ttu-id="b1a54-137">[Instellen van [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="b1a54-137">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="b1a54-138">Financiën</span><span class="sxs-lookup"><span data-stu-id="b1a54-138">Finance</span></span>](finance.md)  
