---
description: View outbound batch job history information for a specified destination and time period.
seo-description: View outbound batch job history information for a specified destination and time period.
seo-title: Outbound History Report
solution: Audience Manager
title: Outbound History Report
uuid: 2ae9d8b5-9310-456c-9707-6e962159ea9e
index: y
internal: n
snippet: y
translate: y
---

# Outbound History Report

View outbound batch job history information for a specified destination and time period.

1. 

   <!-- t_reports_outbound_history.xml -->

   Click **[!UICONTROL Analytics]** > **[!UICONTROL Outbound History]**.

   ![Step Result](assets/outbound_history.png) 
1. In the **[!UICONTROL Search for a Destination]** box, start typing and select the desired destination.
1. In the **[!UICONTROL Select a Date Range]** box, specify the start and end dates for your report, then click **[!UICONTROL Apply Date Filter]**.

   ![Step Result](assets/outbound_history_stats.png)

   The following table contains information corresponding to columns in the report: 

<table id="table_93076D46AC50411395E72B9B987E99BE"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Line </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> Data Sync File Name </td> 
   <td colname="col2"> <p>List of all outbound files that <span class="keyword"> Adobe</span> generated for this destination that were processed together. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Successful </td> 
   <td colname="col2"> <p>Number of records that were successfully sent from <span class="keyword"> Audience Manager</span> to the destination. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Failed </td> 
   <td colname="col2"> <p>Number of records that could not be sent to the destination. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Records Received </td> 
   <td colname="col2"> <p>Total number of records <span class="keyword"> Adobe</span> generated in the files and attempted to send to the destination. In most cases, this should be the total number of successful files and failed files. </p> </td> 
  </tr> 
 </tbody> 
</table>
