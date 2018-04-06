---
title: Artikelen categoriseren| Microsoft Docs
description: Om u te helpen zoeken naar artikelen kunt u artikelkenmerken toewijzen en artikelen categoriseren.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: category, search, attribute, facet
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f7f40054c511b5f3bf1d61dc40d6107cc717dcd8
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="categorize-items"></a><span data-ttu-id="bcfff-103">Artikelen categoriseren</span><span class="sxs-lookup"><span data-stu-id="bcfff-103">Categorize Items</span></span>
<span data-ttu-id="bcfff-104">Om een overzicht van uw artikelen bij te houden en u te helpen artikelen te sorteren en zoeken, is het handig om uw artikelen in artikelcategorieën te organiseren.</span><span class="sxs-lookup"><span data-stu-id="bcfff-104">To maintain an overview of your items and to help you sort and find items, it is useful to organize your items in item categories.</span></span>

<span data-ttu-id="bcfff-105">Als u artikelen op basis van kenmerken wilt zoeken, kunt u artikelkenmerken aan artikelen en ook aan artikelcategorieën toewijzen.</span><span class="sxs-lookup"><span data-stu-id="bcfff-105">To find items by characteristics, you can assign item attributes to items and also to item categories.</span></span> <span data-ttu-id="bcfff-106">Zie [Werken met artikelkenmerken](inventory-how-work-item-attributes.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="bcfff-106">For more information, see [Work with Item Attributes](inventory-how-work-item-attributes.md).</span></span>

## <a name="to-create-an-item-category"></a><span data-ttu-id="bcfff-107">Een artikelcategorie maken</span><span class="sxs-lookup"><span data-stu-id="bcfff-107">To create an item category</span></span>
1. <span data-ttu-id="bcfff-108">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelcategorieën** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="bcfff-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Categories**, and then choose the related link.</span></span>
2. <span data-ttu-id="bcfff-109">Kies in het venster **Artikelcategorieën** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="bcfff-109">In the **Item Categories** window, choose the **New** action.</span></span>
3. <span data-ttu-id="bcfff-110">Vul indien nodig de velden in het venster **Artikelcategoriekaart** op het sneltabblad **Algemeen** in:</span><span class="sxs-lookup"><span data-stu-id="bcfff-110">In the **Item Category Card** window, on the **General** FastTab, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="bcfff-111">Geef op het sneltabblad **Kenmerken** alle artikelkenmerken voor de artikelcategorie op.</span><span class="sxs-lookup"><span data-stu-id="bcfff-111">On the **Attributes** FastTab, specify any item attributes for the item category.</span></span> <span data-ttu-id="bcfff-112">Zie het gedeelte 'Artikelkenmerken aan een artikelcategorie toewijzen' in [Werken met artikelkenmerken](inventory-how-work-item-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="bcfff-112">For more information, see the "To assign item attributes to an item category" section in [Work with Item Attributes](inventory-how-work-item-attributes.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="bcfff-113">Als de artikelcategorie een bovenliggende artikelcategorie heeft, zoals aangegeven door het veld **Bovenliggende categorie**, worden alle artikelkenmerken die aan die bovenliggende artikelcategorie zijn toegewezen, vooraf ingevuld op het sneltabblad **Kenmerken**.</span><span class="sxs-lookup"><span data-stu-id="bcfff-113">If the item category has a parent item category, as indicated by the **Parent Category** field, then any item attributes that are assigned to that parent item category are prefilled on the **Attributes** FastTab.</span></span>

> [!NOTE]  
>   <span data-ttu-id="bcfff-114">Opmerking: artikelkenmerken die u aan een artikelcategorie toewijst, worden automatisch toegepast op het artikel waaraan de artikelcategorie is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="bcfff-114">Item attributes that you assign to an item category will automatically apply to the item that the item category is assigned to.</span></span>

## <a name="to-assign-an-item-category-to-an-item"></a><span data-ttu-id="bcfff-115">Een artikelcategorie aan een artikel toewijzen</span><span class="sxs-lookup"><span data-stu-id="bcfff-115">To assign an item category to an item</span></span>
1. <span data-ttu-id="bcfff-116">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="bcfff-116">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="bcfff-117">Open de kaart voor het artikel dat u aan een artikelcategorie wilt toewijzen.</span><span class="sxs-lookup"><span data-stu-id="bcfff-117">Open the card for the item that you want to assign to an item category.</span></span>
3. <span data-ttu-id="bcfff-118">Kies in het veld **Artikelcategoriecode** de zoekknop en selecteer een bestaande artikelcategorie.</span><span class="sxs-lookup"><span data-stu-id="bcfff-118">Choose the lookup button in the **Item Category Code** field and select an existing item category.</span></span> <span data-ttu-id="bcfff-119">U kunt ook de actie **Nieuw** kiezen om eerst een nieuwe artikelcategorie te maken, zoals is uitgelegd in het gedeelte "Een artikelcategorie maken".</span><span class="sxs-lookup"><span data-stu-id="bcfff-119">Alternatively, choose the **New** action to first create a new item category as explained in the "To create an item category" section.</span></span>

## <a name="see-also"></a><span data-ttu-id="bcfff-120">Zie ook</span><span class="sxs-lookup"><span data-stu-id="bcfff-120">See Also</span></span>
[<span data-ttu-id="bcfff-121">Werken met artikelkenmerken</span><span class="sxs-lookup"><span data-stu-id="bcfff-121">Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)  
[<span data-ttu-id="bcfff-122">Nieuwe artikelen registreren</span><span class="sxs-lookup"><span data-stu-id="bcfff-122">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="bcfff-123">Voorraad</span><span class="sxs-lookup"><span data-stu-id="bcfff-123">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="bcfff-124">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="bcfff-124">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
