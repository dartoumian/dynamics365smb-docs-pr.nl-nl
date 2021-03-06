---
title: Records handmatig koppelen en synchroniseren | Microsoft Docs
description: Als een integratietabeltoewijzing wordt gesynchroniseerd, kunnen gegevens in alle records in een tabel in Business Central en Dynamics 365 Sales worden gesynchroniseerd die zijn gekoppeld.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 10/01/2019
ms.author: bholtorf
ms.openlocfilehash: 0c70b1ba34af32b7cf542149c8f15cb191761358
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2019
ms.locfileid: "2308113"
---
# <a name="couple-and-synchronize-records-manually"></a>Records handmatig koppelen en synchroniseren
In dit onderwerp wordt beschreven hoe u een of meer records in [!INCLUDE[d365fin](includes/d365fin_md.md)] koppelt aan records in [!INCLUDE[crm_md](includes/crm_md.md)]. Door records te koppelen kunt u [!INCLUDE[crm_md](includes/crm_md.md)]-informatie vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)]bekijken en andersom. Door de koppeling kunt u ook gegevens synchroniseren tussen de records. U kunt bestaande records koppelen of nieuwe records maken en koppelen.

> [!Note]
> Gegevens koppelen en synchroniseren met [!INCLUDE[crm_md](includes/crm_md.md)] is alleen beschikbaar als de systeembeheerder een verbinding tussen [!INCLUDE[d365fin](includes/d365fin_md.md)] en [!INCLUDE[crm_md](includes/crm_md.md)] heeft gemaakt. Een snelle manier om dat te controleren is de **Klant**-kaart te openen en de actie **Koppeling instellen** te zoeken. Als de actie beschikbaar is, zijn de apps verbonden.   

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a>Een record koppelen  
1.  In [!INCLUDE[d365fin](includes/d365fin_md.md)] opent u de kaart voor de record die moeten worden gekoppeld. Bijvoorbeeld de klant- of contactkaart.  

    U kunt ook slechts de lijstpagina openen en de record selecteren die u wilt koppelen.  

2.  Kies de actie **Koppeling instellen**.  
3.  Vul de velden in en kies de knop **OK**.  

## <a name="to-synchronize-a-single-record"></a>Eén record synchroniseren  
1.  In [!INCLUDE[d365fin](includes/d365fin_md.md)] opent u de kaart voor de record die moeten worden gekoppeld. Bijvoorbeeld de klant- of contactkaart.  
2.  Kies de actie **Nu synchroniseren**.  
3.  Als een record kan worden gesynchroniseerd vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)] naar [!INCLUDE[crm_md](includes/crm_md.md)] of vanuit [!INCLUDE[crm_md](includes/crm_md.md)] naar [!INCLUDE[d365fin](includes/d365fin_md.md)], selecteert u de optie die de richting van gegevensupdate opgeeft, en kiest u vervolgens **OK**.  

## <a name="to-synchronize-multiple-records"></a>Meerdere records synchroniseren  
1.  Open in [!INCLUDE[d365fin](includes/d365fin_md.md)] de lijstpagina voor de record, zoals lijstpagina Klanten of Contact.  
2.  Selecteer de records die u wilt synchroniseren en kies vervolgens de actie **Nu synchroniseren**.  
3.  Als records kunnen worden gesynchroniseerd vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)] naar [!INCLUDE[crm_md](includes/crm_md.md)] of vanuit [!INCLUDE[crm_md](includes/crm_md.md)] naar [!INCLUDE[d365fin](includes/d365fin_md.md)], selecteert u de optie die de richting van gegevensupdate opgeeft, en kiest u vervolgens **OK**.  

## <a name="see-also"></a>Zie ook  
[Microsoft Dynamics 365 Sales gebruiken vanuit Business Central](marketing-integrate-dynamicscrm.md)
