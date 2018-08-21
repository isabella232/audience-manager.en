---
description: This section describes how to parse a DCS response to retrieve the visitor and region IDs required to make real-time calls to the DCS.
seo-description: This section describes how to parse a DCS response to retrieve the visitor and region IDs required to make real-time calls to the DCS.
seo-title: Get User IDs and Regions From a DCS Response
solution: Audience Manager
title: Get User IDs and Regions From a DCS Response
uuid: 2090543f-c225-4c8a-ad4e-66fda0aed438
index: y
internal: n
snippet: y
translate: y
---

# Get User IDs and Regions From a DCS Response


## User and Region IDs {#section_B823FA32B7634AB3820CD30264284150}

A DCS response contains data about your site visitors. You need the visitor and region ID before you can make server-to-server calls to the DCS. 


* The user ID is required to identify and associate data with a particular visitor.
* The region ID is required because it is tied to a regional server name, which you need to send data to the DCS. The DCS stores information in data centers that are geographically closest to site visitors. See [ DCS Region IDs, Locations, and Host Names](../../../c_api/dcs-intro/dcs-api-reference/dcs-regions.md#concept_01C1E017A6694D1EAF9BF65BFFA54091).


These parameters are described below. Code in *italics* represents a variable placeholder. 



<table id="table_822C02D5978348DCB7153001882D397C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Parameter </th> 
   <th colname="col2" class="entry"> Data type </th> 
   <th colname="col3" class="entry"> Example </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p><span class="codeph">"uuid":<span class="varname"> user ID</span></span> </p> </td> 
   <td colname="col2"> <p>String </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> "uuid":"123456789"</span> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph">"dcs_region":<span class="varname"> region ID</span></span> </p> </td> 
   <td colname="col2"> <p>Int </p> </td> 
   <td colname="col3"> <p> <span class="codeph"> "dcs_region":9</span> </p> </td> 
  </tr> 
 </tbody> 
</table>


## Sample Response {#section_0D29A02C954C407596E75DD8174E5705}

This simple response shows the UUID and region ID. Note, this is sample data only. Your log files may be longer and more complex. 


```
js{
    "stuff": [],
    "uuid": "22920112968019678612904394744954398990",
    "dcs_region": 7,
    "tid": "31ZpxW5bQGc="
}
```


## Next Steps {#section_66EF69EF07CB48D487DA5C7A510ABDA0}

Once you have the user ID and regional server name, you can start sending and receiving DCS data. See[ Making DCS API Calls](../../../c_api/dcs-intro/dcs-s2s/dcs-s2s-calls.md#concept_57686178E4174EE1A952E0E51BC8A52C). 