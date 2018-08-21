---
description: Create mutually exclusive test segments in Segment Test Groups to compare and measure effectiveness of different destinations. You can set aside a control group and divide your segment into percentages of a whole, in order to test efficacy.
seo-description: Create mutually exclusive test segments in Segment Test Groups to compare and measure effectiveness of different destinations. You can set aside a control group and divide your segment into percentages of a whole, in order to test efficacy.
seo-title: Audience Lab
solution: Audience Manager
title: Audience Lab
topic: DIL API
uuid: 307546e7-2abc-470a-a901-a20232041d8d
index: y
internal: n
snippet: y
translate: y
---

# Audience Lab

[!UICONTROL  Audience Lab] uses [ Profile Link](../../c_features/profile-link-intro/profile-link-intro.md#concept_5FCB08A53C4D4C2B82800BC9FD2B8EC9) to power cross-device testing. This helps ensure a user qualifies for the same test segment and receives the same treatment across devices. The test segments in test groups will inherit the [ Profile Merge Rule](../../c_features/profile-link-intro/merge-rules-dashboard.md#concept_0D5FDF17A17B400598B787099A48F865) the base segment has assigned to it. 

The [!UICONTROL  Audience Lab] default view displays a card for each of the test groups. Click a card to access the **[!UICONTROL  Test Group]** view. This view includes the following information: 


* ** [ Test Group Information ](../../c_features/audience-lab/audience-lab-information-view.md#concept_C8A8844639CE41E9AE9D6886D829B8E0) **
* ** [ Test Group Reporting ](../../c_features/audience-lab/audience-lab-reporting-view.md#concept_C8A089E2B1C54D268C4F6475C4D5C9D6) **


You are able to create **up to 10 test groups**, each one with **up to 15 test segments**. 

![](assets/test-groups-view.PNG) 

## Status {#section_4A6E6FC7095B4F13A8CEC8E2EBC01EBF}

The status of a test group can be draft, pending, active, paused or completed. More information on each of them in the table below: 



<table id="table_7A0388BA02E045AC971C06A22DAC2C63"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Status </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Draft</span> </p> </td> 
   <td colname="col2">A <i>draft</i> test group is not yet active and can still be edited. It does not yet send data to the mapped destinations. </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Pending</span> </p> </td> 
   <td colname="col2"> <p>A <i>pending</i> test group is not yet active but cannot be edited anymore. It will become active at the start date you selected in the <b>Create Test Groups</b> wizard. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Active </span> </p> </td> 
   <td colname="col2"> <p>An <i>active</i> test group means that data is currently being sent to destinations. Press <span class="uicontrol"> Pause Test</span> in the <span class="uicontrol"> Test Group</span> card to suspend sending data to destinations. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Paused </span> </p> </td> 
   <td colname="col2"> <p>A <i>paused</i> test group does not currently send data to destinations. Press <span class="uicontrol"> Make Active</span> in the <span class="uicontrol"> Test Group</span> card to resume sending traits. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Completed</span> </p> </td> 
   <td colname="col2">A <i>completed</i> test group has reached the end date you selected in the <b>Create Test Groups </b>wizard and has stopped sending reporting data. </td> 
  </tr> 
 </tbody> 
</table>


## Actions {#section_7548C5D56B004377AB330399746F79F7}



<table id="table_481A411E2D2F4FE891595D00E775CF60"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Actions </th> 
   <th colname="col2" class="entry"> Description </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Edit</span> </p> </td> 
   <td colname="col2"> <p>Available <b>only</b> for draft test groups. Allows you to resume the <span class="uicontrol"> Create New Test Group</span> wizard. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Pause</span> </p> </td> 
   <td colname="col2"> <p>Available for active test groups. Allows you to pause sending the test segments to destinations. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Make Active </span> </p> </td> 
   <td colname="col2"> <p>Available for paused test groups. Allows you to resume sending the test segments to destinations. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> View</span> </p> </td> 
   <td colname="col2"> <p>Available for completed test groups. Allows you to view the reporting information the test has generated. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Duplicate</span> </p> </td> 
   <td colname="col2"> <p>Allows you to create a new test group with the same configuration as the one you are duplicating. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="uicontrol"> Delete</span> </p> </td> 
   <td colname="col2"> <p>Allows you to delete a test group. The test segments will be unmapped from the destinations, the baseline segment and conversion traits associated to the test group are fully editable. An alert will prompt you to download the CSV file when you delete a test group to save the reporting if you wish. </p> </td> 
  </tr> 
 </tbody> 
</table>
