---
description: Common product and function-related questions and issues.
keywords: audience manager cookies
seo-description: Common product and function-related questions and issues.
seo-title: Product Features and Functions FAQ
solution: Audience Manager
title: Product Features and Functions FAQ
uuid: 780bd9ee-b988-49c4-8274-e5e9313b7df4
index: y
internal: n
snippet: y
translate: y
---

# Product Features and Functions FAQ

**What is my Organization ID and how do I find it?** 

The *` Organization ID`* is a unique ID that identifies your organization to [!DNL  Audience Manager] and the [!DNL  Adobe Experience Cloud]. It consists of a case-sensitive, 24-character alphanumeric string followed by [!UICONTROL  @AdobeOrg]. For example, an Organization ID looks like this: ` 1FD6776A524453CC0A490D44@AdobeOrg`. The Organization ID is used by Audience Manager's [ DIL ](../c_api/c_dil/c_dil.md#concept_6D73ED3DBA604EE49B66B5572AA6A32C) API, the [ Experience Cloud ID service ](https://marketing.adobe.com/resources/help/en_US/mcvid/), and other [!DNL  Experience Cloud] solutions. Users with Administrator permissions can find the Organization ID on the [!DNL  Adobe Admin Console]. See the [ Administration - User Management FAQ ](https://marketing.adobe.com/resources/help/en_US/mcloud/admin_getting_started.html). 

**Can I create traits or destinations in bulk?** 

Yes. See [ Bulk Management Tools ](../c_reference/c_bulk/c_bulk.md#concept_8D6CB301643C482F994938F6484B390C). 


>[!NOTE]
>
>The [!UICONTROL  Bulk Management Tools] tools *are not* supported by [!DNL  Audience Manager]. They're provided for convenience and as a courtesy only. For bulk changes, we recommend you work with the [ Audience Manager APIs ](../c_api/c_api.md#concept_8C41AAD825A24A01806E64C32F71472A) instead. 



**Can [!DNL  Audience Manager] reduce the need for third-party tags or pixels and improve page load times?** 

If [!DNL  Audience Manager] is integrated with your third-party data partner, you can replace their pixels and tags with a server-to-server ID call to [!DNL  Audience Manager]. In this case, [!DNL  Audience Manager] would fire a single ID call the first time we see a user and synchronize that information with your third-party partner. This eliminates the need to make multiple pixels call from every page. Reducing pixel calls can improve page load times. 

**I've subscribed to a Data Feed. Where is that data stored?** 

Your Data Feed and all the traits contained in the feed appear as subfolders and traits in [!DNL  Audience Manager]. Go to **[!UICONTROL  Audience Data > Traits]** and expand the 3rd-Party Data folder to view your traits or create segments and models with this data. 

