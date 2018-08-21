---
description: The Cross Channel Conversion option in the Audience Optimization reports allows you to attribute offline conversions to served online impressions or clicks.
seo-description: The Cross Channel Conversion option in the Audience Optimization reports allows you to attribute offline conversions to served online impressions or clicks.
seo-title: Cross Channel Conversion
solution: Audience Manager
title: Cross Channel Conversion
uuid: 45473b28-1add-4fb0-9437-ac4aa3d63e53
index: y
internal: n
snippet: y
translate: y
---

# Cross Channel Conversion

The [!UICONTROL  Cross Channel Conversion] reports combine results from the DoubleClick Campaign Manager (DCM) platform with Audience Manager conversion traits. This lets you link offline conversions to online impressions or clicks. You can use the [!UICONTROL  Cross Channel Conversion] for the [ Segment Performance](../../../../c_features/c_analytics/audience-optimization-reports/aor-advertisers/segment-performance.md#concept_16474D96F85C44BEBBE767E66F79D8DE) and [ Optimal Frequency](../../../../c_features/c_analytics/audience-optimization-reports/aor-advertisers/optimal-frequency.md#concept_147AF0587D6546FA814C7870DBAA81EB) reports. 

To view the [!UICONTROL  Cross Channel Conversion] reports, select the **[!UICONTROL  AAM+DCM]** item in the **[!UICONTROL  Platform]** drop-down list. 

The following table lists important considerations when setting up [!UICONTROL  Cross Channel Conversion]: 



<table id="table_62590B4AB7624B619EC9AA8FF89722C9"> 
 <thead> 
  <tr> 
   <th class="entry"> Consideration </th> 
   <th class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col01"> <p>Minimum number of conversion traits </p> </td> 
   <td colname="col1"> <p>At least one conversion trait must be assigned to a data source in order for the <span class="wintitle"> Cross Channel Conversion</span> reports to run. See <a href="../../../../c_features/c_tb_overview/c_tb_main/c_trait_create/c_tb_basics.md#concept_D80233EF56764376B0F4C4FF882BAD2E" format="dita" scope="local"> Basic Information for Traits</a> for more information on traits. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col01"> <p>Maximum number of conversion traits </p> </td> 
   <td colname="col1"> <p>The reports pull in a <i>maximum</i> of 50 conversion traits from the user. If you reach the maximum, the reports use the first 50 conversion traits based on trait ID, in ascending order. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Attribution window </p> </td> 
   <td> <p> <span class="uicontrol"> The AAM+DCM</span> attribution window is 14 days, meaning that only conversion traits exhibited in the last two weeks are considered. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Last-touch methodology </p> </td> 
   <td> <p>The creative that the user has seen last before converting is the one awarded the conversion. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Clicks versus impressions </p> </td> 
   <td> <p>A click takes precedence over an impression when deciding attribution if they occur at the exact same time. For example, on a page where multiple creatives are displayed, the one being clicked on is awarded the conversion. </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Data recency </p> </td> 
   <td> <p>The reports are always calculated for data available the previous day. </p> </td> 
  </tr> 
 </tbody> 
</table>
