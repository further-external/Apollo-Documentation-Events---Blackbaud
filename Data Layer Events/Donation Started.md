# Donation Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "begin_checkout",
  "detailed_event": "Donation Started",
    "ecommerce": {
        "currency": "<currency>",
        "items": [
            {
                "item_brand": "<item_brand>",
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "price": "<price>",
                "quantity": <quantity>
            }
        ],
        "type": "<type>",
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|Specifies the currency to be used. Enables exchange rate calucations at the time of data caputure.|USD, CAD, GBP, CHF|^[A-Z]{3}$|3|3||||
|ecommerce.items[n].item_brand|string|Captures the event type \(RFL, RMWP, MSABC, etc.\)|RFL, RMWP, MSABC|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\). This may be equivalent to the FR\_ID value.|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\). Captures the name of the event for which the user is donating.|jeggings|||||||
|ecommerce.items[n].price|string|Captures the donation amount. If unknown at any stage, set to 0.|200, 29.99, 50, 0|^[0-9]*(\.[0-9]{1,2})?$||||||
|ecommerce.items[n].quantity|integer|Number of items. For donations, this will always be 1 and the value of the donation will be captured in a separate field.|1, 2, 3, 4, 5||||1|||
|ecommerce.type|string|Captures the type of donation made \(i.e. Luminaria, Participant, Team, Event\).|Luminaria, Participant, Team, Event|||||||
|ecommerce.value|number|The monetary value of the event. If no value is yet available, set to 0.|7.77, 239.55, 659|||||||




