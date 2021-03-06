---
title: Artikelkaarten maken voor goederen of services| Microsoft Docs
description: U maakt artikelkaarten voor services die u als uren en voor fysieke producten verkoopt, zoals componenten, gereedgemelde goederen, onderdelen of grondstoffen, die u uit uw voorraad verkoopt.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item, finished good, component, raw material, assembly item
ms.date: 11/27/2019
ms.author: sgroespe
ms.openlocfilehash: 3cb9ffd6dadaeba7aab782c0bd8f45d3f4aa5387
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878338"
---
# <a name="register-new-items"></a>Nieuwe artikelen registreren
Artikelen vormen met andere producten de basis van uw bedrijf, de goederen of services waarin u handelt. Elk artikelproduct moet worden geregistreerd als een artikelkaart.

Artikelkaarten bevatten de informatie die is vereist om artikelen te kopen, op te slaan, te verkopen, te leveren en te verantwoorden.

De artikelkaart kan van het type **Voorraad**, **Service** of **Niet-voorraad** zijn om op te geven of het artikel een fysieke voorraadeenheid, een eenheid voor arbeidskosten of een fysieke eenheid die niet in voorraad wordt getraceerd, is. Zie voor meer informatie [Over artikeltypen](inventory-about-item-types.md).

Een artikel kan als bovenliggend artikel met onderliggende artikelen in een stuklijst worden gestructureerd. In [!INCLUDE[d365fin](includes/d365fin_md.md)] kan een stuklijst een assemblagestuklijst of productiestuklijst zijn, afhankelijk van het gebruik. Zie [Werken met stuklijsten](inventory-how-work-BOMs.md) voor meer informatie.

Als u hetzelfde artikel inkoopt bij meerdere leveranciers, kunt u die leveranciers aan de artikelkaart koppelen. De leveranciers worden vervolgens weergegeven op de pagina **Artikelleveranciers**, zodat u gemakkelijk een alternatieve leverancier kunt selecteren.

Artikelen die u aan uw klanten aanbiedt, maar die u niet in uw systeem wilt beheren tot u ze begint te verkopen, kunnen worden ingesteld als catalogusartikelen. Catalogusartikelen moeten niet worden verward met normale artikelen van het type **Niet-voorraad**. Zie voor meer informatie [Werken met catalogusartikelen](inventory-how-work-nonstock-items.md).  

> [!NOTE]  
> Als klantsjablonen voor verschillende klantsoorten bestaan, wordt een pagina automatisch weergegeven wanneer u een nieuwe artikelkaart maakt van waaruit u een geschikte sjabloon kunt selecteren. Als er slechts één artikelsjabloon bestaat, gebruiken nieuwe artikelkaarten altijd deze sjabloon.

In de volgende procedure wordt uitgelegd hoe u een geheel nieuwe artikelkaart maakt. U kunt ook nieuwe artikelkaarten maken door bestaande te kopiëren. Zie voor meer informatie [Bestaande items kopiëren om nieuwe items te maken](inventory-how-copy-items.md).<br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE47eLx]

## <a name="to-create-a-new-item-card"></a>Een nieuwe artikelkaart maken
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Artikelen** in en kies de gerelateerde koppeling.  
2. Kies op de pagina **Artikelen** de actie **Nieuw**.

    Als er slechts één artikelsjabloon bestaat, wordt vervolgens een nieuwe artikelkaart geopend waarin enkele velden zijn ingevuld met informatie van de sjabloon.
3. Kies op de pagina **Selecteer een sjabloon voor een nieuw artikel** de sjabloon die u wilt gebruiken voor de nieuwe artikelkaart.
4. Kies de knop **Ok**. Een nieuwe artikelkaart wordt geopend met enkele velden met informatie uit de sjabloon.
5. Ga door met velden op de artikelkaart in te vullen of te wijzigen. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> In het veld **Waarderingsmethode** bepaalt u hoe de eenheidskostprijs van het artikel wordt berekend door de veronderstellingen die worden gemaakt over de stroom van artikelen in het bedrijf. Afhankelijk van het type item zijn vijf waarderingsmethoden beschikbaar. Zie [Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md) voor meer informatie.
>
> Als u de waarderingsmethode **Gemiddeld** gebruikt, worden de eenheidskosten van een artikel berekend als de gemiddelde eenheidskosten op een bepaald moment na een aanschaf. Voorraad wordt gewaardeerd met de aanname dat alle voorraad tegelijkertijd wordt verkocht. Met deze instelling kunt u het veld **Kostprijs** kiezen en zo op de pagina **Overzicht gemiddelde-kostenberekening** de historie bekijken van de transacties waaruit de gemiddelde kostprijs wordt berekend.

U kunt speciale prijzen of kortingen weergeven of bewerken die u voor het artikel verleent als aan bepaalde criteria, zoals klant, minimaal orderaantal of einddatum wordt voldaan. U doet dit door de actie **Speciale prijzen instellen** of **Speciale kortingen instellen** te kiezen. Elke rij op de pagina **Verkoopprijzen** vertegenwoordigt bijvoorbeeld een speciale prijs. Elke kolom vertegenwoordigt een criterium dat moet gelden om een klant de speciale prijs te geven die u invoert in het veld **Eenheidsprijs** op de pagina **Verkoopprijzen**. Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).

Het artikel is nu geregistreerd en de artikelkaart is klaar om voor inkoop- en verkoopdocumenten te worden gebruikt.

Als u deze artikelkaart als sjabloon wilt gebruiken wanneer u nieuwe artikelkaarten maakt, kunt u deze opslaan als een sjabloon. Zie de volgende onderwerpen voor meer informatie.

## <a name="to-save-the-item-card-as-a-template"></a>De artikelkaart als sjabloon opslaan
1. Kies op de pagina **Artikelkaart** de actie **Opslaan als sjabloon**. De pagina **Artikelsjabloon** opent de weergave van de artikelkaart als sjabloon.
2. Vul de benodigde velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Als u sjablonen wilt hergebruiken, kiest u de actie **Dimensies**. De pagina **Dimensiesjablonen** geeft alle dimensiecodes weer die voor het item zijn ingesteld.
4. Bewerk of typ dimensiecodes die van toepassing zijn op nieuwe artikelkaarten die worden gemaakt met de sjabloon.
5. Wanneer u de nieuwe artikelsjabloon hebt voltooid, kiest u de knop **OK**.

De artikelsjabloon wordt toegevoegd aan de lijst met artikelsjablonen, zodat u deze kunt gebruiken om nieuwe artikelkaarten te maken.

## <a name="to-set-up-multiple-vendors-for-an-item"></a>Meerdere leveranciers voor een artikel instellen  
Als u hetzelfde artikel bij meerdere leveranciers inkoopt, moet u informatie over elk van deze leveranciers invoeren, bijvoorbeeld informatie over prijzen, levertermijn, kortingen, enzovoort.  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Artikelen** in en kies de gerelateerde koppeling.  
2.  Selecteer het betreffende artikel en kies vervolgens de actie **Bewerken**.  
3.  Kies de actie **Leveranciers**.  
4.  Klik op het veld **Leveranciersnr.** en selecteer vervolgens de leverancier waarvoor u het artikel wilt instellen.  
5.  Het invullen van de overige velden is optioneel.  
6.  Herhaal stap 2 t/m 5 voor elke leverancier waarbij u het artikel wilt kunnen inkopen.

Deze leveranciers worden vervolgens weergegeven op de pagina **Artikelleveranciers**, dat u opent vanuit de artikelkaart, zodat u gemakkelijk een alternatieve leverancier kunt selecteren.

## <a name="see-also"></a>Zie ook
[Nummerreeksen maken](ui-create-number-series.md)  
[Voorraad](inventory-manage-inventory.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Verkoop](sales-manage-sales.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
