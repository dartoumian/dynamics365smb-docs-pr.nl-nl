---
title: Over de kosten van de gereedgemelde productieorder | Microsoft Docs
description: Het gereedmelden van de productieorder is een belangrijke taak in het voltooien van de levenscyclus van de waardering van het artikel dat wordt geproduceerd. De uiteindelijke kosten, inclusief verschillen in een standaardwaarderingsomgeving, werkelijke kosten in een FIFO, gemiddelde of LIFO-waarderingsomgeving, worden berekend met behulp van de batchverwerking Kostprijs herwaarderen - Artikelposten.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 509ee1cdbcf9c0ddd362435ed4d2319561a9e731
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2019
ms.locfileid: "2302641"
---
# <a name="about-finished-production-order-costs"></a>Over de kosten van de gereedgemelde productieorder
Het gereedmelden van de productieorder is een belangrijke taak in het voltooien van de levenscyclus van de waardering van het artikel dat wordt geproduceerd. De uiteindelijke kosten (inclusief verschillen in een standaard waarderingsomgeving; werkelijke kosten in een FIFO, gemiddelde, of LIFO waarderingsomgeving) worden berekend met behulp van de batchverwerking **Kostprijs herwaarderen - Artikelposten**, die voorziet in financiële reconciliatie van de kostprijzen van artikelproductie. Een productieorder kan alleen in aanmerking komen voor kostenwaardering als de status **Gereedgemeld** is. Het is daarom van groot belang dat na voltooiing de status van een productieorder wordt gewijzigd in **Gereedgemeld**.  

## <a name="example"></a>Opmerking  
 Als u in een omgeving met vaste verrekenprijzen materiaal verbruikt voor het produceren van een artikel, worden de kosten van het artikel plus arbeid en overhead simpelweg naar OHW overgebracht. Wanneer het item wordt geproduceerd, wordt OHW verminderd met het bedrag van de vaste verrekenprijs van het artikel. Gewoonlijk is het saldo hiervan niet nul. Om met deze kosten op nul uit te komen, moet u de batchverwerking **Kostprijs herwaarderen - Artikelposten** uitvoeren, waarbij u erop moet letten dat alleen productieorders met de status **Gereedgemeld** in aanmerking komen voor herwaardering.  

## <a name="see-also"></a>Zie ook  
[Voorraadkosten beheren](finance-manage-inventory-costs.md)  
[Productie](production-manage-manufacturing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
