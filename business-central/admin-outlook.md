---
title: Business Central gebruiken met Outlook | Microsoft Docs
description: Deze service is nauw geïntegreerd met Office 365. U kunt al uw bedrijfs- en e-mailcommunicatie met klanten en leveranciers rechtstreeks in Outlook beheren.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: SMTP, mail, Office 365
ms.date: 01/13/2020
ms.author: edupont
ms.openlocfilehash: 5098087fc5d4ea821e32d644c159deeb5289b837
ms.sourcegitcommit: ead69ebe5b29927876a4fb23afb6c066f8854591
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/14/2020
ms.locfileid: "2953012"
---
# <a name="using-business-central-as-your-business-inbox-in-outlook"></a>Business Central gebruiken als uw bedrijfsinbox in Outlook

[!INCLUDE[d365fin](includes/d365fin_md.md)] introduceert de mogelijkheid bedrijfsinteracties te beheren met uw klanten en leveranciers, direct in Microsoft Outlook. Met de Outlook-invoegtoepassingen voor [!INCLUDE[d365fin](includes/d365fin_md.md)] kunt u financiële gegevens bekijken met betrekking tot klanten en leveranciers, en financiële documenten maken en verzenden, zoals offertes en facturen.  

## <a name="getting-the-add-in"></a>De invoegtoepassing downloaden
Het is gemakkelijk aan de gang te gaan met de [!INCLUDE[d365fin](includes/d365fin_md.md)]-invoegtoepassing voor Outlook. In de begeleide instelling **Uw bedrijfsinbox instellen in Outlook** kunt u de verbinding instellen voor uzelf of voor uw organisatie, als uw organisatie Office 365 gebruikt. Specificeer eenvoudig uw Office 365-gebruikersnaam en -wachtwoord, als u daarom wordt gevraagd, en vertel ons of u een voorbeeld van een e-mailbericht wilt ontvangen. De [!INCLUDE[d365fin](includes/d365fin_md.md)]-invoegtoepassing wordt automatisch toegevoegd aan uw Outlook. Zie voor meer informatie [Minimumvereisten voor Outlook](product-requirements.md#outlook).  

Wanneer u daarna Outlook start, wordt er een e-mailbericht van de *Dynamics 365 Business Central-beheerder* weergegeven. De nieuwe invoegtoepassingen zijn toegevoegd aan het Outlook-lint en in de browser ziet u de [!INCLUDE[prodshort](includes/prodshort.md)]-invoegtoepassingen direct boven of onder de hoofdtekst van het e-mailbericht. De invoegtoepassingen worden regelmatig bijgewerkt en u wordt in Outlook gewaarschuwd dat een nieuwe versie klaar staat.  

> [!TIP]
> Als u de nieuwe Outlook op het web gebruikt, dan kunnen de [!INCLUDE [prodshort](includes/prodshort.md)]-invoegtoepassingen worden verborgen onder **Meer acties**. Als u de invoegtoepassing vaak gebruikt, kunt u deze vastzetten zodat deze altijd direct zichtbaar is. Zie voor meer informatie [Invoegtoepassingen gebruiken in Outlook op het web](https://support.office.com/article/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce?ns=OLWAO365B&version=16).  

Als u met meer dan een [!INCLUDE [prodshort](includes/prodshort.md)]-bedrijf werkt, kunt u in Outlook gemakkelijk tussen bedrijven schakelen. Kies in de actiebalk van de invoegtoepassing **Meer acties** en dan ziet u de optie om te schakelen tussen bedrijven.  

<!--TEMP-->
> [!NOTE]
> Schakelen tussen bedrijven vereist [!INCLUDE [prodshort](includes/prodshort.md)] 2019 releasewave 2 of hoger zoals aangekondigd in het [versieplan](/dynamics365-release-plan/2019wave2/dynamics365-business-central/switch-between-companies-business-inbox-outlook).

Sommige bedrijven die Office 365 gebruiken, beperken de machtigingen van gebruikers om invoegtoepassingen te installeren. U moet er dus voor zorgen dat u een Office 365-abonnement hebt dat e-mail omvat en u toestaat invoegtoepassingen te installeren. Als u de invoegtoepassing toch wilt bekijken, kunt u [Office 365 gratis uitproberen](https://products.office.com/try).  

## <a name="using-the-contact-insights-add-in"></a>De invoegtoepassing Contact Insights gebruiken
Stel u eens voor dat u een e-mailbericht ontvangt van een klant die een offerte voor enkele artikelen wil. U kunt rechtstreeks in Outlook de [!INCLUDE[d365fin](includes/d365fin_md.md)]-invoegtoepassing openen, die de afzender als een klant herkent en de klantkaart voor diens bedrijf opent. Vanuit dit dashboard kunt u overzichtsinformatie voor de klant zien, evenals inzoomen voor meer details over specifieke documenten. U kunt ook de verkoophistorie van de klant bekijken. Als dit een nieuw contact is, kunt u het als nieuwe klant toevoegen in [!INCLUDE[d365fin](includes/d365fin_md.md)] zonder Outlook te verlaten.  

In de invoegtoepassing kunt u een verkoopofferte maken en deze naar de klant verzenden zonder Outlook te verlaten. Alle informatie die u in de verkoopofferte moet verzenden, is beschikbaar in uw bedrijfsinbox in Outlook.  
Nadat u de gegevens hebt ingevoerd, kunt u de offerte boeken. U kunt deze vervolgens via e-mail verzenden. [!INCLUDE[d365fin](includes/d365fin_md.md)] genereert een .pdf-bestand met de verkoopofferte en koppelt dat aan het e-mailbericht dat u opstelt in de invoegtoepassing.  

En als u een e-mail van een leverancier ontvangt, kunt u net zo de invoegtoepassing gebruiken om met leveranciers en inkoopfacturen te werken.  

Soms wilt u meer velden bekijken dan u in de invoegtoepassing kunt weergeven, zoals wanneer u regels in een factuur wilt invullen. Als u wat meer ruimte wilt krijgen om mee te werken kunt u de invoegtoepassing op een aparte pagina openen. Het is nog deel van Outlook, maar u hebt meer ruimte. Terwijl u in de pop-upweergave gegevens voor het document invoert, worden de wijzigingen automatisch opgeslagen. Wanneer u klaar bent met het invoeren van gegevens voor het document, klikt u op **OK**. Als u het invoegtoepassingsframe kiest in Outlook, wordt het document automatisch vernieuwd met de wijzigingen die u in de pop-upweergave hebt aangebracht.  

## <a name="creating-invoices-from-your-meeting-appointments"></a>Facturen maken op basis van uw vergaderafspraken
Sommige bedrijven registreren alle factureerbare afspraken in de Outlook-agenda. Met [!INCLUDE[d365fin](includes/d365fin_md.md)] kunt u de factuur voor de klant rechtstreeks op basis van het agenda-item maken. Open de afspraak, start vervolgens de [!INCLUDE[d365fin](includes/d365fin_md.md)]-invoegtoepassing , zoek bestaande gegevens op of maak meteen een factuur of een ander verkoopdocument aan.  

## <a name="doing-quick-document-lookup"></a>Snel documenten opzoeken
De invoegtoepassing [!INCLUDE[d365fin](includes/d365fin_md.md)] Document Links geeft u snel toegang tot documenten die worden genoemd in e-mailberichten. De invoegtoepassing is beschikbaar voor een e-mailbericht als een documentnummer wordt genoemd in de hoofdtekst van het bericht. Als u de invoegtoepassing opent, hebt u snel toegang tot het document.  

Als u bijvoorbeeld een e-mailbericht ontvangt met de tekst *S-QUO100*, identificeert [!INCLUDE[d365fin](includes/d365fin_md.md)] het als een verkoopofferte en kunt u het document dus openen in Outlook. Kies in Outlook de knop **Documentkoppelingen**, direct boven de hoofdtekst van het e-mailbericht. Kies in de Outlook-webapp de tekst *S-QUO1001* in het hoofdgedeelte van het e-mailbericht.  

In de invoegtoepassing Document Links kunt u acties wijzigen en uitvoeren met het document, net als in [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="adding-the-add-ins-manually"></a>Invoegtoepassingen handmatig toevoegen
In sommige gevallen worden de invoegtoepassingen niet automatisch aan Outlook toegevoegd. Zelfs als u of een collega de begeleide instelling namens het bedrijf hebt uitgevoerd, is [!INCLUDE[d365fin](includes/d365fin_md.md)] mogelijk niet zichtbaar in Outlook. Als u dit probleem tegenkomt, kunt u de [!INCLUDE[d365fin](includes/d365fin_md.md)]-invoegtoepassingen handmatig toevoegen.  

Eerst moet u controleren of u toegang hebt tot de invoegtoepassingen in uw Office 365-account. Open gewoon uw Outlook in een browser, open een bericht, selecteer **Meer acties** (...) boven aan het bericht en kies vervolgens onder aan de lijst **Invoegtoepassingen ophalen**. Dit opent de pagina **Invoegtoepassingen voor Outlook**, waar u [!INCLUDE[prodshort](includes/prodshort.md)] kunt inschakelen voor uw Outlook. Wanneer u daarna opnieuw naar Outlook navigeert, moet [!INCLUDE[prodshort](includes/prodshort.md)] beschikbaar zijn.  

U kunt ook in de Outlook-bureaubladclient controleren of [!INCLUDE[d365fin](includes/d365fin_md.md)] wordt vermeld op de pagina **Invoegtoepassingen ophalen**.  

In beide gevallen moet u, als [!INCLUDE[d365fin](includes/d365fin_md.md)] nog steeds niet beschikbaar is, moet u de manifestbestanden van de invoegtoepassing ophalen. Neem contact op met uw Office 365-beheerder voor meer informatie.

## <a name="using-other-email-accounts"></a>Andere e-mailaccounts gebruiken

De invoegtoepassingen zijn ontworpen om te worden gebruikt met Office 365. Als u [!INCLUDE [prodshort](includes/prodshort.md)] on-premises gebruikt, zal uw beheerder weten of u de [!INCLUDE [prodshort](includes/prodshort.md)]-invoegtoepassingen in Outlook kunt gebruiken. Zie voor meer informatie [Welk e-mailadres kan ik gebruiken voor [!INCLUDE[prodshort](includes/prodshort.md)]?](across-faq.md#what-email-address-can-i-use-with-) en [Functies die specifieke omstandigheden vereisen](/dynamics365/business-central/dev-itpro/features-not-implemented-on-premises#features-that-require-specific-circumstances).  

## <a name="see-related-training-at-microsoft-learnlearnmodulesalternative-interfaces-dynamics-365-business-centralindex"></a>Zie Gerelateerde training op [Microsoft Learn](/learn/modules/alternative-interfaces-dynamics-365-business-central/index)

## <a name="see-also"></a>Zie ook

[Aan de slag](product-get-started.md)  
[Business Central op mijn mobiele apparaat krijgen](install-mobile-app.md)  
[Documenten per e-mail verzenden](ui-how-send-documents-email.md)  
[Financiën](finance.md)  
[Verkoop](sales-manage-sales.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Minimale vereisten voor Outlook](product-requirements.md#outlook)  
[Invoegtoepassingen gebruiken in Outlook op het web](https://support.office.com/article/Using-Add-ins-in-Outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce?appver=OWB150)  
