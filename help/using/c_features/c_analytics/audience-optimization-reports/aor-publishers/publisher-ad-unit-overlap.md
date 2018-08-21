---
description: The Ad Unit Overlap report is displayed as a heat chart that highlights high and low overlaps between your Ad Units.
seo-description: The Ad Unit Overlap report is displayed as a heat chart that highlights high and low overlaps between your Ad Units.
seo-title: Ad Unit Overlap
solution: Audience Manager
title: Ad Unit Overlap
uuid: 35e90b39-25b5-4206-8f63-6928e1c15596
index: y
internal: n
snippet: y
translate: y
---

# Ad Unit Overlap

Contents: 


<ul class="simplelist"> 
 <li> <a href="../../../../c_features/c_analytics/audience-optimization-reports/aor-publishers/publisher-ad-unit-overlap.md#section_23446DAFA3424CDBA8834816832EC2B0" format="dita" scope="local"> Use Case</a> </li> 
 <li><a href="../../../../c_features/c_analytics/audience-optimization-reports/aor-publishers/publisher-ad-unit-overlap.md#section_62E5C43C88EE4AE688285F759810F57F" format="dita" scope="local"> Using the Ad Unit Overlap Report</a> </li> 
 <li><a href="../../../../c_features/c_analytics/audience-optimization-reports/aor-publishers/publisher-ad-unit-overlap.md#section_CC66FBF6E9F349B8B0F3F70B05C411F0" format="dita" scope="local"> Interpreting the Results</a> </li> 
</ul>



## Use Case {#section_23446DAFA3424CDBA8834816832EC2B0}

With the [!UICONTROL  Ad Unit Overlap] report, you can gain insight into where your audience overlaps across your web properties. The report considers your 100 top related properties and shows you the overlap between them. 

## Using the Ad Unit Overlap Report {#section_62E5C43C88EE4AE688285F759810F57F}

Use the **[!UICONTROL  Top N Base Ad Units]** and **[!UICONTROL  Top N Overlapping Ad Units]** controls to select your desired number of ad units for the overlap. You can select a maximum number of 100 items for each. 

Use the **Day Range** and **Date Through** controls to adjust your look-back range. Note that the 7-day and 30-day look-back periods are only available for Sunday dates. 

Use the **[!UICONTROL  Base Ad Unit]** and the **[!UICONTROL  Overlap Ad Unit]** controls to select which of your ad units you want to display in the overlap report. 


>[!IMPORTANT]
>
>When enabling Audience Optimization for Publishers, you must include descriptive metadata for Ad Unit IDs, as described in Step 3 of[ Import DFP Data Files Into Audience Manager](../../../../c_features/c_analytics/audience-optimization-reports/aor-publishers/import-dfp.md#concept_32EC89A543BA4333B62DD4C0B3E7060A). By doing this, you assure that the report details the web property as Ad Unit instead of the Ad Unit ID. 



## Interpreting the Results {#section_CC66FBF6E9F349B8B0F3F70B05C411F0}

Your Ad Unit Overlap report could look similar to the one below. Hover over any cell to obtain more information about that particular overlap. See descriptions for the additional information in the table below the sample report. 

![](assets/publisher_ad_unit_overlap.png) 



<table id="table_22340F45B1B94D3796174CB30A60E212"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Item </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Overlap Ad Unit </p> </td> 
   <td colname="col2"> <p>The name of your inventory item. For example, this can be one of your websites or an article on your website. In the image above, the base ad units are Articles 9 - 18. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Base Ad Unit </p> </td> 
   <td colname="col2"> <p>The name of your inventory item. For example, this can be one of your websites or an article on your website. In the image above, the base ad units are Articles 1 - 8. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Overlap Ad Unit Uniques Count </p> </td> 
   <td colname="col2"> <p>The number of your users who have visited the ad unit items 9 - 18. This information is extracted from the DFP logs. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Base Ad Unit Uniques Count </p> </td> 
   <td colname="col2"> <p>The number of your users who have visited the ad unit items 1 - 8. This information is extracted from the DFP logs. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Overlap Uniques Count </p> </td> 
   <td colname="col2"> <p>The overlap between your users who have visited a Base Ad Unit and Overlap Ad Unit. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Overlap Percentage </p> </td> 
   <td colname="col2"> <p>The overlap between your users who have visited a Base Ad Unit and Overlap Ad Unit. This is the Overlap Uniques Count, expressed as a percentage of the Base Ad Unit. </p> </td> 
  </tr> 
 </tbody> 
</table>
