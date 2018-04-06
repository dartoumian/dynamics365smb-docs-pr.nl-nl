---
title: 'Ontwerpdetails: Dimensiesetposten | Microsoft Docs'
description: Deze documentatie biedt gedetailleerd technisch inzicht in de concepten en principes die worden gebruikt om de opslag- en boekingsfunctie voor dimensieposten opnieuw te ontwerpen.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, dimensions, codeunit
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 66de44003ac66bad52a7b7e57d582659047bdbdf
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="design-details-dimension-set-entries"></a><span data-ttu-id="05e90-103">Ontwerpdetails: Dimensiesetposten</span><span class="sxs-lookup"><span data-stu-id="05e90-103">Design Details: Dimension Set Entries</span></span>
<span data-ttu-id="05e90-104">Deze documentatie biedt gedetailleerd technisch inzicht in de concepten en principes die worden gebruikt om de opslag- en boekingsfunctie voor dimensieposten in [!INCLUDE[d365fin](includes/d365fin_md.md)] opnieuw te ontwerpen.</span><span class="sxs-lookup"><span data-stu-id="05e90-104">This documentation provides detailed technical insight into the concepts and principles that are used to redesign the dimension entry storing and posting feature in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="05e90-105">In de documentatie wordt als eerste het conceptoverzicht van het nieuwe ontwerp beschreven.</span><span class="sxs-lookup"><span data-stu-id="05e90-105">The documentation starts by describing conceptual overviews of the redesign.</span></span> <span data-ttu-id="05e90-106">Vervolgens wordt de technische architectuur uitgelegd om te tonen hoe het nieuwe ontwerp wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="05e90-106">Then it explains the technical architecture to show how the redesign is made.</span></span> <span data-ttu-id="05e90-107">Ten slotte worden codevoorbeelden geleverd om u voor te bereiden op dimensiecodemigratie en -upgrade.</span><span class="sxs-lookup"><span data-stu-id="05e90-107">Finally, it provides code examples to prepare you for dimension code migration and upgrade.</span></span>  

## <a name="in-this-section"></a><span data-ttu-id="05e90-108">In dit gedeelte</span><span class="sxs-lookup"><span data-stu-id="05e90-108">In This Section</span></span>  
[<span data-ttu-id="05e90-109">Dimensiesetposten - overzicht</span><span class="sxs-lookup"><span data-stu-id="05e90-109">Dimension Set Entries Overview</span></span>](design-details-dimension-set-entries-overview.md)  
[<span data-ttu-id="05e90-110">Ontwerpdetails: Dimensiecombinaties zoeken</span><span class="sxs-lookup"><span data-stu-id="05e90-110">Design Details: Searching for Dimension Combinations</span></span>](design-details-searching-for-dimension-combinations.md)  
[<span data-ttu-id="05e90-111">Ontwerpdetails: Tabelstructuur</span><span class="sxs-lookup"><span data-stu-id="05e90-111">Design Details: Table Structure</span></span>](design-details-table-structure.md)  
[<span data-ttu-id="05e90-112">Ontwerpdetails: Codeunit 408 dimensiebeheer</span><span class="sxs-lookup"><span data-stu-id="05e90-112">Design Details: Codeunit 408 Dimension Management</span></span>](design-details-codeunit-408-dimension-management.md)  
[<span data-ttu-id="05e90-113">Ontwerpdetails: Codevoorbeelden van gewijzigde patronen in wijzigingen</span><span class="sxs-lookup"><span data-stu-id="05e90-113">Design Details: Code Examples of Changed Patterns in Modifications</span></span>](design-details-code-examples-of-changed-patterns-in-modifications.md)
