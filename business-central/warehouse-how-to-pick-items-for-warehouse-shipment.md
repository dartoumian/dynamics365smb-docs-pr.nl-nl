---
title: Artikelen picken voor magazijnverzending | Microsoft Docs
description: Als voor de locatie zowel magazijnpickverwerking als magazijnverzendingsverwerking is vereist, gebruikt u magazijnpickdocumenten om de pickinformatie te beheren voordat u de magazijnverzending boekt.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: d35c6dec3eee09ec72a09325dcc527c18dc9b8c4
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2876676"
---
# <a name="pick-items-for-warehouse-shipment"></a>Picken van artikelen voor magazijnverzending
Als voor de locatie zowel magazijnpickverwerking als magazijnverzendingsverwerking is vereist, gebruikt u magazijnpickdocumenten om de pickinformatie te beheren voordat u de magazijnverzending boekt.  

Een magazijn-pickdocument kan niet van het begin af gemaakt worden, omdat een pick-activiteit altijd onderdeel is van een werkstroom, zowel bij een pull- als bij een push-scenario.  

U kunt magazijn-pickdocumenten op een pull-manier maken door het openen van een leeg document voor magazijnverzending, detecteren van brondocumenten die zijn vrijgegeven voor verzending en vervolgens maken van magazijnpickregels voor deze verzendingen. U kunt de functies **Brondocumenten ophalen** of **Filter gebruiken om brondocumenten op te halen** voor het detecteren van brondocumenten die gereed zijn voor verzending.

U kunt ook de pagina **Werkblad Pick** gebruiken om pickregels in de batchmodus te halen en te maken. Zie [Picks plannen in voorstellen](warehouse-how-to-plan-picks-in-worksheets.md) voor meer informatie.  

U kunt ook magazijn-pickdocumenten op push-wijze vanuit de pagina **Magazijnverzending** maken door **Pick maken** te selecteren.  

> [!NOTE]  
>  Het picken voor magazijnverzending van artikelen die worden samengesteld voor de verkooporder die wordt verzonden volgt dezelfde stappen als gewone magazijnpicks voor verzending, zoals beschreven in dit onderwerp. Het aantal pickregels per te verzenden aantal is mogelijk echter veel-op-één omdat u de componenten pickt, niet het assemblageartikel.  
>   
>  De magazijnpickregels zijn gemaakt voor de waarde in het veld **Resterend aantal** op de regels van de assemblage die is gekoppeld aan de verkooporderregel die wordt verzonden. Dit zorgt ervoor dat alle onderdelen in één actie worden gepickt.  
>   
>  Zie de sectie Op-order-assembleren-artikelen in magazijnverzendingen afhandelen voor meer informatie.  
>   
>  Zie [Picken voor productie of assemblage](warehouse-how-to-pick-for-production.md) voor informatie over het picken van onderdelen voor assemblageorders in het algemeen, met inbegrip van situaties waar de assemblage niet voor een verkoopverzending is.  

## <a name="to-pick-items-for-warehouse-shipment"></a>Picken van artikelen voor magazijnverzending  
1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Magazijnpicks** in en kies de desbetreffende koppeling.  

    Als u een bepaalde pick wilt bewerken, selecteert u het pickformulier of het overzicht. U kunt het overzicht ook filteren op picks die speciaal aan u zijn toegewezen. De pickkaart openen.  
2.  Indien het veld **Toegewezen gebruikers-ID** leeg is, voert u uw ID in om uzelf te identificeren indien nodig.  
3.  Uitvoeren van het werkelijke picken van artikelen.  

    Indien het magazijn opslaglocaties gebruikt, worden de standaard opslaglocaties voor de artikelen voorgesteld om de artikelen uit te halen. De instructies worden op twee afzonderlijke regels weergegeven, minimaal één voor elk soort actie, Nemen en Plaatsen.  

    Indien voor het magazijn gestuurde opslag en pick is ingesteld, wordt de opslaglocatievolgorde gebruikt voor het berekenen van de beste opslaglocaties waaruit gepickt kan worden en deze opslaglocaties worden vervolgens voorgesteld op de pickregels. De instructies worden op twee afzonderlijke regels weergegeven, minimaal één voor elk soort actie, Nemen en Plaatsen.  

4.  Als u de pick hebt uitgevoerd en de artikelen op de verzendlocatie hebt geplaatst, kiest u de actie **Pick registreren**.  

De persoon die verantwoordelijk is voor verzending kan nu de artikelen naar de afdeling voor verzending overbrengen en de verzending boeken, inclusief het verwante brondocument, op de pagina **Mag. -verzending**. Zie [Artikelen verzenden](warehouse-how-ship-items.md) voor meer informatie.   

Naast het picken voor brondocumenten zoals beschreven in dit onderwerp kunt u artikelen tussen opslaglocaties nemen en plaatsen zonder te verwijzen naar de brondocumenten. Zie voor meer informatie [Picken en opslaan zonder een brondocument](warehouse-how-to-create-put-aways-from-internal-put-aways.md).  

## <a name="handling-assemble-to-order-items-in-warehouse-shipments"></a>Op-order-assembleren-artikelen in magazijnverzendingen afhandelen
In scenario's voor het assembleren op order, wordt het veld **Te verzenden aantal** op magazijnverzendingsregels gebruikt om vast te leggen hoeveel eenheden worden geassembleerd. Het opgegeven aantal wordt vervolgens geboekt als assemblageuitvoer wanneer de magazijnverzending wordt geboekt.

Voor andere magazijnverzendingsregels is de waarde in het veld **Te verzenden aantal** nul vanaf het begin.

Wanneer werknemers die verantwoordelijk zijn voor het assembleren klaar zijn met het assembleren van onderdelen of de volledige hoeveelheid voor op order assembleren, registreren ze dit in het veld **Te verzenden aantal** op de magazijnverzendingsregel en kiezen ze de actie **Verzending boeken**. Het resultaat is dat de bijbehorende assemblageuitvoer wordt geboekt, inclusief het materiaalverbruik. Een verkoopverzending voor de hoeveelheid wordt geboekt voor de verkooporder.

Op de assemblageorder kunt u **Magazijnverzendregel op order assembleren** om toegang te krijgen tot de magazijnverzendregel. Dit is handig voor werknemers die gewoonlijk niet de pagina **Magazijnverzending** gebruiken.

Na het boeken van de magazijnverzending, worden verschillende velden op de orderregel bijgewerkt om de voortgang in het magazijn weer te geven. De volgende velden worden ook bijgewerkt om weer te geven hoeveel op-order-assembleren-aantallen nog moeten worden geassembleerd en verzonden:

- **AoO-mag. uitstaand aantal**
- **AoO-mag. uitst. aant. (basis)**

> [!NOTE]
> In combinatiescenario's waarbij een deel van de hoeveelheid eerst moet worden geassembleerd en een ander deel uit voorraad moet worden verzonden, worden twee magazijnverzendregels gemaakt. Eén voor het op-order-assembleren-aantal, en één voor het voorraadaantal.

> In dat geval wordt het op-order-assembleren-aantal verwerkt zoals beschreven in dit onderwerp, en het voorraadaantal wordt verwerkt als een gewone magazijnverzendregel. Zie voor meer informatie over combinatiescenario's [Op voorraad assembleren of Op order assembleren begrijpen](assembly-assemble-to-order-or-assemble-to-stock.md).

## <a name="see-also"></a>Zie ook  
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
