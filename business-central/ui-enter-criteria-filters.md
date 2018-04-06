---
title: Gegevens zoeken en filtercriteria invoeren | Microsoft Docs
description: Beschrijft hoe u met filters werkt, zoals het Snelfilter, om de resultaten te verfijnen die u krijgt wanneer u gegevens zoekt.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: a7fd74ad235e51b1793b02e19834bdb0bd17820b
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="searching-filtering-and-sorting-data"></a><span data-ttu-id="ec675-103">Gegevens zoeken, filteren en sorteren</span><span class="sxs-lookup"><span data-stu-id="ec675-103">Searching, Filtering, and Sorting Data</span></span>
<span data-ttu-id="ec675-104">U kunt een paar dingen doen om records in een lijst te vinden, te lokaliseren en te scannen.</span><span class="sxs-lookup"><span data-stu-id="ec675-104">There are a few things that you can do that will help you find, pinpoint, and scan records in a list.</span></span> <span data-ttu-id="ec675-105">U kunt de records bijvoorbeeld sorteren, doorzoeken en filteren.</span><span class="sxs-lookup"><span data-stu-id="ec675-105">These include sorting, searching and filtering.</span></span>

<span data-ttu-id="ec675-106">Wanneer u naar gegevens, zoals klantnamen, adressen of productgroepen wilt zoeken, voert u criteria in.</span><span class="sxs-lookup"><span data-stu-id="ec675-106">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="ec675-107">In zoekcriteria kunt u alle cijfers en letters gebruiken die u normaal in het specifieke veld gebruikt.</span><span class="sxs-lookup"><span data-stu-id="ec675-107">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="ec675-108">Daarnaast kunt u speciale symbolen gebruiken om de resultaten verder te filteren.</span><span class="sxs-lookup"><span data-stu-id="ec675-108">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="ec675-109">U kunt op twee manieren zoeken: met het snelfilter of kolomfilters.</span><span class="sxs-lookup"><span data-stu-id="ec675-109">There are two ways to search: using the Quick Filter or column filters.</span></span>

## <a name="sorting"></a><span data-ttu-id="ec675-110">Sorteervolgorde</span><span class="sxs-lookup"><span data-stu-id="ec675-110">Sorting</span></span>
<span data-ttu-id="ec675-111">Met de sorteerfunctie krijgt u snel een overzicht van de gegevens.</span><span class="sxs-lookup"><span data-stu-id="ec675-111">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="ec675-112">Als u veel klanten hebt, kunt u er bijvoorbeeld voor kiezen hen te sorteren op **Klantnr.**, **Klantboekingsgroep**, **Valutacode**, **Land-/regiocode** of **Btw-nummer** voor het door u gewenste overzicht.</span><span class="sxs-lookup"><span data-stu-id="ec675-112">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="ec675-113">Als u een lijst wilt sorteren, kunt u een kolomkoptekst kiezen om te schakelen tussen op- en aflopend, of de kleine pijl-omlaag in de kolomkop kiezen en vervolgens **Oplopend** of **Aflopend** kiezen.</span><span class="sxs-lookup"><span data-stu-id="ec675-113">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small downs arrow in the column heading, and then choose **Ascending** or **Descending**.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="ec675-114">Sorteren wordt niet ondersteund bij afbeeldingen, BLOB-velden, FlowFilters en velden die niet deel van een tabel zijn.</span><span class="sxs-lookup"><span data-stu-id="ec675-114">Sorting is not supported images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching-by-using-the-quick-filter"></a><span data-ttu-id="ec675-115">Zoeken met het snelfilter</span><span class="sxs-lookup"><span data-stu-id="ec675-115">Searching by using the Quick Filter</span></span>
<span data-ttu-id="ec675-116">U kunt filters toevoegen aan alle pagina's met het Snelfilter.</span><span class="sxs-lookup"><span data-stu-id="ec675-116">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="ec675-117">Het Snelfilter wordt ingeschakeld door het vergrootglaspictogram in de rechterbovenhoek van een pagina te kiezen.</span><span class="sxs-lookup"><span data-stu-id="ec675-117">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="ec675-118">Dit type filter wordt gebruikt voor een snelle invoer van criteria.</span><span class="sxs-lookup"><span data-stu-id="ec675-118">This filtering type is used for a fast entry of criteria.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="ec675-119">Het snelfilter biedt een eenvoudig toegang tot filtergegevens door onbewerkte tekst in te voeren, maar biedt ook veel opties voor zoekcriteria.</span><span class="sxs-lookup"><span data-stu-id="ec675-119">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="ec675-120">Afhankelijk van of u normale tekst of tekst met symbolen invoert, werkt het snelfilter anders.</span><span class="sxs-lookup"><span data-stu-id="ec675-120">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  

* <span data-ttu-id="ec675-121">Als u gewone tekst in de zoekcriteria opgeeft, worden de zoekcriteria geïnterpreteerd als een hoofdletterongevoelige zoekactie die bepaalde tekst bevat.</span><span class="sxs-lookup"><span data-stu-id="ec675-121">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
* <span data-ttu-id="ec675-122">Als u tekst inclusief symbolen in de zoekcriteria opgeeft, worden de zoekcriteria precies zo geïnterpreteerd als u ze hebt ingevoerd en wordt onderscheid gemaakt tussen hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="ec675-122">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="ec675-123">Snelfiltercriteria</span><span class="sxs-lookup"><span data-stu-id="ec675-123">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="ec675-124">Zoekcriteria</span><span class="sxs-lookup"><span data-stu-id="ec675-124">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="ec675-125">Geïnterpreteerd als...</span><span class="sxs-lookup"><span data-stu-id="ec675-125">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="ec675-126">Retourneert...</span><span class="sxs-lookup"><span data-stu-id="ec675-126">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="ec675-127">man</span><span class="sxs-lookup"><span data-stu-id="ec675-127">man</span></span></TD>
    <TD><span data-ttu-id="ec675-128">@&#42;man&#42;</span><span class="sxs-lookup"><span data-stu-id="ec675-128">@&#42;man&#42;</span></span></TD>
    <TD><span data-ttu-id="ec675-129">Alle records met de tekst <b>man</b> en ongevoelig voor hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="ec675-129">All records that contain the text <b>man</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="ec675-130">se</span><span class="sxs-lookup"><span data-stu-id="ec675-130">se</span></span></TD>
    <TD><span data-ttu-id="ec675-131">@&#42;zo&#42;</span><span class="sxs-lookup"><span data-stu-id="ec675-131">@&#42;se&#42;</span></span></TD>
    <TD><span data-ttu-id="ec675-132">Alle records met de tekst <b>se</b> en ongevoelig voor hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="ec675-132">All records that contain the text <b>se</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="ec675-133">Man&#42;</span><span class="sxs-lookup"><span data-stu-id="ec675-133">Man&#42;</span></span></TD>
    <TD><span data-ttu-id="ec675-134">Begint met <b>Man</b> en is hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="ec675-134">Starts with <b>Man</b> and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="ec675-135">Alle records die beginnen met de tekst <b>Man</b>.</span><span class="sxs-lookup"><span data-stu-id="ec675-135">All records that start with the text <b>Man</b>.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="ec675-136">'man'</span><span class="sxs-lookup"><span data-stu-id="ec675-136">'man'</span></span></TD>
    <TD><span data-ttu-id="ec675-137">Een exacte tekst en gevoelig voor hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="ec675-137">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="ec675-138">Alle records die precies overeenkomen met <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="ec675-138">All records that match <b>man</b> exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="ec675-139">@man\*</span><span class="sxs-lookup"><span data-stu-id="ec675-139">@man\*</span></span> </TD>
    <TD><span data-ttu-id="ec675-140">Begint met en is niet hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="ec675-140">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="ec675-141">Alle records die beginnen met <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="ec675-141">All records that start with <b>man</b>.</span></span></TD>
  </TR>
    <TR>
    <TD><span data-ttu-id="ec675-142">@&#42;man</span><span class="sxs-lookup"><span data-stu-id="ec675-142">@&#42;man</span></span></TD>
    <TD><span data-ttu-id="ec675-143">Eindigt met en is niet hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="ec675-143">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="ec675-144">Alle records die eindigen met <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="ec675-144">All records that end with <b>man</b>.</span></span></TD>
  </TR>
</TABLE>

> [!NOTE]  
>   <span data-ttu-id="ec675-145">U kunt geen jokerteken gebruiken bij het filteren op opsommingsvelden, zoals het veld **Status** op verkooporders.</span><span class="sxs-lookup"><span data-stu-id="ec675-145">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="ec675-146">Om een filter voor deze veldsoort in te voeren, kunt u de numerieke waarde als een filterparameter invoeren.</span><span class="sxs-lookup"><span data-stu-id="ec675-146">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="ec675-147">Bijvoorbeeld: gebruik in het veld **Status** op een verkooporder met de waarden **Open**, **Vrijgegeven**, **Wacht op goedkeuring** en **Wacht op vooruitbetaling** de waarden **0**, **1**, **2** en **3** om voor deze opties te filteren.</span><span class="sxs-lookup"><span data-stu-id="ec675-147">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span> 

## <a name="searching-by-using-column-filters"></a><span data-ttu-id="ec675-148">Zoeken met kolomfilters</span><span class="sxs-lookup"><span data-stu-id="ec675-148">Searching by using column Filters</span></span>
<span data-ttu-id="ec675-149">U kunt een filter toevoegen aan een of meer kolommen in een lijst.</span><span class="sxs-lookup"><span data-stu-id="ec675-149">You can add a filter on one or more columns in a list.</span></span> <span data-ttu-id="ec675-150">Kolomfilters bieden een meer flexibele en geavanceerde methode dan het snelfilter.</span><span class="sxs-lookup"><span data-stu-id="ec675-150">Filtering on columns is more flexible and enhanced than the Quick Filter.</span></span> 

### <a name="to-add-a-filter-on-a-column"></a><span data-ttu-id="ec675-151">Een filter toevoegen aan een kolom</span><span class="sxs-lookup"><span data-stu-id="ec675-151">To add a filter on a column</span></span>
1.  <span data-ttu-id="ec675-152">Voordat u een filter toevoegt, klikt u op het pictogram ![Als overzicht weergeven](media/ui_show_as_list_icon.png "pijl-links Als overzicht weergeven") om de weergave te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="ec675-152">Before you add a filter, choose ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to change to the list view.</span></span>
2. <span data-ttu-id="ec675-153">Kies de pijl-omlaag in de kolomkop en kies **Filter**.</span><span class="sxs-lookup"><span data-stu-id="ec675-153">Choose the downwards arrow in the column heading, and then choose **Filter**.</span></span>
3. <span data-ttu-id="ec675-154">Ga op een van de volgende manieren te werk:</span><span class="sxs-lookup"><span data-stu-id="ec675-154">Do one of the following:</span></span> 
  -  <span data-ttu-id="ec675-155">Kies *...* naast het vak om een waarde in de lijst te selecteren.</span><span class="sxs-lookup"><span data-stu-id="ec675-155">Choose *...* next to the box to select a value from a list.</span></span>
  -  <span data-ttu-id="ec675-156">Voer filtercriteria in het vak in.</span><span class="sxs-lookup"><span data-stu-id="ec675-156">Enter filter criteria in the box.</span></span> <span data-ttu-id="ec675-157">Zie het volgende gedeelte voor details.</span><span class="sxs-lookup"><span data-stu-id="ec675-157">See the next section for details.</span></span>
4. <span data-ttu-id="ec675-158">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="ec675-158">Choose the **OK** button.</span></span>

## <a name="filter-criteria-and-symbols"></a><span data-ttu-id="ec675-159">Filtercriteria en -symbolen</span><span class="sxs-lookup"><span data-stu-id="ec675-159">Filter criteria and symbols</span></span>
<span data-ttu-id="ec675-160">U kunt bij de invoer van criteria alle cijfers en letters gebruiken die u normaal ook kunt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="ec675-160">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="ec675-161">Daarnaast kunt u speciale symbolen gebruiken om de resultaten verder te filteren.</span><span class="sxs-lookup"><span data-stu-id="ec675-161">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="ec675-162">De volgende tabellen bevatten de tekens die in filters kunnen worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="ec675-162">The following tables show the symbols which can be used in filters.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="ec675-163">Het kan voorkomen dat veldwaarden deze symbolen bevatten en u hierop wilt filteren.</span><span class="sxs-lookup"><span data-stu-id="ec675-163">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="ec675-164">Hiervoor moet u de filterexpressie opnemen die het symbool tussen aanhalingstekens (“) bevat.</span><span class="sxs-lookup"><span data-stu-id="ec675-164">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="ec675-165">Als u wilt filteren op records die beginnen met de tekst *S&R*, is de filterexpressie bijvoorbeeld **'S&R\*'**.</span><span class="sxs-lookup"><span data-stu-id="ec675-165">For example, if you want to filter on records that start with the text *S&R*, the filter expression is **'S&R\*'**.</span></span>  
  
### <a name="-interval"></a><span data-ttu-id="ec675-166">(..) Interval</span><span class="sxs-lookup"><span data-stu-id="ec675-166">(..) Interval</span></span>  
  
|<span data-ttu-id="ec675-167">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-167">Sample Expression</span></span>|<span data-ttu-id="ec675-168">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-168">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-169">1.100..2.100</span><span class="sxs-lookup"><span data-stu-id="ec675-169">1100..2100</span></span>|<span data-ttu-id="ec675-170">Nummers 1100 t/m 2100</span><span class="sxs-lookup"><span data-stu-id="ec675-170">Numbers 1100 through 2100</span></span>|  
|<span data-ttu-id="ec675-171">..2.500</span><span class="sxs-lookup"><span data-stu-id="ec675-171">..2500</span></span>|<span data-ttu-id="ec675-172">Tot en met 2500</span><span class="sxs-lookup"><span data-stu-id="ec675-172">Up to and including 2500</span></span>|  
|<span data-ttu-id="ec675-173">..31 12 00</span><span class="sxs-lookup"><span data-stu-id="ec675-173">..12 31 00</span></span>|<span data-ttu-id="ec675-174">Datums tot en met 31.12.00</span><span class="sxs-lookup"><span data-stu-id="ec675-174">Dates up to and including 12 31 00</span></span>|  
|<span data-ttu-id="ec675-175">P8..</span><span class="sxs-lookup"><span data-stu-id="ec675-175">P8..</span></span>|<span data-ttu-id="ec675-176">Gegevens voor boekhoudperiode 8 en verder</span><span class="sxs-lookup"><span data-stu-id="ec675-176">Information for accounting period 8 and thereafter</span></span>|  
|<span data-ttu-id="ec675-177">..23</span><span class="sxs-lookup"><span data-stu-id="ec675-177">..23</span></span>|<span data-ttu-id="ec675-178">Van begindatum tot 23 lopende maand, lopend jaar 23:59:59</span><span class="sxs-lookup"><span data-stu-id="ec675-178">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|<span data-ttu-id="ec675-179">23..</span><span class="sxs-lookup"><span data-stu-id="ec675-179">23..</span></span>|<span data-ttu-id="ec675-180">Van 23 lopende maand, lopend jaar 00:00:00 tot eindtijd</span><span class="sxs-lookup"><span data-stu-id="ec675-180">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|<span data-ttu-id="ec675-181">22..23</span><span class="sxs-lookup"><span data-stu-id="ec675-181">22..23</span></span>|<span data-ttu-id="ec675-182">Van 22 lopende maand, lopend jaar 0:00:00 tot 23 lopende maand, lopend jaar 23:59:59</span><span class="sxs-lookup"><span data-stu-id="ec675-182">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  
  
### <a name="124-eitheror"></a><span data-ttu-id="ec675-183">(&#124;) Of/of</span><span class="sxs-lookup"><span data-stu-id="ec675-183">(&#124;) Either/or</span></span>  
  
|<span data-ttu-id="ec675-184">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-184">Sample Expression</span></span>|<span data-ttu-id="ec675-185">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-185">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-186">1200&#124;1300</span><span class="sxs-lookup"><span data-stu-id="ec675-186">1200&#124;1300</span></span>|<span data-ttu-id="ec675-187">Nummers met 1200 of 1300</span><span class="sxs-lookup"><span data-stu-id="ec675-187">Numbers with 1200 or 1300</span></span>|  
  
### <a name="-not-equal-to"></a><span data-ttu-id="ec675-188">(<>) Niet gelijk aan</span><span class="sxs-lookup"><span data-stu-id="ec675-188">(<>) Not equal to</span></span>  
  
|<span data-ttu-id="ec675-189">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-189">Sample Expression</span></span>|<span data-ttu-id="ec675-190">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-190">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-191"><>0</span><span class="sxs-lookup"><span data-stu-id="ec675-191"><>0</span></span>|<span data-ttu-id="ec675-192">Alle nummers behalve 0</span><span class="sxs-lookup"><span data-stu-id="ec675-192">All numbers except 0</span></span><br /><br /> <span data-ttu-id="ec675-193">Met de SQL Server-optie kunt u dit teken combineren met jokertekens.</span><span class="sxs-lookup"><span data-stu-id="ec675-193">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="ec675-194"><>A\* betekent bijvoorbeeld 'Niet gelijk aan tekst die begint met A'.</span><span class="sxs-lookup"><span data-stu-id="ec675-194">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  
  
### <a name="-greater-than"></a><span data-ttu-id="ec675-195">(>) Groter dan</span><span class="sxs-lookup"><span data-stu-id="ec675-195">(>) Greater than</span></span>  
  
|<span data-ttu-id="ec675-196">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-196">Sample Expression</span></span>|<span data-ttu-id="ec675-197">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-197">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-198">>1.200</span><span class="sxs-lookup"><span data-stu-id="ec675-198">>1200</span></span>|<span data-ttu-id="ec675-199">Nummers groter dan 1200</span><span class="sxs-lookup"><span data-stu-id="ec675-199">Numbers greater than 1200</span></span>|  
  
### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="ec675-200">(>=) Groter dan of gelijk aan</span><span class="sxs-lookup"><span data-stu-id="ec675-200">(>=) Greater than or equal to</span></span>  
  
|<span data-ttu-id="ec675-201">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-201">Sample Expression</span></span>|<span data-ttu-id="ec675-202">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-202">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-203">>=1.200</span><span class="sxs-lookup"><span data-stu-id="ec675-203">>=1200</span></span>|<span data-ttu-id="ec675-204">Nummers groter dan of gelijk aan 1200</span><span class="sxs-lookup"><span data-stu-id="ec675-204">Numbers greater than or equal to 1200</span></span>|  
  
### <a name="-less-than"></a><span data-ttu-id="ec675-205">(<) Kleiner dan</span><span class="sxs-lookup"><span data-stu-id="ec675-205">(<) Less than</span></span>  
  
|<span data-ttu-id="ec675-206">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-206">Sample Expression</span></span>|<span data-ttu-id="ec675-207">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-207">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-208"><1.200</span><span class="sxs-lookup"><span data-stu-id="ec675-208"><1200</span></span>|<span data-ttu-id="ec675-209">Nummers kleiner dan 1200</span><span class="sxs-lookup"><span data-stu-id="ec675-209">Numbers less than 1200</span></span>|  
  
### <a name="-less-than-or-equal-to"></a><span data-ttu-id="ec675-210">(<=) Kleiner dan of gelijk aan</span><span class="sxs-lookup"><span data-stu-id="ec675-210">(<=) Less than or equal to</span></span>  
  
|<span data-ttu-id="ec675-211">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-211">Sample Expression</span></span>|<span data-ttu-id="ec675-212">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-212">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-213"><=1.200</span><span class="sxs-lookup"><span data-stu-id="ec675-213"><=1200</span></span>|<span data-ttu-id="ec675-214">Nummers kleiner dan of gelijk aan 1200</span><span class="sxs-lookup"><span data-stu-id="ec675-214">Numbers less than or equal to 1200</span></span>|  
  
### <a name="-and"></a><span data-ttu-id="ec675-215">(&) En</span><span class="sxs-lookup"><span data-stu-id="ec675-215">(&) And</span></span>  
  
|<span data-ttu-id="ec675-216">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-216">Sample Expression</span></span>|<span data-ttu-id="ec675-217">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-217">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-218">>200&<1200</span><span class="sxs-lookup"><span data-stu-id="ec675-218">>200&<1200</span></span>|<span data-ttu-id="ec675-219">Getallen groter dan 200 en kleiner dan 1200</span><span class="sxs-lookup"><span data-stu-id="ec675-219">Numbers greater than 200 and less than 1200</span></span>|  
  
### <a name="-an-exact-character-match"></a><span data-ttu-id="ec675-220">('') Een exacte tekenovereenkomst</span><span class="sxs-lookup"><span data-stu-id="ec675-220">('') An exact character match</span></span>  
  
|<span data-ttu-id="ec675-221">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-221">Sample Expression</span></span>|<span data-ttu-id="ec675-222">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-222">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-223">'man'</span><span class="sxs-lookup"><span data-stu-id="ec675-223">'man'</span></span>|<span data-ttu-id="ec675-224">Tekst die exact overeenkomt met man en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="ec675-224">Text that matches man exactly and is case sensitive.</span></span>|  
  
### <a name="-case-insensitive"></a><span data-ttu-id="ec675-225">(@) Niet hoofdlettergevoelig</span><span class="sxs-lookup"><span data-stu-id="ec675-225">(@) Case insensitive</span></span>  
  
|<span data-ttu-id="ec675-226">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-226">Sample Expression</span></span>|<span data-ttu-id="ec675-227">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-227">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-228">@man\*</span><span class="sxs-lookup"><span data-stu-id="ec675-228">@man\*</span></span>|<span data-ttu-id="ec675-229">Tekst die begint met man en niet hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="ec675-229">Text that starts with man and is case insensitive.</span></span>|  
  
### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="ec675-230">(\*) Een onbeperkt aantal onbekende tekens</span><span class="sxs-lookup"><span data-stu-id="ec675-230">(\*) An indefinite number of unknown characters</span></span>  
  
|<span data-ttu-id="ec675-231">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-231">Sample Expression</span></span>|<span data-ttu-id="ec675-232">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-232">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-233">*Co*</span><span class="sxs-lookup"><span data-stu-id="ec675-233">*Co*</span></span>|<span data-ttu-id="ec675-234">Tekst die “Co“ bevat en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="ec675-234">Text that contains "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="ec675-235">\*Be</span><span class="sxs-lookup"><span data-stu-id="ec675-235">\*Co</span></span>|<span data-ttu-id="ec675-236">Tekst die eindigt met “Co“ en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="ec675-236">Text that ends with "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="ec675-237">Be\*</span><span class="sxs-lookup"><span data-stu-id="ec675-237">Co\*</span></span>|<span data-ttu-id="ec675-238">Tekst die begint met “Co“ en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="ec675-238">Text that begins with "Co" and is case sensitive.</span></span>|  
  
### <a name="-one-unknown-character"></a><span data-ttu-id="ec675-239">(?) Een onbekend teken</span><span class="sxs-lookup"><span data-stu-id="ec675-239">(?) One unknown character</span></span>  
  
|<span data-ttu-id="ec675-240">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-240">Sample Expression</span></span>|<span data-ttu-id="ec675-241">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-241">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-242">Jans?n</span><span class="sxs-lookup"><span data-stu-id="ec675-242">Hans?n</span></span>|<span data-ttu-id="ec675-243">Tekst zoals Jansen of Jansma</span><span class="sxs-lookup"><span data-stu-id="ec675-243">Text such as Hansen or Hanson</span></span>|  
  
### <a name="combined-format-expressions"></a><span data-ttu-id="ec675-244">Gecombineerde notatiesoorten</span><span class="sxs-lookup"><span data-stu-id="ec675-244">Combined format expressions</span></span>  
  
|<span data-ttu-id="ec675-245">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="ec675-245">Sample Expression</span></span>|<span data-ttu-id="ec675-246">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="ec675-246">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="ec675-247">5999&#124;8100..8490</span><span class="sxs-lookup"><span data-stu-id="ec675-247">5999&#124;8100..8490</span></span>|<span data-ttu-id="ec675-248">Alle records met het nummer 5999 of een nummer uit het interval 8100 tot en met 8490.</span><span class="sxs-lookup"><span data-stu-id="ec675-248">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|<span data-ttu-id="ec675-249">..1299&#124;1400..</span><span class="sxs-lookup"><span data-stu-id="ec675-249">..1299&#124;1400..</span></span>|<span data-ttu-id="ec675-250">Records met een nummer kleiner dan of gelijk aan 1299 of gelijk aan 1400 en hoger. Met andere woorden: alle nummers behalve 1300 tot en met 1399.</span><span class="sxs-lookup"><span data-stu-id="ec675-250">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|<span data-ttu-id="ec675-251">>50&<100</span><span class="sxs-lookup"><span data-stu-id="ec675-251">>50&<100</span></span>|<span data-ttu-id="ec675-252">Records met een nummer groter dan 50 en kleiner dan 100, ofwel nummer 51 tot en met 99.</span><span class="sxs-lookup"><span data-stu-id="ec675-252">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  
 
## <a name="see-also"></a><span data-ttu-id="ec675-253">Zie ook</span><span class="sxs-lookup"><span data-stu-id="ec675-253">See Also</span></span>
<span data-ttu-id="ec675-254">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="ec675-254">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
