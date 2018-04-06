---
title: Gebruikersmachtigingen toewijzen of bewerken | Microsoft Docs
description: Hier wordt beschreven hoe u Office 365-gebruikers toevoegt aan Business Central en vervolgens machtigingen, toegangsrechten en beveiligingsinstellingen toewijst.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: access, right, security
ms.date: 03/08/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 602c429733104a792a49f4a7f38e2a3090420c9d
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="manage-users-and-permissions"></a><span data-ttu-id="635b7-103">Gebruikers en machtigingen beheren</span><span class="sxs-lookup"><span data-stu-id="635b7-103">Manage Users and Permissions</span></span>
<span data-ttu-id="635b7-104">Als u gebruikers wilt toevoegen in [!INCLUDE[d365fin](includes/d365fin_md.md)], moet de Office 365-beheerder van uw bedrijf eerst de gebruikers in het Office 365-beheercentrum maken.</span><span class="sxs-lookup"><span data-stu-id="635b7-104">To add users in [!INCLUDE[d365fin](includes/d365fin_md.md)], your company's Office 365 administrator must first create the users in the Office 365 Admin Center.</span></span> <span data-ttu-id="635b7-105">Zie voor meer informatie [Gebruikers aan Office 365 toevoegen voor bedrijven](https://support.office.com/en-us/article/Add-users-to-Office-365-for-business-435ccec3-09dd-4587-9ebd-2f3cad6bc2bc)</span><span class="sxs-lookup"><span data-stu-id="635b7-105">For more information, see [Add Users to Office 365 for business](https://support.office.com/en-us/article/Add-users-to-Office-365-for-business-435ccec3-09dd-4587-9ebd-2f3cad6bc2bc)</span></span>

<span data-ttu-id="635b7-106">Als gebruikers in Office 365 zijn gemaakt, kunnen ze worden geïmporteerd in het venster **Gebruikers** door middel van de actie **Gebruikers ophalen uit Office 365**.</span><span class="sxs-lookup"><span data-stu-id="635b7-106">Once users are created in Office 365, they can be imported into the **Users** window by using the **Get Users from Office 365** action.</span></span> <span data-ttu-id="635b7-107">Aan gebruikers worden machtigingensets toegewezen op basis van het plan dat aan de gebruiker is toegewezen in Office 365.</span><span class="sxs-lookup"><span data-stu-id="635b7-107">Users are assigned permission sets depending on the plan assigned to the User in Office 365.</span></span>

<span data-ttu-id="635b7-108">U kunt vervolgens machtigingensets aan gebruikers toewijzen om te bepalen tot welke databaseobjecten (en daardoor tot welke UI-elementen) zij toegang hebben en in welke bedrijven.</span><span class="sxs-lookup"><span data-stu-id="635b7-108">You can then proceed to assign permission sets to the users to define which database objects, and thereby which UI elements, they have access to, and in which companies.</span></span> <span data-ttu-id="635b7-109">U kunt gebruikers toevoegen aan gebruikersgroepen.</span><span class="sxs-lookup"><span data-stu-id="635b7-109">You can add users to user groups.</span></span> <span data-ttu-id="635b7-110">Hierdoor wordt het gemakkelijker om dezelfde machtigingensets aan meerdere gebruikers toe te wijzen.</span><span class="sxs-lookup"><span data-stu-id="635b7-110">This makes it easier to assign the same permission sets to multiple users.</span></span>

<span data-ttu-id="635b7-111">Een machtigingenset is een verzameling machtigingen voor bepaalde objecten in de database.</span><span class="sxs-lookup"><span data-stu-id="635b7-111">A permission set is a collection of permissions for specific objects in the database.</span></span> <span data-ttu-id="635b7-112">Aan alle gebruikers moeten een of meer machtigingensets worden toegewezen voordat ze toegang hebben tot [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="635b7-112">All users must be assigned one or more permission sets before they can access [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="635b7-113">Er zijn standaard verschillende vooraf gedefinieerde machtigingensets beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="635b7-113">A number of predefined permission sets are provided by default.</span></span> <span data-ttu-id="635b7-114">U kunt de machtigingensets gebruiken zoals deze zijn gedefinieerd, u kunt de sets aanpassen of u kunt uw eigen machtigingensets maken.</span><span class="sxs-lookup"><span data-stu-id="635b7-114">You can use these permission sets as already defined, modify the default permission sets, or create additional permission sets.</span></span>

<span data-ttu-id="635b7-115">Beheerders kunnen het venster **Gebruikersinstellingen** gebruiken om perioden te definiëren waarin opgegeven gebruikers kunnen boeken en ook kunnen opgeven of het systeem de tijdsduur vastlegt gedurende welke gebruikers zijn aangemeld.</span><span class="sxs-lookup"><span data-stu-id="635b7-115">Administrators can use the **User Setup** window to define periods of time during which specified users are able to post, and also specify if the system logs the amount of time users are logged on.</span></span>

## <a name="to-assign-permissions-to-a-user"></a><span data-ttu-id="635b7-116">Machtigingen toewijzen aan een gebruiker</span><span class="sxs-lookup"><span data-stu-id="635b7-116">To assign permissions to a user</span></span>
1. <span data-ttu-id="635b7-117">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Gebruikers** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="635b7-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Users**, and then choose the related link.</span></span>
2. <span data-ttu-id="635b7-118">Selecteer de gebruiker waaraan u machtigingen wilt toewijzen.</span><span class="sxs-lookup"><span data-stu-id="635b7-118">Select the user that you want to assign permission to.</span></span>
<span data-ttu-id="635b7-119">Alle machtigingensets die al zijn toegewezen aan de gebruiker worden weergegeven in het feitenblok **Machtigingensets**.</span><span class="sxs-lookup"><span data-stu-id="635b7-119">Any permission sets that are already assigned to the user are displayed in the **Permission Sets** FactBox.</span></span>
3. <span data-ttu-id="635b7-120">Kies de actie **Bewerken** om het venster **Gebruikerskaart** te openen.</span><span class="sxs-lookup"><span data-stu-id="635b7-120">Choose the **Edit** action to open the **User Card** window.</span></span>
4. <span data-ttu-id="635b7-121">Vul op het sneltabblad **Gebruikersmachtigingensets** waar nodig de velden in op een nieuwe regel.</span><span class="sxs-lookup"><span data-stu-id="635b7-121">On the **User Permission Sets** FastTab, on a new line, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-group-users-in-user-groups"></a><span data-ttu-id="635b7-122">Gebruikers in gebruikersgroepen samenvoegen</span><span class="sxs-lookup"><span data-stu-id="635b7-122">To group users in user groups</span></span>
<span data-ttu-id="635b7-123">U kunt gebruikersgroepen instellen om u te helpen machtigingensets te beheren voor groepen gebruikers in uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="635b7-123">You can set up users groups to help you manage permission sets for groups of users in your company.</span></span> <span data-ttu-id="635b7-124">U kunt een functie gebruiken om alle machtigingensets van een bestaande gebruikersgroep naar de nieuwe gebruikersgroep te kopiëren.</span><span class="sxs-lookup"><span data-stu-id="635b7-124">You can use a function to copy all permission sets from an existing user group to your new user group.</span></span> <span data-ttu-id="635b7-125">De leden van de gebruikersgroep worden niet gekopieerd.</span><span class="sxs-lookup"><span data-stu-id="635b7-125">User group members are not copied.</span></span>

1. <span data-ttu-id="635b7-126">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Gebruikersgroepen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="635b7-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="635b7-127">U kunt ook in het venster **Gebruikers** de actie **Gebruikersgroepen** kiezen.</span><span class="sxs-lookup"><span data-stu-id="635b7-127">Alternatively, in the **Users** window, choose the **User Groups** action.</span></span>
3. <span data-ttu-id="635b7-128">Kies in het venster **Gebruikersgroep** de actie **Gebruikersgroepsleden**.</span><span class="sxs-lookup"><span data-stu-id="635b7-128">In the **User Group** window, choose the **User Group Members** action.</span></span>
6. <span data-ttu-id="635b7-129">Kies in het venster **Gebruikersgroepsleden** de actie **Gebruikers toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="635b7-129">In the **User Group Members** window, choose the **Add Users** action.</span></span>
7. <span data-ttu-id="635b7-130">Als u nieuwe of extra machtigingensets wilt toevoegen, kiest u in het venster **Gebruikersgroepen** de actie **Machtigingensets van gebruikersgroep**.</span><span class="sxs-lookup"><span data-stu-id="635b7-130">To add new or additional permission sets, in the **User Groups** window, choose the **User Group Permission Sets** action.</span></span>
8. <span data-ttu-id="635b7-131">Vul in het venster **Machtigingensets van gebruikersgroep** op een nieuwe regel de velden waar nodig in door bestaande machtigingensets te selecteren.</span><span class="sxs-lookup"><span data-stu-id="635b7-131">In the **User Group Permission Sets** window, on a new line, fill in the fields as necessary by selecting from existing permission sets.</span></span>

## <a name="to-set-up-user-time-constraints"></a><span data-ttu-id="635b7-132">Tijdsbeperkingen voor gebruikers instellen</span><span class="sxs-lookup"><span data-stu-id="635b7-132">To set up user time constraints</span></span>
<span data-ttu-id="635b7-133">Beheerders kunnen perioden definiëren waarin opgegeven gebruikers kunnen boeken en ook kunnen opgeven of het systeem de tijdsduur vastlegt gedurende welke gebruikers zijn aangemeld.</span><span class="sxs-lookup"><span data-stu-id="635b7-133">Administrators can define periods of time during which specified users are able to post, and also specify if the system logs the amount of time users are logged on.</span></span> <span data-ttu-id="635b7-134">Beheerders kunnen ook divisies toewijzen aan gebruikers.</span><span class="sxs-lookup"><span data-stu-id="635b7-134">Administrators can also assign responsibility centers to users.</span></span> <span data-ttu-id="635b7-135">Zie [Werken met divisies](inventory-responsibility-centers.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="635b7-135">For more information, see [Work with Responsibility Centers](inventory-responsibility-centers.md).</span></span>

1. <span data-ttu-id="635b7-136">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Gebruikersinstellingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="635b7-136">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **User Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="635b7-137">Kies in het venster **Gebruikersinstellingen** dat wordt geopend, de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="635b7-137">In the **User Setup** window opens, choose the **New** action.</span></span>
3. <span data-ttu-id="635b7-138">Voer in het veld **Gebruikers-id** de id van een gebruiker in of kies het veld om alle huidige Windows-gebruikers in het systeem te zien.</span><span class="sxs-lookup"><span data-stu-id="635b7-138">In the **User ID** field, enter the ID of a user, or choose the field to see all current Windows users in the system.</span></span>
4. <span data-ttu-id="635b7-139">Vul de velden in.</span><span class="sxs-lookup"><span data-stu-id="635b7-139">Fill in the fields as necessary.</span></span>

## <a name="see-also"></a><span data-ttu-id="635b7-140">Zie ook</span><span class="sxs-lookup"><span data-stu-id="635b7-140">See Also</span></span>
[<span data-ttu-id="635b7-141">Voorbereid zijn om zaken te doen</span><span class="sxs-lookup"><span data-stu-id="635b7-141">Getting Ready for Doing Business</span></span>](ui-get-ready-business.md)  
<span data-ttu-id="635b7-142">[Installatie en beheer in [!INCLUDE[d365fin](includes/d365fin_md.md)]](admin-setup-and-administration.md)</span><span class="sxs-lookup"><span data-stu-id="635b7-142">[Setup and Administration in [!INCLUDE[d365fin](includes/d365fin_md.md)]](admin-setup-and-administration.md)</span></span>  
<span data-ttu-id="635b7-143">[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="635b7-143">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
<span data-ttu-id="635b7-144">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="635b7-144">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
