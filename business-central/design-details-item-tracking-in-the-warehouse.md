---
title: Ontwerpdetails - Artikeltracering in het magazijn | Microsoft Docs
description: De verwerking van serie- en lotnummers is hoofdzakelijk een magazijntaak. Daarom hebben alle inkomende en uitgaande magazijndocumenten standaardfunctionaliteit voor het toewijzen en selecteren van artikeltraceringsnummers. Omdat het reserveringsysteem echter op artikelposten is gebaseerd, worden magazijnactiviteitsdocumenten die alleen magazijnposten registreren, niet volledig ondersteund.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, serial number, lot number, outbound documents
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: b7fdb0d6495f1512e1ab3bf80eb76a5dad9d87e5
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2880181"
---
# <a name="design-details-item-tracking-in-the-warehouse"></a>Ontwerpdetails: Artikeltracering in het magazijn
De verwerking van serie- en lotnummers is hoofdzakelijk een magazijntaak. Daarom hebben alle inkomende en uitgaande magazijndocumenten standaardfunctionaliteit voor het toewijzen en selecteren van artikeltraceringsnummers.  

Omdat het reserveringsysteem echter op artikelposten is gebaseerd, worden magazijnactiviteitsdocumenten die alleen magazijnposten registreren, niet volledig ondersteund. Omdat reserveringen en artikeltraceringsnummers alleen op locatieniveau kunnen worden verwerkt, en niet op het niveau van de opslaglocatie en de zone, kan de pagina **Artikeltraceringsregels** niet worden geopend vanuit magazijnactiviteitsdocumenten. Hetzelfde geldt voor de pagina **Reservering**.  

Nadat een serienummer of lotnummer is toegevoegd aan een artikel op een magazijnlocatie, kan het vrijelijk binnen het magazijn worden verplaatst en geherclassificeerd met behulp van een onafhankelijke artikeltraceringstructuur die niet gerelateerd is aan het reserveringsysteem. De velden **Serienummer** en **Lotnr.** zijn rechtstreeks toegankelijk op magazijndocumentregels. Wanneer het serie- of lotnummer later wordt gebruikt bij uitgaande posten, wordt het gesynchroniseerd met het reserveringssysteem als onderdeel van de normale opslaglocatieherwaardering. Zie [Ontwerpdetails: Integratie met voorraad](design-details-integration-with-inventory.md) voor meer informatie.  

Het reserveringsysteem houdt echter rekening met magazijnactiviteiten wanneer beschikbaarheid wordt berekend. Artikelen die zijn toegewezen aan picks, of zijn geregistreerd als gepickt, kunnen bijvoorbeeld niet worden gereserveerd. Zie voor meer informatie [Ontwerpdetails: Magazijnbeschikbaarheid](design-details-availability-in-the-warehouse.md).

## <a name="see-also"></a>Zie ook  
[Ontwerpdetails: Artikeltracering](design-details-item-tracking.md)  
[Ontwerpdetails: Integratie met voorraad](design-details-integration-with-inventory.md)  
[Ontwerpdetails: Magazijnbeschikbaarheid](design-details-availability-in-the-warehouse.md)  
[Ontwerpdetails: Ontwerp artikeltracering](design-details-item-tracking-design.md)
