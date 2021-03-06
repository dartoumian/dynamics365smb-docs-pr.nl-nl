---
title: De extensie AMC Banking 365 Fundamentals gebruiken | Microsoft Docs
description: Wissel eenvoudig gegevens uit met uw banken door gegevens om te zetten in de indeling die ze nodig hebben.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: bank, format, data
ms.date: 10/14/2019
ms.author: bholtorf
ms.openlocfilehash: 9c9d927fb13d68c195bd457eb6bd2cbbfe078ea2
ms.sourcegitcommit: 86498fe4326b9ce26cc31e8645db27570d13bdf9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/06/2019
ms.locfileid: "2767535"
---
# <a name="using-the-amc-banking-365-fundamentals-extension"></a>De extensie AMC Banking 365 Fundamentals gebruiken
Met de extensie AMC Banking 365 Fundamentals kunt u eenvoudiger en nauwkeuriger gegevens naar uw banken verzenden. De extensie verbindt [!INCLUDE[d365fin](includes/d365fin_md.md)] met de service AMC Banking 365 Fundamentals voor Microsoft Dynamics 365 Business Central. Hiermee kunnen bankgegevens worden geconverteerd van [!INCLUDE[d365fin](includes/d365fin_md.md)] naar indelingen die worden gebruikt door meer dan 600 banken over de hele wereld. Dit maakt het bijvoorbeeld gemakkelijker om betalingen en tegoeden over te dragen aan leveranciers door de betalingen in te voeren in [!INCLUDE[d365fin](includes/d365fin_md.md)] en vervolgens te uploaden naar uw bank. De indelingen kunnen ook bankafstemmingsprocessen vereenvoudigen. Zie voor meer informatie [AMC Banking voor Microsoft Dynamics 365 Business Central](https://amcbanking.com/landing365bc/help).

> [!Note]
> AMC Banking heeft extra extensies gebouwd die werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]. In dit onderwerp wordt alleen de Fundamentals-extensie beschreven.

## <a name="using-our-demonstration-account"></a>Ons demonstratieaccount gebruiken
[!INCLUDE[d365fin](includes/d365fin_md.md)] wordt geleverd met een demonstratieaccount waarmee u de extensie AMC Banking 365 Fundamentals kunt uitproberen. We bieden standaardinstellingen om verbinding te maken met AMC Banking, met vermelding van de bankrekeningen waarvan gegevens kunnen worden opgehaald naar [!INCLUDE[d365fin](includes/d365fin_md.md)], plus enkele definities van gegevensuitwisseling. U kunt de verbindingsinstellingen bekijken op de pagina **AMC Banking instellen**. Voor bankrekeningen voert de extensie waarden in in de velden **Banknaam**, **Berichtnummers krediettransfer**, **Importindeling van bankafschrift** en **Exportindeling betaling** op bankrekeningkaarten.

Wij verstrekken de instellingen, maar om de extensie uit te proberen, moet u de gids van de begeleide instelling uitvoeren om ze toe te passen. Om de gids uit te voeren, kiest u op de pagina **AMC Banking instellen** de actie **Begeleide instelling**.

> [!Note]
> Het demo-account heeft een aantal beperkingen. Wanneer u bijvoorbeeld betalingen converteert, komt het bedrag in het geconverteerde bestand niet overeen met het werkelijke bedrag. In plaats daarvan bestaat het bedrag altijd uit vijf eenheden van de valuta die u gebruikt voor betalingen.  

## <a name="setting-up-the-extension"></a>De extensie instellen
Om met de extensie aan de slag te gaan, hoeft u slechts enkele eenvoudige stappen uit te voeren. Met een begeleide instelling wordt de verbinding gemaakt en de extensie ingeschakeld. De gids installeert onder andere de definities van de gegevensuitwisseling voor de configuratie van het exporteren/importeren van bankafschriften, en initieert de nummerreeks die wordt gebruikt voor overschrijvingsberichten.  

### <a name="to-set-up-the-required-permission-sets"></a>De vereiste machtigingensets instellen
Voordat iemand deze extensie kan gebruiken, moet uw beheerder de volgende machtigingensets kopiëren, ze bewerken en de bewerkte machtigingensets vervolgens toewijzen aan gebruikers:

* **D365 Basic**
* **D365-teamlid**
* **D365 Lezen**
* **IntelligentCloudBC**

Zie voor meer informatie [Een machtigingenset kopiëren](ui-define-granular-permissions.md#to-copy-a-permission-set).

Geef voor elke nieuwe machtigingenset alleen de machtiging **Lezen** voor de **AMC Banking-instellingentabel (20101)**. Zie voor meer informatie [Machtigingen handmatig maken of wijzigen](ui-define-granular-permissions.md#to-create-or-modify-permissions-manually).

### <a name="to-connect-the-extension-to-amc-banking"></a>De extensie verbinden met AMC Banking
1. Verkrijg een module en een serviceplan voor AMC Banking. Ga daarvoor naar de pagina [AMC-licentie](https://license.amcbanking.com/register).
2. Kies in [!INCLUDE[d365fin](includes/d365fin_md.md)] het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **AMC Banking instellen** in en kies de gerelateerde koppeling.  
3. Kies op de pagina **AMC Banking instellen** de actie **Begeleide instelling**.
4. Voer de stappen uit in het handleiding met begeleide instellingen.

### <a name="to-connect-bank-accounts-to-the-extension"></a>De bankrekeningen verbinden met de extensie
1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.
2. Open de kaart voor de bankrekening die u met de service wilt verbinden.
3. Kies in het veld **Banknaam** de indeling die uw bank vereist.  

   De indelingen worden zo gefilterd dat alleen de indelingen worden weergegeven die relevant zijn voor het land/de regio die is opgegeven voor de bankrekening.
4. Kies in het veld **Berichtnummers krediettransfer** de nummerreeks die moet worden gebruikt voor berichten bij betalingen.
5. Kies in de velden **Importindeling van bankafschrift** en **Exportindeling betaling** de definities van gegevensuitwisseling die uw bank nodig heeft.

## <a name="using-the-extension"></a>De extensie gebruiken
Het gebruik van deze extensie is een kwestie van gegevens exporteren naar de pagina **Betalingsdagboeken** pagina en deze vervolgens uploaden naar de webservice van uw bank. Zie voor meer informatie [Betalingen verrichten met Conversie van bankgegevens of SEPA-overmaking](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md).

> [!Note]
> U moet de velden **SWIFT-code** en **IBAN** invullen voor elke bankrekening.

### <a name="to-export-data-and-submit-it-to-your-bank"></a>Gegevens exporteren en indienen bij uw bank
> [!CAUTION]  
>  Wanneer u gegevens exporteert met de extensie AMC Banking 365 Fundamentals, zijn bepaalde bedrijfsgegevens zichtbaar voor de aanbieder van de service. De serviceprovider, AMC Consult A/S, is verantwoordelijk voor de privacy van deze informatie. Zie [AMC-privacybeleid](https://go.microsoft.com/fwlink/?LinkId=510158) voor meer informatie.

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Betalingsdagboeken** in en kies de gerelateerde koppeling.
2. Maak de dagboekregels die u wilt exporteren.  

   > [!Note]
   > Denk eraan dat u voor elke regel de optie **Elektronische betaling** in het veld **Betalingssoort** kiest.
3. Kies de actie **Exporteren**.

### <a name="to-import-and-apply-the-converted-file"></a>Het geconverteerde bestand importeren en toepassen
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Betalingsreconciliatiedagboek** in en kies de gerelateerde koppeling.
2. Kies de actie **Banktransactie importeren** en kies vervolgens het geconverteerde bestand.  

   [!INCLUDE[d365fin](includes/d365fin_md.md)] maakt een nieuw betalingsreconciliatiedagboek dat gegevens uit het bestand bevat. Zie voor meer informatie [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](receivables-apply-payments-auto-reconcile-bank-accounts.md).

## <a name="see-also"></a>Zie ook
[[!INCLUDE[d365fin](includes/d365fin_md.md)] aanpassen met behulp van extensies](ui-extensions.md)  
[Aan de slag](product-get-started.md)
