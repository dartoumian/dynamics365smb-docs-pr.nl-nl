---
title: Outputboeking tegenboeken | Microsoft Docs
description: Het kan voorkomen dat een outputboeking moet worden tegengeboekt. Dit is bijvoorbeeld het geval als er een gegevensinvoerfout is gemaakt en er een onjuiste hoeveelheid output is geboekt op een productieorder.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 2cdda8a01d6391f97bfae5600ce35d2ab989ae54
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2877838"
---
# <a name="reverse-output-posting"></a>Outputboeking tegenboeken
Het kan voorkomen dat een outputboeking moet worden tegengeboekt. Dit is bijvoorbeeld het geval als er een gegevensinvoerfout is gemaakt en er een onjuiste hoeveelheid output is geboekt op een productieorder.  

## <a name="to-reverse-an-output-posting"></a>Een outputboeking tegenboeken  
1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Outputdagboek** in en kies de desbetreffende koppeling. Selecteer uw batch.  
2. Vul de benodigde velden in. Zie voor meer informatie [Output en bewerkingstijd in batches boeken](production-how-to-post-output-quantity.md).
3.  Selecteer in het veld **Vereffenen met post** de bijbehorende artikelpost. Hiermee voert u een tegenboeking uit van de capaciteit en artikelposten.  
4. Boek de tegenboeking door het dagboek te boeken.  

De posten van het outputdagboek worden als positieve herwaardering geboekt op de artikelposten.  

## <a name="see-also"></a>Zie ook  
 [Productie](production-manage-manufacturing.md)    
 [Productie instellen](production-configure-production-processes.md)  
 [Gepland](production-planning.md)      
 [Voorraad](inventory-manage-inventory.md)  
 [Inkoop](purchasing-manage-purchasing.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
