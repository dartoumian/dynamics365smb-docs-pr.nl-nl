---
title: Een prioriteitsniveau toewijzen aan een leverancier | Microsoft Docs
description: U kunt nummers toewijzen aan uw leveranciers om deze te prioriteren en betalingsvoorstellen in Business Central te vergemakkelijken.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 538a6f4b1ead61afde223391441bf097f3c26f77
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2877588"
---
# <a name="prioritize-vendors"></a>De prioriteit van leveranciers bepalen
[!INCLUDE[d365fin](includes/d365fin_md.md)] heeft een functie die voorstellen kan doen voor betalingen aan leveranciers, bijvoorbeeld bij betalingen die binnenkort moeten worden betaald, of als voor een betaling een korting mogelijk is. Zie voor meer informatie [Leveranciersbetalingen voorstellen](payables-how-suggest-vendor-payments.md).

Eerst moet u aan uw leveranciers eerst een prioriteit toewijzen door nummers aan hen toe te wijzen.
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE3PRGa]

## <a name="to-prioritize-vendors"></a>Leveranciers in een prioriteitsvolgorde plaatsen
1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Leveranciers** in en kies de desbetreffende koppeling.
2. Selecteer de relevante leverancier en kies **Bewerken**.
3. Voer in het veld **Prioriteit** een nummer in.

In [!INCLUDE[d365fin](includes/d365fin_md.md)] heeft het laagste nummer, 0 uitgezonderd, de hoogste prioriteit. Als u bijvoorbeeld de nummers 1, 2 en 3 toewijst, heeft nummer 1 de hoogste prioriteit.

Als u geen prioriteitsnummer wilt toekennen aan een leverancier, laat u het veld **Prioriteit** leeg. Die leverancier wordt onder alle leveranciers met prioriteitsnummers geplaatst wanneer u betalingsvoorstellen in het programma inschakelt. U kunt zo veel prioriteitsniveaus invoeren als er nodig zijn.

## <a name="see-also"></a>Zie ook
[Inkoop instellen](purchasing-setup-purchasing.md)  
[Betalingsverplichtingen beheren](payables-manage-payables.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
