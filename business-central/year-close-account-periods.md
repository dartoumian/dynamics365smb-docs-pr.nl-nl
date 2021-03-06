---
title: Boekingsperioden afsluiten voor een boekjaar | Microsoft Docs
description: Beschrijft hoe u de boekhoudperioden afsluit die een boekjaar vormen.
services: project-madeira
documentationcenter: ''
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: year closing, close accounting period, close fiscal year, bank account detailed trial balance
ms.date: 10/01/2019
ms.author: jswymer
ms.openlocfilehash: ba6cd85d50f9d2b4d98fb45cbd38bcc57e08e3a2
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2019
ms.locfileid: "2313805"
---
# <a name="close-accounting-periods"></a>Boekhoudperioden afsluiten
Wanneer een boekjaar is afgelopen, moet u de hierin opgenomen perioden afsluiten.

## <a name="to-close-accounting-periods"></a>Boekhoudperioden afsluiten
1. Kies het pictogram ![lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Boekingsperioden** in en kies vervolgens de gerelateerde koppeling.
2. Kies op de pagina **Boekingsperioden** de actie **Jaar afsluiten**.

    Als er meerdere boekjaren zijn geopend, wordt het vroegste boekjaar automatisch geselecteerd om te worden afgesloten. Er verschijnt een bericht waarin wordt aangegeven welk jaar wordt afgesloten en welke gevolgen dit heeft.
3. Kies de knop **Ja** om het jaar af te sluiten.

Het boekjaar is nu afgesloten en de selectievakjes **Afgesloten** en **Geblokkeerd** zijn ingeschakeld voor alle perioden van het jaar. U kunt het boekjaar niet meer openen en de selectievakjes **Afgesloten** en **Geblokkeerd** niet uitschakelen.

> [!NOTE]  
>   U kunt een boekjaar niet afsluiten voordat u een nieuw boekjaar hebt gemaakt. Wanneer een boekjaar is afgesloten, kunt u de begindatum van het volgende boekjaar niet meer wijzigen.

Zelfs als een boekjaar is afgesloten, kunt u er nog steeds grootboekposten voor boeken. Als u dit doet, worden de posten gemarkeerd als zijnde geboekt naar een afgesloten boekjaar en wordt het veld **Naboeking** geselecteerd.

Nadat een boekjaar is afgesloten, moet u de resultaten- of winst- en verliesrekeningen afsluiten en de jaarresultaten naar een balansrekening overbrengen. U kunt deze procedure herhalen telkens wanneer u boekt naar een afgesloten boekjaar.

## <a name="see-also"></a>Zie ook
[Boeken afsluiten](year-close-books.md)  
[De jaareinde-ultimopost boeken](year-how-post-year-end-close-entry.md)  
[Een nieuw boekjaar openen](finance-how-open-new-fiscal-year.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
