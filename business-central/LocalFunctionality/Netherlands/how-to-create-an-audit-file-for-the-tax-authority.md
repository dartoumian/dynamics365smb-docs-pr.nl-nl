---
title: Een auditfile voor de belastingdienst maken
description: Tijdens een controle van de boeken voor een boekjaar kan een belastinginspecteur om gegevens over de basistransacties vanuit het grootboek voor dat boekjaar vragen. Basistransacties worden gewoonlijk via dagboekposten verwerkt.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 2d3a53f4487110fd82267c5f2a5221ceff00ec11
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881358"
---
# <a name="create-an-audit-file-for-the-tax-authority"></a>Een auditfile voor de belastingdienst maken
Tijdens een controle van de boeken voor een boekjaar kan een belastinginspecteur om gegevens over de basistransacties vanuit het grootboek voor dat boekjaar vragen. Basistransacties worden gewoonlijk via dagboekposten verwerkt. Daarom vormen de dagboekposten de basis voor het auditbestand.  

 De belastingdienst stimuleert bedrijven om het auditfile te gebruiken, maar dat is niet verplicht.  

 De auditfile kan tevens worden gebruikt om gegevens uit te wisselen tussen bedrijven. U kunt elke gewenste periode selecteren, maar de begindatum en einddatum van de opgegeven periode moeten in hetzelfde boekjaar liggen.  

## <a name="to-make-an-audit-file"></a>Een auditfile maken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken"), voer **Belastingdienst - Auditfile** in en kies vervolgens de gerelateerde koppeling.  
2.  Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Begindatum**|Geef de begindatum of de periode op waarop de gegevens moeten worden gebaseerd.|  
    |**Einddatum**|Geef de einddatum of de periode op waarop de gegevens moeten worden gebaseerd.|  
    |**Beginsaldo uitsluiten**|Geeft op of het auditbestand het beginsaldo moet bevatten van grootboekrekeningen.<br /><br /> Het veld kan worden bewerkt als de begindatum van de periode gelijk is aan de begindatum van een boekjaar.|  

3.  Kies de knop **OK** om het auditbestand te maken. Als u het auditbestand niet wilt maken, kiest u de knop **Annuleren** om de pagina te sluiten.  

Wanneer u het rapport uitvoert, moet u de naam en locatie van het geëxporteerde bestand opgeven. De standaardbestandsnaam is **audit.xaf**, maar u kunt dat wijzigen. De bestandsextensie moet .xaf zijn.  

## <a name="see-also"></a>Zie ook  
 [Elektronische btw- en ICP-aangiften verzenden](electronic-vat-and-icp-declarations.md)
