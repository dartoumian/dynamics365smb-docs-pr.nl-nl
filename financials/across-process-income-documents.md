---
title: Inkomende documenten verwerken| Microsoft Docs
description: Als u een extern document wilt registreren, zoals een PDF, in Dynamics 365 for Financials, moet u eerst een inkomende documentrecord maken of voltooien.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: b4d344c52bf6f10d00f2157fbdb45903402f6c55
ms.contentlocale: nl-nl
ms.lasthandoff: 07/07/2017


---
# <a name="processing-incoming-documents"></a>Inkomende documenten verwerken
Als u een extern document wilt registreren in [!INCLUDE[d365fin](includes/d365fin_md.md)], moet u eerst een inkomende documentrecord maken of voltooien. U kunt dit handmatig doen of u kunt een foto van het externe document maken en vervolgens de inkomende documentrecord maken met het afbeeldingsbestand bijgevoegd.

Vanuit PDF- of afbeeldingsbestanden die u ontvangt van uw handelspartners, kunt u elektronische documenten laten genereren door een externe OCR-service (Optical Character Recognition - optische tekenherkenning), die kunnen worden geconverteerd naar documentrecords in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Bijvoorbeeld, wanneer u facturen in PDF-indeling van uw leverancier ontvangt, kunt u deze naar de OCR-service verzenden vanuit het venster **Inkomende documenten**. U kunt ook het bestand naar de OCR-service via e-mail verzenden. Wanneer u het elektronische document terug ontvangt, wordt automatisch een gerelateerde inkomende documentrecord gemaakt. Na enkele seconden krijgt u het bestand weer terug van de OCR-service als een elektronische factuur die kan worden geconverteerd naar een inkoopfactuur voor de leverancier.

| Als u dit wilt doen | Zie |
| --- | --- |
| Maak inkomende documentrecords handmatig of automatisch door een foto te maken van een papieren ontvangstbewijs, bijvoorbeeld. |[Procedure: Inkomende documentrecords maken](across-how-create-income-document-records.md) |
| Gebruik een OCR-service om PDF- en afbeeldingsbestanden naar elektronische documenten om te zetten die bijvoorbeeld kunnen worden geconverteerd naar inkoopfacturen in [!INCLUDE[d365fin](includes/d365fin_md.md)]. Train de OCR-service om fouten te voorkomen als de volgende keer vergelijkbare gegevens worden verwerkt. |[Procedure: OCR gebruiken om PDF- en afbeeldingsbestanden te converteren naar elektronische documenten](across-how-use-ocr-pdf-images-files.md) |
| Verbind of verwijder inkomende documentrecords voor elk niet-geboekte verkoop- of inkoopdocument en voor elke klant- of grootboekpost uit het document of de post. |[Procedure: Inkomende documentrecords maken direct van documenten en posten](across-how-connect-disconnect-income-document-records.md) |
| Vanuit de vensters **Rekeningschema** en **Grootboekposten** zoekt u naar grootboekposten voor geboekte documenten die geen inkomende documentrecords hebben, en koppelt u deze centraal aan bestaande records of maakt u nieuwe records met gekoppelde documentbestanden. |[Procedure: Geboekte documenten zonder inkomende documentrecords zoeken](across-how-find-posted-documents-without-income-document-records.md) |
| Beter overzicht krijgen door inkomende documentrecords in te stellen op Verwerkt om ze te verwijderen uit de standaardweergave. |[Procedure: Vele inkomende documentrecords beheren](across-how-manage-many-income-document-records.md) |

## <a name="see-also"></a>Zie ook
[Inkomende documenten](across-income-documents.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
