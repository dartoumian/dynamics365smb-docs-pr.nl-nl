---
title: Financiële processen instellen| Microsoft Docs
description: Meer informatie over de taken om financiën in uw bedrijf in te stellen voor al uw boekhoudings-, controle- of boekingsbehoeften.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accounting, auditing, bookkeeping
ms.date: 01/13/2020
ms.author: sgroespe
ms.openlocfilehash: fa8b324c0a63f7c00209579878b9739af8178041
ms.sourcegitcommit: ead69ebe5b29927876a4fb23afb6c066f8854591
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/14/2020
ms.locfileid: "2953656"
---
# <a name="setting-up-finance"></a>Financiën instellen
Voordat u kunt beginnen met de uitvoering van uw bedrijf, moet u regels en standaardinstellingen opgeven voor de manier waarop u financiële processen voor het bedrijf wilt beheren. Ten eerste moet u de kern van de boekhoudadministratie van het bedrijf instellen: het rekeningschema. Vervolgens stelt u de boekingsgroepen in, waarmee standaard-grootboekrekeningen efficiënter kunnen worden toegewezen aan klanten, leveranciers en artikelen.

Sommige financiële instellingen kunnen automatisch worden uitgevoerd met behulp van guides voor begeleide instelling en sommige moeten handmatig worden uitgevoerd. Zie voor meer informatie [Voorbereid zijn om zaken te doen](ui-get-ready-business.md).

Met dimensies kunt u verschillende soorten informatie toevoegen aan elke transactie. U kunt de basisdimensies van uw bedrijf instellen, zoals Projecten en Afdelingen. Later kunt u zo nodig meer dimensies toevoegen en tijdelijke dimensies instellen voor gebruik gedurende een beperkte tijdsperiode, bijvoorbeeld in verband met een verkoopcampagne. Zie voor meer informatie [Werken met dimensies](finance-dimensions.md).

Veel van de instellingstaken moeten worden voltooid voordat u financiële transacties kunt gaan registreren, maar u kunt de meeste instellingen naderhand wijzigen. Sommige instellingstaken zijn optioneel: u stelt bijvoorbeeld alleen IC-boekingen en -consolidaties in als u met meerdere bedrijven werkt. Sommige instellingstaken moeten periodiek worden herhaald, zoals het opgeven van de periode waarin een boeking is toegestaan.  

De volgende tabel beschrijft een reeks taken, met koppelingen naar de onderwerpen waarin deze worden beschreven.

| Als u dit wilt doen | Zie |
| --- | --- |
| Bepaal hoe u uw leveranciers wilt betalen. |[Betalingsmethoden definiëren](finance-payment-methods.md) |
| Geef de boekingsgroepen op die entiteiten zoals klanten, leveranciers, artikelen, resources en verkoop- en inkoopdocumenten toewijzen aan grootboekrekeningen. |[Boekingsgroepen instellen](finance-posting-groups.md)|
|Maak rapportageschema's en definieer rekeningcategorieën om de inhoud van financiële grafieken en rapporten te definiëren, zoals de rapporten Balans en Resultatenrekening.|[Financiële rapportage voorbereiden met rapportageschema's en rekeningcategorieën](bi-how-work-account-schedule.md)|
|Stel een tolerantie in waarmee het systeem een factuur sluit hoewel de betaling, inclusief een eventuele korting, het bedrag op de factuur niet volledig dekt.|[Werken met betalingstolerantie en contantkortingstolerantie](finance-payment-tolerance-and-payment-discount-tolerance.md)|
| Stel boekperioden in. |[Een nieuw boekjaar openen](finance-how-open-new-fiscal-year.md) |
| Definiëren hoe u btw-bedragen die u hebt geïnd voor verkopen, rapporteert aan de belastingdienst. |[Btw instellen](finance-setup-vat.md)|
|Verwerking voorbereiden van niet gerealiseerde btw in verband met op kas gebaseerde boekhoudingsmethoden.|[Ongerealiseerde btw voor op kas gebaseerde boekhouding instellen](finance-setup-unrealized-vat.md)|
| Stel uw verkoop- en inkoopfuncties in om betalingen in vreemde valuta's te verwerken.|[Vereffening van posten in verschillende valuta's inschakelen](finance-how-enable-application-ledger-entries-different-currencies.md)
|Definieer een of meer extra valuta's, zodat bedragen automatisch worden gerapporteerd in zowel de LV als de extra rapportagevaluta in elke grootboekpost en in andere posten.|[Een extra rapportagevaluta instellen.](finance-how-setup-additional-currencies.md)|
|Pas periodiek extra valuta-equivalenten aan in verband met schommelende wisselkoersen.|[Valutawisselkoersen bijwerken](finance-how-update-currencies.md)|
|Definieer meerdere rentepercentages voor verschillende perioden voor vertraagde betalingen in handelstransacties.|[Meerdere rentetarieven instellen](finance-how-to-set-up-multiple-interest-rates.md)|
|Voorbereiden van automatisch afronden van factuurbedragen wanneer u facturen maakt.|[Factuurafronding instellen](finance-set-up-invoice-rounding.md)|
| Voeg nieuwe rekeningen aan bestaande rekeningschema's. |[Het rekeningschema instellen](finance-setup-chart-accounts.md) |
| Stel de BI-diagrammen (Business Intelligence) in om cashflow te analyseren. |[Cashflowanalyse instellen](finance-setup-cash-flow-analyses.md) |
|Facturering van een klant te schakelen die niet in het systeem is opgenomen.|[Contant betalende klanten instellen](finance-how-to-set-up-cash-customers.md)|
| Intrastat-rapportage instellen en het rapport indienen bij een autoriteit | [Intrastat instellen en rapporteren](finance-how-setup-report-intrastat.md)|
|Zorg dat een post in een grootboek wordt toegewezen aan verschillende rekeningen wanneer u het dagboek boekt, hetzij aantal, percentage of bedrag.|[Verdeelsleutels in dagboeken gebruiken](ui-how-use-allocation-keys-general-journals.md)|

## <a name="see-related-training-at-microsoft-learnlearnpathsset-up-financial-management-dynamics-365-business-central"></a>Zie Gerelateerde training op [Microsoft Learn](/learn/paths/set-up-financial-management-dynamics-365-business-central/)

## <a name="see-also"></a>Zie ook
[Financiën](finance.md)  
[Bankrekeningen reconciliëren](bank-manage-bank-accounts.md)  
[Werken met dimensies](finance-dimensions.md)  
[Bedrijfsgegevens importeren uit andere financiële systemen](across-import-data-configuration-packages.md)  
[Cashflow in uw bedrijf analyseren](finance-analyze-cash-flow.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
