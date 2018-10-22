---
description: A bulk estimate returns segment size data based on segment rules. Follow these instructions to make a bulk estimate request.
seo-description: A bulk estimate returns segment size data based on segment rules. Follow these instructions to make a bulk estimate request.
seo-title: Bulk Estimates
solution: Audience Manager
title: Bulk Estimates
uuid: f782e511-91d2-45fd-9442-12ab93ca8b1a
index: y
internal: n
snippet: y
translate: y
---

# Bulk Estimates

A bulk estimate returns segment size data based on segment rules. Follow these instructions to make a bulk estimate request.

<!-- t_bulk_estimates.xml -->

>[!NOTE]
>
>The [!UICONTROL Bulk Management Tools]* are not* supported by [!DNL Audience Manager]. This tool is provided for convenience and as a courtesy only. For bulk changes, we recommend that you work with the [Audience Manager APIs](https://marketing.adobe.com/resources/help/en_US/aam/?f=c_api.html) instead. [RBAC group permissions](../../c_features/c_administration/c_administration.md#concept_A606A162611E4256BB80F60715282296) assigned in the Audience Manager UI are honored in the Bulk Management Tools.

To make bulk updates, open the [!UICONTROL Bulk Management Tools] worksheet and: 

1. Click the **[!UICONTROL Headers]** tab and copy the [!UICONTROL Estimate Segment Size] header.
1. Click the **[!UICONTROL Estimate]** tab.
1. Paste the estimate header into the first row of the estimate worksheet.
1. Paste or type the data you want to change into a corresponding column based on the header label.
1. In the worksheet toolbar, click the create button that matches the item you're updating.

   This action opens the [!UICONTROL Account Information] dialog box. 1. Provide the required [log on information](../../reference/bulk-management-tools/bulk-management-intro.md#section_6FE9BADB30254A4FADC77D2DCFB6A1EE) and click **[!UICONTROL Submit]**.

   This action creates a [!UICONTROL Response] column in the worksheet that contains estimated segment size data. Before entering data, your bulk estimate worksheet should look similar to the following: 
>
>![](assets/estimate.png) 
>
>If your bulk update returns an error or fails, see [Troubleshooting for Bulk Management Tools](../../reference/bulk-management-tools/bulk-troubleshooting.md#reference_1A3E7E0CEF6A4D8D801BC363A3C30C1A). 
