---
title: Artikelen blokkeren vanuit Verkoop of Inkoop
description: In Business Central kan een artikel worden gemarkeerd als geblokkeerd voor verkoop, geblokkeerd voor inkoop of geblokkeerd voor alle doeleinden.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 12/04/2019
ms.author: sgroespe
ms.openlocfilehash: 0218cf1b4982b9e8c5b5c2817590bc5ebd8f1941
ms.sourcegitcommit: b6e506a45a1cd632294bafa1c959746cc3a144f6
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/06/2019
ms.locfileid: "2896058"
---
# <a name="block-items-from-sales-or-purchasing"></a>Artikelen blokkeren vanuit Verkoop of Inkoop
U kunt voorkomen dat een artikel wordt ingevoerd op verkoop- of inkoopregels en u kunt voorkomen dat het wordt geboekt in een transactie.  

De volgende tabel laat zien wat er gebeurt wanneer artikelen worden geblokkeerd.  

|Optie|Description|  
|--------------------|------------|  
|**Verkoop geblokkeerd**|U kunt het artikel niet invoeren in een verkoopdocument of een verkoopartikeldagboek.|  
|**Inkoop geblokkeerd**|U kunt het artikel niet invoeren in een inkoopdocument, in een inkoopartikeldagboek of in planningsprocessen voor inkoop.|  
|**Geblokkeerd**|U kunt het artikel niet voor een artikeltransactie gebruiken.|  

> [!NOTE]
> Geblokkeerde artikelen kunnen worden geretourneerd. Dit betekent dat geen van de bovenstaande instellingen van toepassing zijn als het artikel wordt gebruikt in retourorders en creditnota's.

Wanneer u de functie **Document kopiëren** gebruikt om nieuwe documenten te maken op basis van bestaande documenten, ontvangt u een bericht als er items op de brondocumentregels zijn geblokkeerd. De geblokkeerde documentregels worden uitgesloten van het nieuwe document en een bericht toont een overzicht van alle documentregels die in het brondocument zijn geblokkeerd.

## <a name="to-block-an-item-from-being-entered-on-sales-lines"></a>Voorkomen dat een artikel wordt ingevoerd op verkoopregels  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Artikelen** in en kies de gerelateerde koppeling.  
2.  Selecteer het artikel dat u wilt blokkeren en schakel vervolgens het selectievakje **Verkoop geblokkeerd** in.  

Wanneer u probeert het artikel in te voeren in een verkoopdocument of -dagboekregel, wordt nu een foutbericht weergegeven dat aangeeft dat het artikel is geblokkeerd.

## <a name="to-block-an-item-from-being-entered-on-purchase-lines"></a>Voorkomen dat een artikel wordt ingevoerd op inkoopregels  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Artikelen** in en kies de gerelateerde koppeling.  
2.  Selecteer het artikel dat u wilt blokkeren en schakel vervolgens het selectievakje **Inkoop geblokkeerd** in.  

Wanneer u probeert het artikel in te voeren in een inkoopdocument of -dagboekregel, wordt nu een foutbericht weergegeven dat aangeeft dat het artikel is geblokkeerd.

## <a name="to-block-an-item-from-being-posted"></a>Voorkomen dat een artikel wordt geboekt
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Artikelen** in en kies de gerelateerde koppeling.
2. Selecteer het artikel dat u wilt blokkeren en schakel vervolgens het selectievakje **Geblokkeerd** in.

Wanneer u probeert een transactie van welke aard dan ook te boeken voor het artikel, krijgt u nu een foutbericht dat het artikel is geblokkeerd.

## <a name="see-also"></a>Zie ook  
[Nieuwe artikelen registreren](inventory-how-register-new-items.md)  
[Voorraad](inventory-manage-inventory.md)  
