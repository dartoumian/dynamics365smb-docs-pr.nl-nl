---
title: Artikelen picken | Microsoft Docs
description: De magazijnactiviteit van het picken van artikelen voordat deze worden verzonden of verbruikt, wordt op verschillende manieren uitgevoerd, afhankelijk van hoe de functies voor magazijnbeheer zijn geconfigureerd. De complexiteit van de [instelling](../configure-warehouse-processes.md) varieert, van geen magazijnfuncties via standaardmagazijnconfiguraties voor de afzonderlijke verwerking van orders in een of meer activiteiten tot geavanceerde configuraties waarbij alle activiteiten in een gestuurde werkstroom moeten worden uitgevoerd.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 3922c9696c7b0a06e49c0bfc505343bdfb58b231
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881507"
---
# <a name="pick-items"></a>Artikelen picken
De magazijnactiviteit van het picken van artikelen voordat deze worden verzonden of verbruikt, wordt op verschillende manieren uitgevoerd, afhankelijk van hoe de functies voor magazijnbeheer zijn geconfigureerd. De complexiteit varieert, van geen magazijnfuncties via standaardmagazijnconfiguraties voor de afzonderlijke verwerking van orders in een of meer activiteiten tot geavanceerde configuraties waarbij alle activiteiten in een gestuurde werkstroom moeten worden uitgevoerd. Zie voor meer informatie [Magazijnbeheer instellen](warehouse-setup-warehouse.md).

Als u de pickactiviteiten wilt ordenen en vastleggen met behulp van magazijndocumenten, schakelt u het selectievakje **Pick vereist** in bij de vestiging. Hiermee geeft u aan dat u, wanneer er artikelen moeten worden gepickt voor een uitgaand brondocument, het picken van deze artikelen door het programma wilt laten uitvoeren. Een uitgaand brondocument kan een verkooporder, een inkoopretourorder, een uitgaande transferorder of een serviceorder zijn waarvan de onderdelen moeten worden gepickt.

> [!NOTE]
> Hoewel de instelling **Pick vereist** wordt genoemd, kunt u nog wel verzendingen rechtstreeks vanuit het bronbedrijfsdocument boeken voor vestigingen waarvoor u dit selectievakje inschakelt.

Als voor uw vestiging pickverwerking is ingesteld, maar niet verzendingsverwerking, gebruikt u de pagina **Voorraadpick** om de pickinformatie in te delen, om deze af te drukken, om het resultaat van de pick in te voeren en om de pickinformatie te boeken, waardoor vervolgens de verzending van de artikelen wordt geboekt. Wanneer u onderdelen voor een productieorder pickt, wordt ook het verbruik geboekt wanneer u de pick boekt.

Wanneer voor uw vestiging de verwerking van zowel picken als verzending vereist is en de velden **Pick vereist** en **Verzending vereist** op de locatiekaart zijn ingeschakeld, gebruikt u de pagina **Magazijnpick** om de pick te verwerken. U voert een magazijnpick op dezelfde manier uit als een voorraadpick, maar in plaats van de pickgegevens te boeken, registreert u de pick. Met dit registratieproces wordt de verzending niet geboekt, maar maakt u de artikelen alleen beschikbaar voor verzending. Als magazijnmanager kunt u met behulp van pickvoorstellen pickgegevens ordenen voordat de afzonderlijke magazijnpickinstructies worden gemaakt.

In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.   

|**Als u dit wilt doen**|**Zie**|
|------------|-------------|  
|De verzending van artikelen direct boeken in het document voor uitgaande orders, omdat er geen magazijnfuncties zijn. (Werkt hetzelfde voor verkooporders, uitgaande transferorders en retourverzendingen.)|[Artikelen verzenden](warehouse-how-ship-items.md)|  
|Artikelen per order picken en de verzending in dezelfde activiteit boeken, in een standaardmagazijnconfiguratie.|[Artikelen picken met een voorraadpick](warehouse-how-to-pick-items-with-inventory-picks.md)|
|Artikelen opslaan voor meerdere orders in een geavanceerde magazijnconfiguratie.|[Artikelen picken met een magazijnpick](warehouse-how-to-pick-items-for-warehouse-shipment.md)|  
|Onderdelen picken voor productie of assemblage in een standaardmagazijnconfiguratie.|[Picken voor assemblage of productie in standaardmagazijnconfiguraties](warehouse-how-to-pick-for-production.md)|
|Onderdelen picken voor productie of assemblage in een geavanceerde magazijnconfiguratie.|[Picken voor assemblage of productie in geavanceerde magazijnconfiguraties](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md)|  
|Geoptimaliseerde pickinstructies plannen voor een aantal verzendingen, in plaats van magazijnmedewerkers direct laten handelen naar geboekte verzendingen.|[Picks plannen in het voorstel](warehouse-how-to-plan-picks-in-worksheets.md)|  
|Artikelen technisch picken voor een speciaal doel, zoals een productieafdeling die extra onderdelen nodig heeft, zodanig dat de artikelen technisch het magazijn niet verlaten.|[Picken en opslaan zonder een brondocument](warehouse-how-to-create-put-aways-from-internal-put-aways.md)|
|Begrijpen hoe artikelen automatisch worden gepickt op basis van de vervaldatum, bijvoorbeeld beperkt houdbare artikelen.|[Picken op basis van FEFO](warehouse-picking-by-fefo.md)|
|Een pickregel in meerdere regels splitsen, bijvoorbeeld omdat er onvoldoende artikelen beschikbaar zijn in de aangewezen opslaglocatie.|[Magazijnactiviteitsregels splitsen](warehouse-how-to-split-warehouse-activity-lines.md)|
|Direct toegang verkrijgen tot picks die aan u als magazijnmedewerker zijn toegewezen.|[Magazijntoewijzingen zoeken](warehouse-how-to-find-your-warehouse-assignments.md)|  

## <a name="see-also"></a>Zie ook  
[Magazijnbeheer](warehouse-manage-warehouse.md)  
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)     
[Assemblagebeheer](assembly-assemble-items.md)    
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
