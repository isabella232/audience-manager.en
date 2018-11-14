---
description: Describes methods in the DIL.tools namespace. These utility functions help you perform specific tasks.
seo-description: Describes methods in the DIL.tools namespace. These utility functions help you perform specific tasks.
seo-title: DIL Tools
solution: Audience Manager
title: DIL Tools
uuid: 2bc62ce2-16bd-4e80-b493-c816ba643b59
index: y
internal: n
snippet: y
---

# DIL Tools{#dil-tools}

Describes methods in the DIL.tools namespace. These utility functions help you perform specific tasks.

## <wintitle> DIL </wintitle> Tools {#concept_775B2F571721454392969A7FDAB02B37}

Describes methods in the `DIL.tools` namespace. These utility functions help you perform specific tasks.

<!-- 

c_dil_functions.xml

 -->

## getSearchReferrer {#reference_1658BF0239D24C87811BA963E4DB0FB8}

Returns search terms used to reach the current page.

<!-- 

r_dil_get_search_referrer.xml

 -->

**Purpose of `getSearchReferrer`**

In DIL, `getSearchReferrer` returns search results (names and key words) used to reach your site. You can pass in specific search terms to this function or let it search the supported search engines ( [!DNL AOL], [!DNL Ask], [!DNL Bing], [!DNL Google], and [!DNL Yahoo]) against `document.referrer` by default. 
**Function signature:** `DIL.tools.getSearchReferrer(uri, initConfig)`  **Function Parameters**

`getSearchReferrer` accepts:

* *`{string}`*: *(Optional)* A string containing the search URL (uses `document.referrer` if undefined). 

* *`{object}`**(Optional)* An object containing the configuration for the `hostPattern`, `queryParam`, or `queryPattern`.

And returns:

* *`{object}`*: An object that contains valid names and keywords.

**Examples** 

<table id="table_D035276601EC428295E4D619F05BB8D0"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Search Type </th> 
   <th colname="col02" class="entry"> Description </th> 
   <th colname="col2" class="entry"> Code Sample </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr valign="top"> 
   <td colname="col1"> <b>Default Search</b> </td> 
   <td colname="col02"> Returns keyword search terms used by the <span class="keyword"> AOL </span>, <span class="keyword"> Ask </span>, <span class="keyword"> Bing </span>, <span class="keyword"> Google </span>, and <span class="keyword"> Yahoo </span> search engines. </td> 
   <td colname="col2"> 
    <codeblock>
      var&amp;nbsp;results&amp;nbsp;=&amp;nbsp;DIL.tools.getSearchReferrer(); 
    </codeblock> </td> 
  </tr> 
  <tr valign="top"> 
   <td colname="col1"> <b>Pass in a Custom URL</b> </td> 
   <td colname="col02"> Returns the search referrer based on a custom URL. </td> 
   <td colname="col2"> 
    <codeblock>
      var&nbsp;results&nbsp;= 
     
DIL.tools.getSearchReferrer("https://www.ehow.com/ 
     
search.aspx?q=adobe+rules"); 
    </codeblock> </td> 
  </tr> 
  <tr valign="top"> 
   <td colname="col1"> <b>Match URL Hostname with a Custom Regex</b> </td> 
   <td colname="col02"> Pass in a custom regex to match the host name of the referring URL. </td> 
   <td colname="col2"> 
    <codeblock>
      var&nbsp;results&nbsp;= 
     
DIL.tools.getSearchReferrer("https://www.ehow.com/ 
     
search.aspx?q=adobe+rules",{ 
     
&nbsp;&nbsp;&nbsp;hostPattern:/ehow\./, 
     
&nbsp;&nbsp;&nbsp;queryParam:"p" 
     
}); 
    </codeblock> </td> 
  </tr> 
  <tr valign="top"> 
   <td colname="col1"> <b>Match Search Patterns with a Custom Regex</b> </td> 
   <td colname="col02"> Pass in a custom regex to perform a custom search. </td> 
   <td colname="col2"> 
    <codeblock>
      var&nbsp;results&nbsp;= 
     
DIL.tools.getSearchReferrer("https://www.ehow.com/ 
     
search.aspx?q=adobe+rules,{ 
     
&nbsp;&nbsp;&nbsp;hostPattern:/ehow\./, 
     
&nbsp;&nbsp;&nbsp;search_pattern:/[&amp;\?]p=([^&amp;]+/ 
     
}); 
    </codeblock> </td> 
  </tr> 
 </tbody> 
</table>

## decomposeURI {#reference_222B85A7E6E34722B67212C7C080FE5F}

Disassembles a Uniform Resource Identifier ( [!DNL URI]) into its constituent components: hash, host, href, pathname, protocol, search, and [!DNL uriParams].

<!-- 

r_dil_decompose.xml

 -->

Function signature: `DIL.tools.decomposeURI`

**Function Parameters**

`decomposeURI` accepts:

* *`uri {string}`*: *(Optional)* A string containing the URI. Defaults to `document.location.href` if not specified.

And returns:

* *`{object}`*: An object that contains valid names and keywords.

**Sample Code** 

```
var uriData = DIL.tools.decomposeURI('https://www.adobe.com/?arg1=123&arg2=456#am'); 
  
{ 
  hash : "#am", 
  host : "www.adobe.com", 
  hostname : "www.adobe.com", 
  href : "https://www.adobe.com/?arg1=123&arg2=456#am", 
  pathname : "", 
  protocol : "https:", 
  search : "?arg1=123&arg2=456", 
  uriParams : { 
    arg1 : "123", 
    arg2 : "456" 
  } 
}
```

## getMetaTags {#reference_411CD926DD6E45F599581DB5D19C4B30}

Searches for specific content defined in the meta tags on a Web page and returns that data in an object.

<!-- 

r_dil_get_metatags.xml

 -->

**Function signature:** `DIL.tools.getMetaTags( 1 or more parameters)`

**Function Parameters**

`getMetaTags` accepts one or more name parameters (string type) to search for. It returns an object composed of key-value pairs.

**Sample Code** 

```
var dataLib = DIL.create({ 
     partner: ' 
<i>partnerName'</i>, 
     containerNSID:  
<i>containerNSID</i> 
}); 
 
dataLib.api.signals(DIL.tools.getMetaTags(' 
<i>application</i>', ' 
<i>keywords</i>', 
' 
<i>description</i>'), 'c_').submit();
```
