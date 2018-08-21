---
description: Describes the common platform-level key-value pairs you can use to target users with device-related variables across all properties in your Audience Manager account.
seo-description: Describes the common platform-level key-value pairs you can use to target users with device-related variables across all properties in your Audience Manager account.
seo-title: Device Targeting With Platform-level Keys
solution: Audience Manager
title: Device Targeting With Platform-level Keys
uuid: 5b754fb4-71c2-43c4-aee3-e1242db36ff8
index: y
internal: n
snippet: y
translate: y
---

# Device Targeting With Platform-level Keys


## Purpose of Platform-level Variables {#section_57C422B2079C480B907279D5B57A6AEF}

Platform-level variables let you take data passed in from a particular site and make it available for targeting across all the properties in your Audience Manager account. These variables are formed by [ key-value pairs ](../../../c_reference/c_key_value_explained.md#concept_E4236E003076483AA939791FE2492B49) with the key prefixed by ` d_` as shown below. 

## Platform-level Keys Defined by User Agent {#section_BF1FD752F0CF4C8E9326F25F2B9D2136}

The Data Collection Servers extract the values for these keys from the [ user agent header ](https://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.43) in HTTP requests. The values represent device-level information from the Device Atlas database. The signals in the table below are available, as extracted from the user agent example. [ Download a list of the most common keys ](https://marketing.adobe.com/resources/help/en_US/aam/downloads/device_keys.csv), according to Device Atlas measurements. 



|  Signal  | Type  | Example  |
|---|---|---|
|  ` d_device_vendor`  | VENDOR  | apple  |
|  ` d_device_hardware_type`  | HARDWARE  | mobile phone  |
|  ` d_device_os_version`  | OS VERSION  | 5_0  |
|  ` d_device_os_name`  | OS NAME  | ios  |
|  ` d_device_model`  | MODEL  | iphone  |
|  ` d_device_marketing_name`  | MARKETING NAME  | iphone  |
|  ` d_device_manufacturer`  | MANUFACTURER  | apple  |


```
 Mozilla/5.0 (iPhone; CPU iPhone OS 5_0 like Mac OS X) AppleWebKit/534.46 (KHTML, like Gecko) Version/5.1 Mobile/9A334 Safari/7534.48.3
```

>[!NOTE]
>
>Even if one or more signals cannot be retrieved from the user agent header, the other signals will still be passed to the Data Collection Servers.


>[!MORE_LIKE_THIS]
>
>* [ Prefix Requirements for Key Variables ](r_tb_variable_prefixes.md#reference_E6F1E4257F664FC2A797C406BF147ABC)