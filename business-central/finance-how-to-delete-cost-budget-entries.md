---
title: 'Procedure: kostenbudgetposten verwijderen | Microsoft Docs'
description: Door middel van de batchtaak Kostenbudgetposten verwijderen annuleert u kostenbegrotingsposten uit het kostenbudgetregister.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 04510e87789e6d69b33009be7ebbaf7a405d0dff
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2882688"
---
# <a name="delete-cost-budget-entries"></a>Kostenbudgetposten verwijderen
Door middel van de batchtaak **Kostenbudgetposten verwijderen** annuleert u kostenbegrotingsposten uit het kostenbudgetregister.  

Om hiaten in de kostenbudgetposten en kostenregisterposten te voorkomen, kunt u één enkele post of een reeks posten middenin een lijst met registerposten niet verwijderen.  

### <a name="to-delete-a-cost-budget-entry"></a>Kostenbudgetposten verwijderen  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Kostenbudgetposten verwijderen** in en kies de desbetreffende koppeling.  

    Het veld **Naar journaalnr.** bevat het nummer van de laatste journaalpost en kan niet worden gewijzigd.  

    U kunt het veld **Van journaalnr.** gebruiken om een nummer voor een journaalpost te selecteren waar de verwijdering moet beginnen.  
2.  Kies de knop **OK** om de geselecteerde kostenbegrotingsposten te verwijderen.  

> [!NOTE]  
>  Om te voorkomen dat kostenbegrotingsposten onbedoeld worden verwijderd, kunt u journaalposten sluiten door de regels als **gesloten** te markeren in het veld **Gesloten** op de pagina **Kostenbudgetregisters**.  

## <a name="see-also"></a>Zie ook  
[Kosten verantwoorden](finance-manage-cost-accounting.md)
[Kostenbudgetten maken](finance-create-cost-budgets.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
