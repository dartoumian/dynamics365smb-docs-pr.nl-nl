---
title: De extensie van de Afbeeldingsanalyse gebruiken | Microsoft Docs
description: Met deze extensie kunt u afbeeldingen analyseren van contactpersonen en artikelen om kenmerken te zoeken, zodat u deze snel kunt toewijzen in Business Central.
documentationcenter: 
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: API, extension, Cognitive Services, image, computer vision, attribute, tag, recognition
ms.date: 06/19/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: e075aedde1bd52a6b852fd92e419aca11367b742
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---

# <a name="the-image-analyzer-extension-for-microsoft-business-central"></a><span data-ttu-id="78250-103">De extensie Afbeeldingsanalyse voor Microsoft Business Central</span><span class="sxs-lookup"><span data-stu-id="78250-103">The Image Analyzer Extension for Microsoft Business Central</span></span>
<span data-ttu-id="78250-104">De extensie Afbeeldingsanalyse gebruikt krachtige afbeeldingsanalyse die wordt verschaft door de Computer Vision-API voor Cognitieve services van Microsoft om kenmerken te detecteren in de afbeeldingen die u importeert voor artikelen en contactpersonen, zodat u deze gemakkelijk kunt bekijken en toewijzen.</span><span class="sxs-lookup"><span data-stu-id="78250-104">The Image Analyzer extension uses powerful image analytics provided by the Computer Vision API for Microsoft Cognitive Services to detect attributes in the images that you import for items and contact persons, so you can easily review and assign them.</span></span> <span data-ttu-id="78250-105">Voor artikelen kunnen kenmerken bijvoorbeeld zijn of het artikel een tafel of een auto is en of het rood of blauw is.</span><span class="sxs-lookup"><span data-stu-id="78250-105">For items, attributes could be whether the item is a table or a car, and whether it is red or blue.</span></span> <span data-ttu-id="78250-106">Voor contactpersonen kunnen kenmerken geslacht of leeftijd zijn.</span><span class="sxs-lookup"><span data-stu-id="78250-106">For contact persons, attributes can be gender or age.</span></span>

<span data-ttu-id="78250-107">Afbeeldingsanalyse stelt kenmerken voor op basis van tags die de Computer Vision-API vindt, en een vertrouwensniveau.</span><span class="sxs-lookup"><span data-stu-id="78250-107">Image Analyzer suggests attributes based on tags that the Computer Vision API finds, and a confidence level.</span></span> <span data-ttu-id="78250-108">Standaard worden alleen kenmerken voorgesteld als het ten minste 80% zeker is dat het kenmerk klopt.</span><span class="sxs-lookup"><span data-stu-id="78250-108">By default, it suggests attributes only if it is at least 80% sure that the attribute is correct.</span></span> <span data-ttu-id="78250-109">U kunt een ander vertrouwensniveau instellen, indien nodig.</span><span class="sxs-lookup"><span data-stu-id="78250-109">You can set another confidence level, if needed.</span></span> <span data-ttu-id="78250-110">Als u meer wilt weten over hoe de tags en vertrouwensniveaus worden bepaald, raadpleegt u [Computer Vision-API](https://go.microsoft.com/fwlink/?linkid=851476)</span><span class="sxs-lookup"><span data-stu-id="78250-110">To learn more about how the tags and confidence level are determined, see [Computer Vision API](https://go.microsoft.com/fwlink/?linkid=851476).</span></span>  

<span data-ttu-id="78250-111">De Afbeeldingsanalyse is gratis in [!INCLUDE[d365fin](includes/d365fin_md.md)], maar er is een limiet van het aantal artikelen dat u tijdens een periode kunt analyseren.</span><span class="sxs-lookup"><span data-stu-id="78250-111">Image Analyzer is free in [!INCLUDE[d365fin](includes/d365fin_md.md)], but there is a limit to the number of items that you can analyze during a certain period of time.</span></span> <span data-ttu-id="78250-112">Standaard kunt u 100 afbeeldingen per maand analyseren.</span><span class="sxs-lookup"><span data-stu-id="78250-112">By default, you can analyze 100 images per month.</span></span>

<span data-ttu-id="78250-113">Nadat u de extensie hebt ingeschakeld, wordt de Afbeeldingsanalyse steeds uitgevoerd wanneer u een afbeelding of contactpersoon importeert.</span><span class="sxs-lookup"><span data-stu-id="78250-113">After you enable the extension, Image Analyzer runs each time you import an image to an item or contact person.</span></span> <span data-ttu-id="78250-114">U ziet direct de kenmerken, het vertrouwensniveau en de details en kunt besluiten wat er met elk kenmerk moet gebeuren.</span><span class="sxs-lookup"><span data-stu-id="78250-114">You will see the attributes, confidence level, and details right away, and can decide what to do with each attribute.</span></span> <span data-ttu-id="78250-115">Als u afbeeldingen hebt geïmporteerd voordat u de Afbeeldingsanalyse hebt ingeschakeld, moet u naar de artikel- of contactpersoonkaarten gaan en de actie **Afbeelding analyseren** kiezen.</span><span class="sxs-lookup"><span data-stu-id="78250-115">If you imported images before you enabled the Image Analyzer extension, you must go to the item or contact cards and choose the **Analyze Picture** action.</span></span>  

>   [!NOTE]  
>   <span data-ttu-id="78250-116">Door deze extensie in te schakelen gaat u ermee akkoord dat Microsoft uw gegevens mag opslaan en gebruiken om Microsoft-services te verbeteren, bijvoorbeeld om de Computer Vision API beter te maken.</span><span class="sxs-lookup"><span data-stu-id="78250-116">By enabling this extension you agree that Microsoft may store your data and use it to improve Microsoft services, such as making the Computer Vision API better.</span></span> <span data-ttu-id="78250-117">Om te helpen uw privacy te beschermen nemen we stappen om uw gegevens anoniem en veilig te maken.</span><span class="sxs-lookup"><span data-stu-id="78250-117">To help protect your privacy, we take steps to make your data anonymous and keep it secure.</span></span> <span data-ttu-id="78250-118">We publiceren uw gegevens niet en laten anderen deze niet gebruiken.</span><span class="sxs-lookup"><span data-stu-id="78250-118">We will not publish your data or let other people use it.</span></span> <span data-ttu-id="78250-119">U kunt de afbeelding van het artikel in [!INCLUDE[d365fin](includes/d365fin_md.md)] verwijderen, maar de Computer Vision API bevat het dan nog in de niet-geïdentificeerde vorm.</span><span class="sxs-lookup"><span data-stu-id="78250-119">You can remove the image from the item in [!INCLUDE[d365fin](includes/d365fin_md.md)], however, the Computer Vision API will still have the image in its de-identified form.</span></span> <span data-ttu-id="78250-120">Zie voor meer informatie [Microsoft Vertrouwenscentrum](https://go.microsoft.com/fwlink/?linkid=851463).</span><span class="sxs-lookup"><span data-stu-id="78250-120">For more information, see [Microsoft Trust Center](https://go.microsoft.com/fwlink/?linkid=851463).</span></span>

## <a name="requirements"></a><span data-ttu-id="78250-121">Vereisten</span><span class="sxs-lookup"><span data-stu-id="78250-121">Requirements</span></span>
<span data-ttu-id="78250-122">Er zijn enkele vereisten voor de afbeeldingen:</span><span class="sxs-lookup"><span data-stu-id="78250-122">There are a few requirements for the images:</span></span>

* <span data-ttu-id="78250-123">Afbeeldingsindelingen: JPEG, PNG, GIF, BMP</span><span class="sxs-lookup"><span data-stu-id="78250-123">Image formats: JPEG, PNG, GIF, BMP</span></span>  
* <span data-ttu-id="78250-124">Maximale bestandsgrootte: minder dan 4 MB</span><span class="sxs-lookup"><span data-stu-id="78250-124">Maximum file size: Less than 4 MB</span></span>  
* <span data-ttu-id="78250-125">Afbeeldingdimensies: groter dan 50 x 50 pixels</span><span class="sxs-lookup"><span data-stu-id="78250-125">Image dimensions: Greater than 50 x 50 pixels</span></span>  

## <a name="blacklisting-suggested-attributes"></a><span data-ttu-id="78250-126">Op zwarte lijst plaatsen van voorgestelde kenmerken</span><span class="sxs-lookup"><span data-stu-id="78250-126">Blacklisting suggested attributes</span></span>
<span data-ttu-id="78250-127">Als de analyse een kenmerk voorstelt dat u niet wilt zien, kunt u het op de zwarte lijst plaatsen.</span><span class="sxs-lookup"><span data-stu-id="78250-127">If the analysis suggests an attribute that you do not want to see you can blacklist the attribute.</span></span> <span data-ttu-id="78250-128">Wees echter voorzichtig.</span><span class="sxs-lookup"><span data-stu-id="78250-128">Use caution, however.</span></span> <span data-ttu-id="78250-129">Kenmerken op de zwarte lijst worden ook niet voorgesteld voor andere artikelen of contactpersonen.</span><span class="sxs-lookup"><span data-stu-id="78250-129">Blacklisted attributes are not suggested for other items or contact persons either.</span></span> <span data-ttu-id="78250-130">Als u betreurt dat een kenmerk op de zwarte lijst staat, kunt u **Op de zwarte lijst gezette kenmerken** kiezen en het kenmerk van de lijst verwijderen.</span><span class="sxs-lookup"><span data-stu-id="78250-130">If you regret blacklisting an attribute, you can choose **Blacklisted Attributes**, and then delete the attribute from the list.</span></span>

## <a name="to-enable-image-analyzer"></a><span data-ttu-id="78250-131">Afbeeldingsanalyse inschakelen</span><span class="sxs-lookup"><span data-stu-id="78250-131">To enable Image Analyzer</span></span>
<span data-ttu-id="78250-132">De extensie Afbeeldingsanalyse is ingebouwd in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="78250-132">The Image Analyzer extension is built-in to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="78250-133">U hoeft het alleen in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="78250-133">You just need to turn it on.</span></span>

> [!NOTE]  
> <span data-ttu-id="78250-134">Als u de extensie Afbeeldinganalyse wilt inschakelen, moet u een beheerder zijn.</span><span class="sxs-lookup"><span data-stu-id="78250-134">To enable the Image Analyzer extension, you must be an administrator.</span></span> <span data-ttu-id="78250-135">Zorg ervoor dat aan u de machtigingenset **SUPER** is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="78250-135">Make sure that you are assigned the **SUPER** user permission set.</span></span>

1. <span data-ttu-id="78250-136">Als u de extensie Afbeeldingsanalyse wilt inschakelen, voert u een van de volgende handelingen uit:</span><span class="sxs-lookup"><span data-stu-id="78250-136">To enable the Image Analyzer extension, do one of the following:</span></span>

* <span data-ttu-id="78250-137">Open een artikel- of contactkaart.</span><span class="sxs-lookup"><span data-stu-id="78250-137">Open an item or contact card.</span></span> <span data-ttu-id="78250-138">Kies op de berichtbalk **Afbeeldingen analyseren** en volg vervolgens de stappen in de begeleide instelling.</span><span class="sxs-lookup"><span data-stu-id="78250-138">In the notification bar, choose **Analyze Images**, and then follow the steps in the assisted setup guide.</span></span>  
* <span data-ttu-id="78250-139">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Serviceverbindingen** in en kies vervolgens **Afbeeldingsanalyse**.</span><span class="sxs-lookup"><span data-stu-id="78250-139">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Connections**, and then choose **Image Analysis Setup**.</span></span> <span data-ttu-id="78250-140">Kies het selectievakje **Afbeeldingsanalyse inschakelen** en volg vervolgens de stappen in de begeleide instelling.</span><span class="sxs-lookup"><span data-stu-id="78250-140">Choose the **Enable Image Analyzer** check box, and then complete the steps in the assisted setup guide.</span></span>  

>   [!TIP]  
>   <span data-ttu-id="78250-141">De pagina **Instelling van afbeeldingsanalyse** is ook waar u de mate van vertrouwen voor kenmerksuggesties kunt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="78250-141">The **Image Analysis Setup** page is also where you can change the degree of confidence for attribute suggestions.</span></span> <span data-ttu-id="78250-142">Als u bijvoorbeeld een grotere mate van vertrouwen wilt vereisen, kunt u een hoger percentage invoeren.</span><span class="sxs-lookup"><span data-stu-id="78250-142">For example, if you want to require a greater degree of confidence, you can enter a higher percentage.</span></span>

## <a name="to-analyze-an-image-of-an-item"></a><span data-ttu-id="78250-143">Een afbeelding van een artikel analyseren</span><span class="sxs-lookup"><span data-stu-id="78250-143">To analyze an image of an item</span></span>
<span data-ttu-id="78250-144">In de volgende stappen wordt beschreven hoe u een afbeelding analyseert die is geïmporteerd voordat u de extensie Afbeeldingsanalyse hebt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="78250-144">The following steps describe how to analyze an image that was imported before you enabled the Image Analyzer extension.</span></span>  

1. <span data-ttu-id="78250-145">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Artikelen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="78250-145">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Items**, and then choose the related link.</span></span>  
2. <span data-ttu-id="78250-146">Kies het artikel en kies vervolgens de actie **Afbeelding analyseren**.</span><span class="sxs-lookup"><span data-stu-id="78250-146">Choose the item, and then choose the **Analyze Picture** action.</span></span>  
3. <span data-ttu-id="78250-147">De pagina **Kenmerken van afbeeldinganalyse** bevat de ontdekte kenmerken, het vertrouwensniveau en andere informatie over het kenmerk.</span><span class="sxs-lookup"><span data-stu-id="78250-147">The **Image Analyzer Attributes** page displays the detected attributes, the confidence level, and other details about the attribute.</span></span> <span data-ttu-id="78250-148">Gebruik de opties **Uit te voeren acties** om aan te geven wat er met het kenmerk moet gebeuren.</span><span class="sxs-lookup"><span data-stu-id="78250-148">Use the **Action to perform** options to specify what to do with the attribute.</span></span>  

>   [!TIP]  
>   <span data-ttu-id="78250-149">U kunt de naam van het kenmerk toevoegen aan de artikelomschrijving door **Toevoegen aan artikelomschrijving** te kiezen.</span><span class="sxs-lookup"><span data-stu-id="78250-149">You can add the name of the attribute to the item description by choosing **Add to item description**.</span></span> <span data-ttu-id="78250-150">Bijvoorbeeld, het kan handig zijn om snel details toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="78250-150">For example, this can be useful for quickly adding detail.</span></span>  

## <a name="to-analyze-a-picture-of-a-contact-person"></a><span data-ttu-id="78250-151">Een afbeelding van een contactpersoon analyseren</span><span class="sxs-lookup"><span data-stu-id="78250-151">To analyze a picture of a contact person</span></span>
<span data-ttu-id="78250-152">In de volgende stappen wordt beschreven hoe u een afbeelding analyseert die is geïmporteerd voordat u de extensie Afbeeldingsanalyse hebt ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="78250-152">The following steps describe how to analyze an image that was imported before you enabled the Image Analyzer extension.</span></span>  

1. <span data-ttu-id="78250-153">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Contacten** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="78250-153">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Contacts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="78250-154">Kies de contactpersoon en kies vervolgens de actie **Afbeelding analyseren**.</span><span class="sxs-lookup"><span data-stu-id="78250-154">Choose the contact person, and then choose the **Analyze Picture** action.</span></span>  
3. <span data-ttu-id="78250-155">Op het sneltabblad **Profielvragenlijst** controleert u de voorstellen en maakt u correcties, indien nodig.</span><span class="sxs-lookup"><span data-stu-id="78250-155">On the **Profile Questionnaire** FastTab, review the suggestions, and make corrections if needed.</span></span>  

## <a name="to-use-your-own-account-for-the-computer-vision-api"></a><span data-ttu-id="78250-156">Uw eigen account gebruiken voor de Computer Vision API</span><span class="sxs-lookup"><span data-stu-id="78250-156">To use your own account for the Computer Vision API</span></span>
<span data-ttu-id="78250-157">U kunt ook uw eigen account gebruiken voor de Computer Vision-API, bijvoorbeeld als u meer afbeeldingen wilt analyseren dan we toestaan.</span><span class="sxs-lookup"><span data-stu-id="78250-157">You can also use your own account for the Computer Vision API, for example, if you want to analyze more images than we allow.</span></span>  

1. <span data-ttu-id="78250-158">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Instelling van afbeeldingsanalyse** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="78250-158">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Image Analyzer Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="78250-159">Vul de **API-URI** en **API-sleutel** in die u voor de Computer Vision-API hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="78250-159">Enter the **API URI** and **API Key** that you received for Computer Vision API.</span></span>  

>   [!NOTE]  
>   <span data-ttu-id="78250-160">U moet **/analyze** aan het eind van de API-URI toevoegen, als het niet al aanwezig is.</span><span class="sxs-lookup"><span data-stu-id="78250-160">You must add **/analyze** at the end of the API URI, if it isn't already there.</span></span> <span data-ttu-id="78250-161">Bijvoorbeeld: ```https://cronus.api.cognitive.microsoft.com/vision/v1.0/analyze```.</span><span class="sxs-lookup"><span data-stu-id="78250-161">For example: ```https://cronus.api.cognitive.microsoft.com/vision/v1.0/analyze```.</span></span>

## <a name="to-see-how-many-analyses-you-have-left-in-the-current-period"></a><span data-ttu-id="78250-162">Zien hoeveel analyses u in de huidige periode over hebt</span><span class="sxs-lookup"><span data-stu-id="78250-162">To see how many analyses you have left in the current period</span></span>
<span data-ttu-id="78250-163">U kunt het aantal analyses bekijken dat u hebt gedaan, en hoeveel u er in de huidige periode nog kunt doen.</span><span class="sxs-lookup"><span data-stu-id="78250-163">You can view the number of analyses you've done, and how many you can still do, in the current period.</span></span>  

1. <span data-ttu-id="78250-164">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Instelling van afbeeldingsanalyse** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="78250-164">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Image Analyzer Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="78250-165">De **Limietsoort**, **Limietwaarde** en **Analyses uitgevoerd** bieden de gebruiksinformatie.</span><span class="sxs-lookup"><span data-stu-id="78250-165">The **Limit type**, **Limit value**, and **Analyzes performed** provide the usage information.</span></span>  

## <a name="to-stop-using-the-image-analyzer-extension"></a><span data-ttu-id="78250-166">Stoppen met het gebruik van de extensie Afbeeldingsanalyse</span><span class="sxs-lookup"><span data-stu-id="78250-166">To stop using the Image Analyzer extension</span></span>
1. <span data-ttu-id="78250-167">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "Pictogram Zoeken naar pagina of rapport"), voer **Serviceverbindingen** in en kies vervolgens **Instellingen van afbeeldingsanalyse**.</span><span class="sxs-lookup"><span data-stu-id="78250-167">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Connections**, and then choose **Image Analyzer Setup**.</span></span>  
2. <span data-ttu-id="78250-168">Schakel het selectievakje **Afbeeldingsanalyse inschakelen** uit.</span><span class="sxs-lookup"><span data-stu-id="78250-168">Clear the **Enable Image Analyzer** check box.</span></span>  

## <a name="see-also"></a><span data-ttu-id="78250-169">Zie ook</span><span class="sxs-lookup"><span data-stu-id="78250-169">See Also</span></span>
[<span data-ttu-id="78250-170">Werken met artikelkenmerken</span><span class="sxs-lookup"><span data-stu-id="78250-170">Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)  
<span data-ttu-id="78250-171">[[!INCLUDE[d365fin](includes/d365fin_md.md)] aanpassen met behulp van extensies](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="78250-171">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="78250-172">[Welkom bij [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="78250-172">[Welcome to [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)</span></span>  
