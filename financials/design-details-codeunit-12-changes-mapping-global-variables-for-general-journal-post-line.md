---
title: 'Ontwerpdetails - Wijzigingen in codeunit 12: Toewijzing algemene variabelen voor dagboekboekingsregel | Microsoft Docs'
description: "De volgende wijzigingen zijn geïmplementeerd in deze versie van [!INCLUDE[d365fin](includes/d365fin_md.md)]."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: f2c15ecfe98bbbbb8154f46032201221ca32e32e
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="codeunit-12-changes-mapping-global-variables-for-general-journal-post-line"></a><span data-ttu-id="724d7-103">Wijzigingen in codeunit 12: Toewijzing algemene variabelen voor dagboekboekingsregel</span><span class="sxs-lookup"><span data-stu-id="724d7-103">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>
<span data-ttu-id="724d7-104">De volgende wijzigingen zijn geïmplementeerd in deze versie van [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="724d7-104">The following changes have been implemented in this release of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

|<span data-ttu-id="724d7-105">**Microsoft Dynamics NAV 2009 R2**</span><span class="sxs-lookup"><span data-stu-id="724d7-105">**Microsoft Dynamics NAV 2009 R2**</span></span>|<span data-ttu-id="724d7-106">**Microsoft Dynamics NAV 2013 R2**</span><span class="sxs-lookup"><span data-stu-id="724d7-106">**Microsoft Dynamics NAV 2013 R2**</span></span>|<span data-ttu-id="724d7-107">**Opmerking**</span><span class="sxs-lookup"><span data-stu-id="724d7-107">**Comment**</span></span>|  
|----------------------------------------|----------------------------------------|-----------------|  
|<span data-ttu-id="724d7-108">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="724d7-108">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="724d7-109">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="724d7-109">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="724d7-110">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-110">Unchanged</span></span>|  
|<span data-ttu-id="724d7-111">SalesSetup@1010 : Record 311;</span><span class="sxs-lookup"><span data-stu-id="724d7-111">SalesSetup@1010 : Record 311;</span></span>||<span data-ttu-id="724d7-112">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-112">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-113">PurchSetup@1011 : Record 312;</span><span class="sxs-lookup"><span data-stu-id="724d7-113">PurchSetup@1011 : Record 312;</span></span>||<span data-ttu-id="724d7-114">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-114">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-115">AccountingPeriod@1012 : Record 50;</span><span class="sxs-lookup"><span data-stu-id="724d7-115">AccountingPeriod@1012 : Record 50;</span></span>||<span data-ttu-id="724d7-116">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-116">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-117">GLAcc@1013 : Record 15;</span><span class="sxs-lookup"><span data-stu-id="724d7-117">GLAcc@1013 : Record 15;</span></span>||<span data-ttu-id="724d7-118">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-118">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-119">GLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-119">GLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="724d7-120">GlobalGLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-120">GlobalGLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="724d7-121">Naam gewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-121">Renamed</span></span>|  
|<span data-ttu-id="724d7-122">GLEntryTmp@1015 : TIJDELIJKE record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="724d7-123">TempGLEntryBuf@1010 : TIJDELIJKE record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="724d7-124">Naam gewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-124">Renamed</span></span>|  
|<span data-ttu-id="724d7-125">TempGLEntryVAT@1016 : TIJDELIJKE record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="724d7-126">TempGLEntryVAT@1016 : TIJDELIJKE record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="724d7-127">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-127">Unchanged</span></span>|  
|<span data-ttu-id="724d7-128">OrigGLEntry@1017 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-128">OrigGLEntry@1017 : Record 17;</span></span>||<span data-ttu-id="724d7-129">Verwijderd</span><span class="sxs-lookup"><span data-stu-id="724d7-129">Deleted</span></span>|  
|<span data-ttu-id="724d7-130">VATPostingSetup@1019 : Record 325;</span><span class="sxs-lookup"><span data-stu-id="724d7-130">VATPostingSetup@1019 : Record 325;</span></span>||<span data-ttu-id="724d7-131">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-131">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-132">Cust@1020 : Record 18;</span><span class="sxs-lookup"><span data-stu-id="724d7-132">Cust@1020 : Record 18;</span></span>||<span data-ttu-id="724d7-133">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-133">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-134">Vend@1021 : Record 23;</span><span class="sxs-lookup"><span data-stu-id="724d7-134">Vend@1021 : Record 23;</span></span>||<span data-ttu-id="724d7-135">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-135">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-136">GenJnlLine@1022 : Record 81;</span><span class="sxs-lookup"><span data-stu-id="724d7-136">GenJnlLine@1022 : Record 81;</span></span>||<span data-ttu-id="724d7-137">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-137">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-138">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="724d7-138">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="724d7-139">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="724d7-139">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="724d7-140">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-140">Unchanged</span></span>|  
|<span data-ttu-id="724d7-141">CustPostingGr@1030 : Record 92;</span><span class="sxs-lookup"><span data-stu-id="724d7-141">CustPostingGr@1030 : Record 92;</span></span>||<span data-ttu-id="724d7-142">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-142">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-143">VendPostingGr@1031 : Record 93;</span><span class="sxs-lookup"><span data-stu-id="724d7-143">VendPostingGr@1031 : Record 93;</span></span>||<span data-ttu-id="724d7-144">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-144">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-145">Currency@1032 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="724d7-145">Currency@1032 : Record 4;</span></span>||<span data-ttu-id="724d7-146">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-146">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-147">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="724d7-147">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="724d7-148">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="724d7-148">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="724d7-149">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-149">Unchanged</span></span>|  
|<span data-ttu-id="724d7-150">ApplnCurrency@1034 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="724d7-150">ApplnCurrency@1034 : Record 4;</span></span>||<span data-ttu-id="724d7-151">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-151">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-152">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="724d7-152">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="724d7-153">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="724d7-153">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="724d7-154">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-154">Unchanged</span></span>|  
|<span data-ttu-id="724d7-155">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="724d7-155">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="724d7-156">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="724d7-156">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="724d7-157">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-157">Unchanged</span></span>|  
|<span data-ttu-id="724d7-158">BankAcc@1039 : Record 270;</span><span class="sxs-lookup"><span data-stu-id="724d7-158">BankAcc@1039 : Record 270;</span></span>||<span data-ttu-id="724d7-159">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-159">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-160">BankAccLedgEntry@1040 : Record 271;</span><span class="sxs-lookup"><span data-stu-id="724d7-160">BankAccLedgEntry@1040 : Record 271;</span></span>||<span data-ttu-id="724d7-161">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-161">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-162">CheckLedgEntry@1041 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="724d7-162">CheckLedgEntry@1041 : Record 272;</span></span>||<span data-ttu-id="724d7-163">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-163">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-164">CheckLedgEntry2@1042 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="724d7-164">CheckLedgEntry2@1042 : Record 272;</span></span>||<span data-ttu-id="724d7-165">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-165">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-166">BankAccPostingGr@1043 : Record 277;</span><span class="sxs-lookup"><span data-stu-id="724d7-166">BankAccPostingGr@1043 : Record 277;</span></span>||<span data-ttu-id="724d7-167">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-167">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-168">GenJnlTemplate@1044 : Record 80;</span><span class="sxs-lookup"><span data-stu-id="724d7-168">GenJnlTemplate@1044 : Record 80;</span></span>||<span data-ttu-id="724d7-169">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-169">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-170">TaxJurisdiction@1045 : Record 320;</span><span class="sxs-lookup"><span data-stu-id="724d7-170">TaxJurisdiction@1045 : Record 320;</span></span>||<span data-ttu-id="724d7-171">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-171">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-172">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="724d7-172">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="724d7-173">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="724d7-173">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="724d7-174">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-174">Unchanged</span></span>|  
|<span data-ttu-id="724d7-175">FAGLPostBuf@1047 : TIJDELIJKE record 5637;</span><span class="sxs-lookup"><span data-stu-id="724d7-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span></span>||<span data-ttu-id="724d7-176">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-176">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-177">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="724d7-177">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="724d7-178">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="724d7-178">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="724d7-179">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-179">Unchanged</span></span>|  
|<span data-ttu-id="724d7-180">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="724d7-180">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="724d7-181">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="724d7-181">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="724d7-182">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-182">Unchanged</span></span>|  
|<span data-ttu-id="724d7-183">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="724d7-183">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="724d7-184">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="724d7-184">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="724d7-185">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-185">Unchanged</span></span>|  
|<span data-ttu-id="724d7-186">TempVATEntry@1088 : TIJDELIJKE record 254;</span><span class="sxs-lookup"><span data-stu-id="724d7-186">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="724d7-187">TempVATEntry@1088 : TIJDELIJKE record 254;</span><span class="sxs-lookup"><span data-stu-id="724d7-187">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="724d7-188">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-188">Unchanged</span></span>|  
|<span data-ttu-id="724d7-189">ReversedGLEntryTemp@1089 : TIJDELIJKE Record 17;</span><span class="sxs-lookup"><span data-stu-id="724d7-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span></span>||<span data-ttu-id="724d7-190">Verplaatst naar Codeunit17</span><span class="sxs-lookup"><span data-stu-id="724d7-190">Moved to Codeunit17</span></span>|  
|<span data-ttu-id="724d7-191">CostAccSetup@1092 : Record 1108;</span><span class="sxs-lookup"><span data-stu-id="724d7-191">CostAccSetup@1092 : Record 1108;</span></span>||<span data-ttu-id="724d7-192">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-192">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-193">GenJnlCheckLine@1048 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="724d7-193">GenJnlCheckLine@1048 : Codeunit 11;</span></span>|<span data-ttu-id="724d7-194">GenJnlCheckLine@1001 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="724d7-194">GenJnlCheckLine@1001 : Codeunit 11;</span></span>|<span data-ttu-id="724d7-195">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-195">Unchanged</span></span>|  
|<span data-ttu-id="724d7-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span><span class="sxs-lookup"><span data-stu-id="724d7-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span></span>||<span data-ttu-id="724d7-197">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-197">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-198">FAJnlPostLine@1050 : Codeunit 5632;</span><span class="sxs-lookup"><span data-stu-id="724d7-198">FAJnlPostLine@1050 : Codeunit 5632;</span></span>||<span data-ttu-id="724d7-199">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-199">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-200">SalesTaxCalculate@1051 : Codeunit 398;</span><span class="sxs-lookup"><span data-stu-id="724d7-200">SalesTaxCalculate@1051 : Codeunit 398;</span></span>||<span data-ttu-id="724d7-201">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-201">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-202">GenJnlApply@1052 : Codeunit 225;</span><span class="sxs-lookup"><span data-stu-id="724d7-202">GenJnlApply@1052 : Codeunit 225;</span></span>||<span data-ttu-id="724d7-203">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-203">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-204">DimMgt@1053 : Codeunit 408;</span><span class="sxs-lookup"><span data-stu-id="724d7-204">DimMgt@1053 : Codeunit 408;</span></span>||<span data-ttu-id="724d7-205">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-205">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-206">JobPostLine@1028 : Codeunit 1001;</span><span class="sxs-lookup"><span data-stu-id="724d7-206">JobPostLine@1028 : Codeunit 1001;</span></span>||<span data-ttu-id="724d7-207">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-207">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span><span class="sxs-lookup"><span data-stu-id="724d7-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span></span>||<span data-ttu-id="724d7-209">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-209">Changed to Local</span></span>|  
||<span data-ttu-id="724d7-210">PaymentToleranceMgt@1002 : Codeunit 426;</span><span class="sxs-lookup"><span data-stu-id="724d7-210">PaymentToleranceMgt@1002 : Codeunit 426;</span></span>|<span data-ttu-id="724d7-211">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="724d7-211">Added</span></span>|  
||<span data-ttu-id="724d7-212">AddCurrencyCode@1117 : Code[10];</span><span class="sxs-lookup"><span data-stu-id="724d7-212">AddCurrencyCode@1117 : Code[10];</span></span>|<span data-ttu-id="724d7-213">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="724d7-213">Added</span></span>|  
|<span data-ttu-id="724d7-214">FiscalYearStartDate@1054 : Datum;</span><span class="sxs-lookup"><span data-stu-id="724d7-214">FiscalYearStartDate@1054 : Date;</span></span>|<span data-ttu-id="724d7-215">FiscalYearStartDate@1011 : Datum;</span><span class="sxs-lookup"><span data-stu-id="724d7-215">FiscalYearStartDate@1011 : Date;</span></span>|<span data-ttu-id="724d7-216">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-216">Unchanged</span></span>|  
|<span data-ttu-id="724d7-217">NextEntryNo@1055 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-217">NextEntryNo@1055 : Integer;</span></span>|<span data-ttu-id="724d7-218">NextEntryNo@1022 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-218">NextEntryNo@1022 : Integer;</span></span>|<span data-ttu-id="724d7-219">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-219">Unchanged</span></span>|  
|<span data-ttu-id="724d7-220">BalanceCheckAmount@1056 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-220">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="724d7-221">BalanceCheckAmount@1056 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-221">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="724d7-222">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-222">Unchanged</span></span>|  
|<span data-ttu-id="724d7-223">BalanceCheckAmount2@1057 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-223">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="724d7-224">BalanceCheckAmount2@1057 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-224">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="724d7-225">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-225">Unchanged</span></span>|  
|<span data-ttu-id="724d7-226">BalanceCheckAddCurrAmount@1058 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="724d7-227">BalanceCheckAddCurrAmount@1058 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="724d7-228">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-228">Unchanged</span></span>|  
|<span data-ttu-id="724d7-229">BalanceCheckAddCurrAmount2@1059 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="724d7-230">BalanceCheckAddCurrAmount2@1059 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="724d7-231">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-231">Unchanged</span></span>|  
|<span data-ttu-id="724d7-232">CurrentBalance@1060 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-232">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="724d7-233">CurrentBalance@1060 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-233">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="724d7-234">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-234">Unchanged</span></span>|  
|<span data-ttu-id="724d7-235">SalesTaxBaseAmount@1061 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-235">SalesTaxBaseAmount@1061 : Decimal;</span></span>||<span data-ttu-id="724d7-236">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-236">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-237">TotalAddCurrAmount@1062 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-237">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="724d7-238">TotalAddCurrAmount@1062 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-238">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="724d7-239">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-239">Unchanged</span></span>|  
|<span data-ttu-id="724d7-240">TotalAmount@1063 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-240">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="724d7-241">TotalAmount@1063 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-241">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="724d7-242">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-242">Unchanged</span></span>|  
|<span data-ttu-id="724d7-243">UnrealizedRemainingAmountCust@1086 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="724d7-244">UnrealizedRemainingAmountCust@1086 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="724d7-245">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-245">Unchanged</span></span>|  
|<span data-ttu-id="724d7-246">UnrealizedRemainingAmountVend@1074 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="724d7-247">UnrealizedRemainingAmountVend@1074 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="724d7-248">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-248">Unchanged</span></span>|  
|<span data-ttu-id="724d7-249">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-249">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="724d7-250">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-250">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="724d7-251">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-251">Unchanged</span></span>|  
|<span data-ttu-id="724d7-252">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-252">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="724d7-253">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-253">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="724d7-254">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-254">Unchanged</span></span>|  
|<span data-ttu-id="724d7-255">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-255">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="724d7-256">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-256">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="724d7-257">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-257">Unchanged</span></span>|  
|<span data-ttu-id="724d7-258">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-258">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="724d7-259">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-259">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="724d7-260">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-260">Unchanged</span></span>|  
|<span data-ttu-id="724d7-261">InsertedTempGLEntryVAT@1068 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-261">InsertedTempGLEntryVAT@1068 : Integer;</span></span>|<span data-ttu-id="724d7-262">InsertedTempGLEntryVAT@1027 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-262">InsertedTempGLEntryVAT@1027 : Integer;</span></span>|<span data-ttu-id="724d7-263">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-263">Unchanged</span></span>|  
|<span data-ttu-id="724d7-264">LastDocNo@1069 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="724d7-264">LastDocNo@1069 : Code[20];</span></span>|<span data-ttu-id="724d7-265">LastDocNo@1023 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="724d7-265">LastDocNo@1023 : Code[20];</span></span>|<span data-ttu-id="724d7-266">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-266">Unchanged</span></span>|  
|<span data-ttu-id="724d7-267">LastLineNo@1070 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-267">LastLineNo@1070 : Integer;</span></span>||<span data-ttu-id="724d7-268">Verwijderd</span><span class="sxs-lookup"><span data-stu-id="724d7-268">Deleted</span></span>|  
|<span data-ttu-id="724d7-269">LastDate@1071 : Datum;</span><span class="sxs-lookup"><span data-stu-id="724d7-269">LastDate@1071 : Date;</span></span>|<span data-ttu-id="724d7-270">LastDate@1021 : Datum;</span><span class="sxs-lookup"><span data-stu-id="724d7-270">LastDate@1021 : Date;</span></span>|<span data-ttu-id="724d7-271">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-271">Unchanged</span></span>|  
|<span data-ttu-id="724d7-272">LastDocType@1072 : ' ,Betaling,Factuur,Creditnota,Rentefactuur,Aanmaning';</span><span class="sxs-lookup"><span data-stu-id="724d7-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="724d7-273">LastDocType@1025 : ' ,Betaling,Factuur,Creditnota,Rentefactuur,Aanmaning';</span><span class="sxs-lookup"><span data-stu-id="724d7-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="724d7-274">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-274">Unchanged</span></span>|  
|<span data-ttu-id="724d7-275">NextCheckEntryNo@1073 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-275">NextCheckEntryNo@1073 : Integer;</span></span>|<span data-ttu-id="724d7-276">NextCheckEntryNo@1028 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-276">NextCheckEntryNo@1028 : Integer;</span></span>|<span data-ttu-id="724d7-277">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-277">Unchanged</span></span>|  
|<span data-ttu-id="724d7-278">AddCurrGLEntryVATAmt@1075 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span></span>|<span data-ttu-id="724d7-279">AddCurrGLEntryVATAmt@1017 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span></span>|<span data-ttu-id="724d7-280">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-280">Unchanged</span></span>|  
|<span data-ttu-id="724d7-281">CurrencyDate@1076 : Datum;</span><span class="sxs-lookup"><span data-stu-id="724d7-281">CurrencyDate@1076 : Date;</span></span>|<span data-ttu-id="724d7-282">CurrencyDate@1020 : Datum;</span><span class="sxs-lookup"><span data-stu-id="724d7-282">CurrencyDate@1020 : Date;</span></span>|<span data-ttu-id="724d7-283">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-283">Unchanged</span></span>|  
|<span data-ttu-id="724d7-284">CurrencyFactor@1077 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-284">CurrencyFactor@1077 : Decimal;</span></span>|<span data-ttu-id="724d7-285">CurrencyFactor@1019 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-285">CurrencyFactor@1019 : Decimal;</span></span>|<span data-ttu-id="724d7-286">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-286">Unchanged</span></span>|  
|<span data-ttu-id="724d7-287">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-287">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="724d7-288">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-288">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="724d7-289">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-289">Unchanged</span></span>|  
|<span data-ttu-id="724d7-290">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-290">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="724d7-291">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-291">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="724d7-292">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-292">Unchanged</span></span>|  
|<span data-ttu-id="724d7-293">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-293">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="724d7-294">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-294">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="724d7-295">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-295">Unchanged</span></span>|  
|<span data-ttu-id="724d7-296">AllApplied@1081 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-296">AllApplied@1081 : Boolean;</span></span>||<span data-ttu-id="724d7-297">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="724d7-297">Changed to Local</span></span>|  
|<span data-ttu-id="724d7-298">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-298">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="724d7-299">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-299">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="724d7-300">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-300">Unchanged</span></span>|  
|<span data-ttu-id="724d7-301">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-301">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="724d7-302">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-302">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="724d7-303">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-303">Unchanged</span></span>|  
|<span data-ttu-id="724d7-304">Prepayment@1037 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-304">Prepayment@1037 : Boolean;</span></span>||<span data-ttu-id="724d7-305">Verwijderd</span><span class="sxs-lookup"><span data-stu-id="724d7-305">Deleted</span></span>|  
|<span data-ttu-id="724d7-306">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-306">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="724d7-307">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-307">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="724d7-308">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-308">Unchanged</span></span>|  
|<span data-ttu-id="724d7-309">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-309">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="724d7-310">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-310">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="724d7-311">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-311">Unchanged</span></span>|  
|<span data-ttu-id="724d7-312">GLEntryNo@1090 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-312">GLEntryNo@1090 : Integer;</span></span>|<span data-ttu-id="724d7-313">GLEntryNo@1026 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-313">GLEntryNo@1026 : Integer;</span></span>|<span data-ttu-id="724d7-314">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="724d7-314">Unchanged</span></span>|  
||<span data-ttu-id="724d7-315">GLSetupRead@1015 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="724d7-315">GLSetupRead@1015 : Boolean;</span></span>|<span data-ttu-id="724d7-316">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="724d7-316">Added</span></span>|  
||<span data-ttu-id="724d7-317">AmountRoundingPrecision@1012 : Decimaal;</span><span class="sxs-lookup"><span data-stu-id="724d7-317">AmountRoundingPrecision@1012 : Decimal;</span></span>|<span data-ttu-id="724d7-318">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="724d7-318">Added</span></span>|  
||<span data-ttu-id="724d7-319">CrCardTransactionEntryNo@1013 : Integer;</span><span class="sxs-lookup"><span data-stu-id="724d7-319">CrCardTransactionEntryNo@1013 : Integer;</span></span>|<span data-ttu-id="724d7-320">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="724d7-320">Added</span></span>|  

## <a name="see-also"></a><span data-ttu-id="724d7-321">Zie ook</span><span class="sxs-lookup"><span data-stu-id="724d7-321">See Also</span></span>  
 [<span data-ttu-id="724d7-322">Designdetails: Wijzigingen in codeunit 12: Wijzigingen in procedures voor grootboekboekingen</span><span class="sxs-lookup"><span data-stu-id="724d7-322">Design Details: Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)
