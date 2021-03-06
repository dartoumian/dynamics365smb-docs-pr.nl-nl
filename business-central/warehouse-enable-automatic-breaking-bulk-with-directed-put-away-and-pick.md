---
title: Automatisch splitsen van bulkgoederen met gestuurde opslag en pick | Microsoft Docs
description: Voor locaties die gebruikmaken van gestuurde opslag en pick, kunt u eenheden opsplitsen in kleinere eenheden wanneer er magazijninstructies worden gemaakt die voldoen aan de eisen met betrekking tot brondocumenten, -productieorders of interne picks en opslag.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 668837945a850552821d435f56c6374982cc6c8f
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2876844"
---
# <a name="enable-automatic-breaking-bulk-with-directed-put-away-and-pick"></a>Automatisch splitsen van bulkgoederen met gestuurde opslag en pick inschakelen
Voor locaties die gebruikmaken van gestuurde opslag en pick, kan [!INCLUDE[d365fin](includes/d365fin_md.md)] in allerlei situaties, bulkgoederen automatisch splitsen (dit houdt in dat een bepaalde eenheid wordt opgesplitst in kleinere eenheden) wanneer er magazijninstructies worden gemaakt die voldoen aan de eisen met betrekking tot brondocumenten, -productieorders of interne picks en opslag. Bulksplitsing betekent soms ook het verzamelen van kleinere eenheden, indien nodig, om te voldoen aan uitgaande verzoeken door de grotere eenheid op het brondocument of de productieorder te splitsen in kleinere eenheden die in het magazijn beschikbaar zijn.   

## <a name="breakbulking-in-picks"></a>Bulksplitsing in picks  
Als u artikelen wilt opslaan in een aantal verschillende eenheden en deze, zo nodig automatisch wilt laten combineren tijdens het pickproces, selecteert u het veld **Breakbulk toestaan** op de vestigingskaart.  

Voor de uitvoering van een taak zoekt de toepassing automatisch naar een artikel in dezelfde maateenheid. Als deze vorm van het artikel echter niet wordt gevonden en dit veld is geselecteerd, wordt u gevraagd een bepaalde maateenheid op te splitsen in de vereiste maateenheid.  

Als het systeem alleen kleinere eenheden kan vinden, wordt u gevraagd artikelen te verzamelen om aan de hoeveelheid op de verzending of productieorder te kunnen voldoen. In de praktijk wordt de grotere eenheid op het brondocument opgesplitst in kleinere pickeenheden.  

## <a name="breakbulking-in-put-aways"></a>Bulksplitsing in opslag  
Bij de magazijnopslag stelt de toepassing automatisch Plaatsen-actieregels voor in de opslageenheid, bijvoorbeeld stuks, hoewel de artikelen in een andere eenheid arriveren.  

## <a name="breakbulking-in-movements"></a>Bulksplitsing in verplaatsingen  
De toepassing past ook automatisch bulksplitsing toe op aanvullingsverplaatsingen, als u het veld **Breakbulk toestaan** op het sneltabblad **Optie** van de pagina **Opslagloc.-aanvulling** is ingeschakeld.  

U kunt de resultaten van de omzetting van de ene eenheid in de andere weergeven als tussenliggende bulksplitsingsregels in de opslag-, pick- of verplaatsingsinstructies.  

> [!NOTE]  
>  Als u het veld **Breakbulkfilter plaatsen** in de kop van de magazijninstructie selecteert, worden de bulksplitsingsregels verborgen wanneer de grotere eenheid volledig wordt gebruikt. Bijvoorbeeld: als een pallet 12 stuks bevat en u alle 12 stuks gaat gebruiken, wordt u gevraagd 1 pallet te nemen en 12 stuks te plaatsen. Als u echter maar 9 stuks nodig hebt, worden de opsplitsingsregels niet verborgen, zelfs niet als u het veld **Breakbulkfilter** hebt geselecteerd omdat u de resterende drie stuks ergens in het magazijn moet plaatsen.  

> [!NOTE]  
>  Als u wilt dat uw eenheden optimaal presteren in het magazijn, ook in verband met de bulksplitsingsfunctionaliteit, moet u waar mogelijk proberen om:  
>   
> - De basiseenheid voor een artikel in te stellen als de kleinste eenheid die u denkt nodig te hebben in de magazijnprocessen.  
> - Alternatieve eenheden voor het artikel instellen als veelvouden van de basiseenheid.  

## <a name="see-also"></a>Zie ook  
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
