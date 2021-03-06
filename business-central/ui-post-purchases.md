---
title: Begrijpen hoe u inkoopdocumenten boekt | Microsoft Docs
description: Meer informatie over de verschillende boekingsfuncties om inkoopdocumenten te boeken en hoe u geboekte documenten kunt bijwerken.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 01/17/2020
ms.author: sgroespe
ms.openlocfilehash: 2565133adfab4fb5f6febeeccb69c4f3d6f59e71
ms.sourcegitcommit: 877af26e3e4522ee234fbba606615e105ef3e90a
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2020
ms.locfileid: "2991877"
---
# <a name="posting-purchases"></a>Inkopen boeken
In de **Boekingsgroep** op een inkoopdocument kunt u kiezen uit de volgende boekingsfuncties:

* **Boeken**
* **Voorbeeld van boeking weergeven**
* **Boeken en afdrukken**
* **Testrapport**
* **Batchboeken**

Wanneer u alle regels hebt ingevuld en alle informatie hebt ingevoerd op de inkooporder, kunt u de order boeken. Dit houdt in dat u een ontvangst en een factuur maakt.

Wanneer een inkooporder wordt geboekt, worden de rekening van de leverancier, het grootboek en de artikelposten bijgewerkt.

Voor elke inkooporder wordt een inkooppost gemaakt in de tabel **Grootboekpost**. Ook wordt een post in de leveranciersrekening in de tabel **Leverancierspost** gemaakt en wordt er een grootboekpost in de betreffende schuldenrekening gemaakt. Bovendien kan het boeken van de order resulteren in een btw-post en een grootboekpost voor de totale korting. Of er een post voor de korting wordt geboekt, wordt bepaald door de inhoud van het veld **Korting boeken** op de pagina **Inkoopinstellingen**.

Voor elke inkooporderregel wordt een artikelpost gemaakt in de tabel **Artikelpost** (als op de inkoopregels artikelnummers staan) of een grootboekpost in de tabel **Grootboekpost** (als op de inkoopregels een grootboekrekening staat). Daarnaast worden inkooporders altijd vastgelegd in de tabellen **Inkoopontvangst** en **Inkoopfactuur**.

Voordat u gaat boeken, kunt u een controlelijst afdrukken met alle informatie uit de inkooporder en eventuele fouten die erin voorkomen. Kies **Boeken** en vervolgens **Testrapport** als u het rapport wilt afdrukken.

> [!IMPORTANT]  
>   Tijdens het boeken van een order kunt u zowel een ontvangst als een factuur maken. Deze kunt u tegelijkertijd, maar ook onafhankelijk van elkaar maken. U kunt ook een gedeeltelijke ontvangst en een gedeeltelijke factuur maken door de velden **Te ontvangen aantal** en **Te factureren aantal** op de afzonderlijke inkooporderregels in te vullen voordat u de boeking uitvoert. U kunt geen factuur maken voor iets dat niet is ontvangen. Dit betekent dat u pas kunt factureren als er een ontvangst is vastgelegd, of u moet tegelijkertijd ontvangen en factureren.

U kunt de optie Boeken of Boeken en afdrukken kiezen. Als u ervoor kiest om te boeken en af te drukken, wordt een lijst afgedrukt nadat de order is geboekt. U kunt ook de functie **Batchboeken** kiezen, waarmee u verschillende orders tegelijkertijd kunt boeken. Zie voor meer informatie [Meerdere documenten tegelijkertijd boeken](ui-batch-posting.md).

## <a name="viewing-ledger-entries"></a>Posten bekijken
Na de boeking worden de geboekte inkoopregels verwijderd uit de order. Er verschijnt een bericht als de boeking is voltooid. Hierna kunt u de geboekte posten bekijken op de verschillende pagina's die geboekte posten bevatten, zoals de pagina's **Leveranciersposten**, **Grootboekposten**, **Artikelposten**, **Geboekte inkoopontvangsten** en **Geboekte inkoopfacturen**.

In de meeste gevallen kunt u posten openen vanaf de betrokken kaart of het betreffende document. Kies bijvoorbeeld op de pagina **Leverancierskaart** de actie **Posten**.

## <a name="editing-ledger-entries"></a>Posten bewerken
U kunt bepaalde velden in geboekte inkoopdocumenten bewerken, zoals het veld **Betalingsreferentie**. Zie voor meer informatie [Geboekte documenten bewerken](across-edit-posted-document.md). Voor kritiekere velden die van invloed zijn op het controlespoor, moet u het boeken omkeren of ongedaan maken. Zie voor meer informatie [Journaalboekingen tegenboeken en ontvangsten/zendingen ongedaan maken](finance-how-reverse-journal-posting.md). 

## <a name="see-related-training-at-microsoft-learnlearnmodulesreceive-invoice-dynamics-d365-business-centralindex"></a>Zie Gerelateerde training op [Microsoft Learn](/learn/modules/receive-invoice-dynamics-d365-business-central/index)

## <a name="see-also"></a>Zie ook
[Geboekte documenten bewerken](across-edit-posted-document.md)  
[Meerdere documenten tegelijkertijd boeken](ui-batch-posting.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Documenten en dagboeken boeken](ui-post-documents-journals.md)  
[Niet-betaalde inkoopfacturen corrigeren of annuleren](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[Pagina's en informatie zoeken met Vertel me](ui-search.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
