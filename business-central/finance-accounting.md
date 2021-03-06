---
title: Business Central-accountantservaring | Microsoft Docs
description: Meer informatie over de accountantsportal voor Business Central en het accountantrolcentrum dat interne en externe accountants in het cliëntbedrijf ondersteunt.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 01/06/2020
ms.author: edupont
ms.openlocfilehash: 50cc4aba9f3a01b9518d974cf011de3b9b20a4da
ms.sourcegitcommit: 877af26e3e4522ee234fbba606615e105ef3e90a
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/28/2020
ms.locfileid: "2991853"
---
# <a name="accountant-experiences-in-included365fin_longincludesd365fin_long_mdmd"></a>Accountantervaringen binnen [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]
Elk bedrijf moet zijn boekhouding doen en aftekenen. Sommige bedrijven hebben een externe accountant en andere hebben een accountant in dienst. Ongeacht wat voor accountant u bent, u kunt het rolcentrum **Accountant** gebruiken als uw thuis binnen [!INCLUDE[d365fin](includes/d365fin_md.md)]. Van hieruit hebt u toegang tot alle pagina's die u in uw werk nodig hebt.  

## <a name="accountant-role-center"></a>Rolcentrum Accountant
Het rolcentrum is een dashboard met activiteittegels die realtime cijfers bevatten en die u snel toegang geven tot gegevens. In het lint boven op de pagina hebt u toegang tot meer acties, zoals het openen van de vaakst gebruikte financiële rapporten en de rekeningoverzichten in Excel. Op de navigatiebalk bovenin kunt u snel schakelen tussen de lijsten die u het meest gebruikt. Hier ziet u andere gebieden, zoals **Geboekte documenten** met de diverse soorten documenten die het bedrijf heeft geboekt.  

Als [!INCLUDE[d365fin](includes/d365fin_md.md)] nieuw voor u is, kunt u een overzicht van video's direct vanuit uw rolcentrum starten. U kunt ook een **Aan de slag**-rondleiding starten die wijst op belangrijke gebieden.  

## <a name="inviteaccountant"></a>Uw externe accountant uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)]
Als u een externe auditor gebruikt om uw boeken en financiële rapportage te beheren, kan uw beheerder deze uitnodigen voor uw [!INCLUDE[d365fin](includes/d365fin_md.md)], zodat hij of zij met u kan werken aan uw fiscale gegevens. [!INCLUDE[d365fin](includes/d365fin_md.md)] omvat drie licenties van het type Externe accountant. Zie de [Microsoft Dynamics 365 Business Central Licentiehandleiding](https://go.microsoft.com/fwlink/?LinkId=871590) voor meer informatie over licenties.

Als de accountant toegang heeft gekregen tot uw [!INCLUDE[d365fin](includes/d365fin_md.md)], kan hij of zij het rolcentrum **Accountant** gebruiken, dat eenvoudig toegang tot de meest relevante pagina's voor hun werk biedt.  

We hebben het voor u eenvoudig gemaakt om uw externe accountant uit te nodigen. Open gewoon de pagina **Gebruikers** en kies de actie **Externe accountant uitnodigen** op het lint. Er wordt een e-mail voor u gemaakt. Voeg het werke-mailadres van uw accountant eraan toe en verzend de uitnodiging.  

> [!Note]  
> Dit vereist dat u SMTP-e-mail hebt ingesteld. Zie [E-mail instellen](admin-how-setup-email.md) voor meer informatie.   

<!-- ![Invite your accountant](./media/finance-invite-accountant/invite-accountant.png)-->

> [!IMPORTANT]  
> Het e-mailadres van de accountant moet een werkadres op basis van Azure Active Directory zijn. Als de accountant een ander type e-mail gebruikt, kan de uitnodiging niet worden verzonden. 
> 
> Omdat deze taak toegang vereist voor het beheren van gebruikers en licenties in Azure Active Directory, moet de gebruiker die deze uitnodiging verzendt, de rol **Globale beheerder** of **Gebruikersbeheer** hebben in het Office 365-beheercentrum. Zie voor meer informatie [Over beheerdersrollen](/office365/admin/add-users/about-admin-roles) in de Office 365-beheerdersinhoud.  

### <a name="adding-your-accountant-to-your-office-365-via-azure-portal"></a>Uw accountant toevoegen aan uw Office 365 via Azure Portal

Als uw beheerder of wederverkoper geen gebruik wenst te maken van de guide **Externe accountant uitnodigen**, kunnen ze een externe gebruiker toevoegen aan de Azure Portal en deze gebruiker de licentie voor een externe accountant toewijzen. Zie [Snelle start: gastgebruikers toevoegen aan uw directory in de Azure-portal](/azure/active-directory/b2b/b2b-quickstart-add-guest-users-portal) voor meer informatie.

#### <a name="to-add-your-accountant-as-a-guest-user"></a>Uw accountant als gastgebruiker toevoegen

1. Open de [Azure Portal](https://portal.azure.com/).
2. Selecteer **Azure Active Directory** in het linkerdeelvenster.
3. Selecteer onder **Beheren** de optie **Gebruikers**.
4. Selecteer **Nieuwe gastgebruiker**.
5. Selecteer op de pagina **Nieuwe gebruiker** de optie **Gebruiker uitnodigen** en voeg informatie over uw externe accountant toe.  

   Voeg desgewenst een persoonlijk welkomstbericht aan de accountant toe om te laten weten dat hij of zij wordt toegevoegd aan uw [!INCLUDE [prodshort](includes/prodshort.md)].

6. Selecteer **Uitnodigen** om de uitnodiging automatisch te verzenden. Er verschijnt een melding rechtsboven bij het bericht **Gebruiker is uitgenodigd**. 
7. Nadat u de uitnodiging hebt verzonden, wordt het gebruikersaccount automatisch als gast aan de directory toegevoegd.

Daarna moet u de nieuwe gastgebruiker een licentie voor [!INCLUDE [prodshort](includes/prodshort.md)] toewijzen.

#### <a name="to-give-your-accountant-access-to-your-include-prodshortincludesprodshortmd"></a>Uw accountant toegang geven tot uw [!INCLUDE [prodshort](includes/prodshort.md)]

1. Kies **Profiel** in de Azure Portal bij de zojuist toegevoegde gebruiker en kies **Bewerken**
2. Voer in het veld **Gebruikslocatie** het desbetreffende land in en kies **Opslaan**.
3. Kies **Licenties** en open **Toewijzingen**.
4. Kies de **Dynamics 365 Business Central Externe accountant**-licentie.  

    Als deze licentie niet beschikbaar is, moet u in plaats daarvan een beschikbare **Dynamics 365 Business Central voor IW's**-licentie gebruiken.
5. Sla de toewijzing op.

Als dit lukt, wordt de licentie toegewezen aan de gastgebruiker en wordt het gastaccount gemaakt.

### <a name="importing-the-new-user-into-include-prodshortincludesprodshortmd"></a>De nieuwe gebruiker importeren in [!INCLUDE [prodshort](includes/prodshort.md)]

De accountant ontvangt een e-mail met de melding dat hij of zij toegang heeft gekregen tot uw Active Directory. Daarna moet u de accountant toegang geven tot het juiste bedrijf in [!INCLUDE [prodshort](includes/prodshort.md)].

#### <a name="to-add-the-accountant-to-the-right-company"></a>De accountant toevoegen aan het juiste bedrijf

1. Open het [!INCLUDE [prodshort](includes/prodshort.md)]-bedrijf waarvoor u de accountant toegang wilt geven op [https://businesscentral.dynamics.com](https://businesscentral.dynamics.com).
2. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Gebruikers** in en kies de desbetreffende koppeling.  
3. Kies de actie **Nieuwe gebruikers ophalen uit Office 365**.

Hiermee wordt het gebruikersaccount dat u in de Azure Portal hebt gemaakt, naar het bedrijf geïmporteerd. Zie [Een gebruiker toevoegen in Business Central](ui-how-users-permissions.md#to-add-a-user-in-business-central) voor meer informatie.  

Als u toegang wilt geven aan meerdere bedrijven, moet u zich bij elk bedrijf aanmelden en dit proces herhalen. U kunt ook de machtigingsgroepen voor het gebruikersprofiel van de accountant bijwerken in [!INCLUDE [prodshort](includes/prodshort.md)], zoals het toewijzen van de *D365 Bus Premium*-gebruikersgroep. Zie [Machtigingen toewijzen aan gebruikers en groepen](ui-define-granular-permissions.md) voor meer informatie.  

## <a name="accountant-hub"></a>Accountant Hub

Als u een accountant met verschillende cliënten bent, kunt u [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)] gebruiken voor een beter overzicht van uw cliënten. Van daaruit kunt u toegang krijgen tot de tenant van elke cliënt in [!INCLUDE[d365fin](includes/d365fin_md.md)] en het accountantrolcentrum gebruiken zoals hierboven beschreven. Zie voor meer informatie [Welkom bij [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]](/dynamics365/accountants/index).  

> [!NOTE]
> [!INCLUDE [d365acc_long_md](includes/d365acc_long_md.md)] is momenteel in openbare preview op een beperkt aantal markten.

## <a name="see-also"></a>Zie ook

[Financiën](finance.md)  
[Financiën instellen](finance-setup-finance.md)  
[Het grootboek en het rekeningschema](finance-general-ledger.md)  
[Afsluitingsjaren en -perioden](year-close-years-periods.md)  
[Werken met dimensies](finance-dimensions.md)  
[Financiële overzichten analyseren in Excel:](finance-analyze-excel.md)  
[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Cashflowanalyse instellen](finance-setup-cash-flow-analyses.md)  
[Welkom bij [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]](/dynamics365/accountants/index)  
[Dynamics 365 - Accountant Hub op Microsoft.com](https://www.microsoft.com/dynamics365/financial-insights-for-accountants)  
