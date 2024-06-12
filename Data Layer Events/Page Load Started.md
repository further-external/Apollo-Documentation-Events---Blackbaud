# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_load_started",
  "detailed_event": "Page Load Started",
    "page_data": {
        "breadcrumb": "<breadcrumb>",
        "country": "<country>",
        "language": "<language>",
        "name": "<name>",
        "page_location": "<page_location>",
        "site_name": "<site_name>",
        "site_section": "<site_section>",
        "site_type": "<site_type>",
        "system_environment": "<system_environment>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.breadcrumb|string|A delimited list of hierarchical sections that describe the current page's location within the navigation of the site.|Home&gt;Women&gt;Tops&gt;Sweaters, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Checkout &gt; Order Thank You|||||||
|page_data.country|string|The country associated with the current page.|US, CA, FR, UK|||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.|en-us, en-gb, ch-cn, fr-ca, fr-fr|||||||
|page_data.name|string|Captures the name of the page the user is on|product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|page_data.page_location|string|The URL of the page currently being viewed. This value will include the full, unaltered URL of the page\/screen the user is currently viewing, including query parameters, fragments, etc., for example https:\/\/www.example.com\/home?user=true&audience=test\#aboutus.|https:\/\/www.example.com\/home?user=true&audience=test\#aboutus|||||||
|page_data.site_name|string|Common language used within the business to refer to the website. May be specific County Sites.|Prospecting-EU, Prospecting-US, Member Portal, Shop-CA, Shop-US, Shop-EU|||||||
|page_data.site_section|string|The section of the site that the current page resides in. site\_section2 through site\_section5can also be used if the site has many sections.||||||||
|page_data.site_type|string|Common language description of the site type of purpose. May be used to group siteName.|Prospecting, Shop, Members, Brand|||||||
|page_data.system_environment|string|The environment type of the site, is used to distinguish between product and non-production activity.|production, non-production|||||||


## Attached Notes

<p>This should be the first event that loads during the page load process before any other event is fired.</p>
