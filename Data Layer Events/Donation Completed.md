# Donation Completed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "purchase",
  "detailed_event": "Donation Completed",
    "ecommerce": {
        "affiliation": "<affiliation>",
        "currency": "<currency>",
        "items": [
            {
                "affiliation": "<affiliation>",
                "currency": "<currency>",
                "item_brand": "<item_brand>",
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "item_variant": "<item_variant>",
                "price": <price>,
                "quantity": <quantity>
            }
        ],
        "payment_frequency": "<payment_frequency>",
        "payment_id": "<payment_id>",
        "payment_method": "<payment_method>",
        "thank_you_card_type": "<thank_you_card_type>",
        "transaction_id": "<transaction_id>",
        "type": "<type>",
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.affiliation|string|A order affiliation to designate a supplying company or brick and mortar store location.|Google Store|||||||
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format. Set as "USD" unless other currencies are accepted in the future.||||||||
|ecommerce.items[n].affiliation|string|A product affiliation to designate a supplying company or brick and mortar store location.|Google Store|||||||
|ecommerce.items[n].currency|string|The currency, in 3-letter ISO 4217 format. Always set to a static value of "USD" as long as USD is the only accepted currency on the site.|USD|||||||
|ecommerce.items[n].item_brand|string|Captures the event type \(RFL, RMWP, MSABC, etc.\)|RFL, RMWP, MSABC|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\). This may be equivalent to the FR\_ID value.|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\). Captures the name of the event for which the user is donating.|jeggings|||||||
|ecommerce.items[n].item_variant|string|The variant of the item.|Black|||||||
|ecommerce.items[n].price|number|The monetary price of the item, in units of the specified currency parameter.|9.99|||||||
|ecommerce.items[n].quantity|integer|Item quantity.|1|||||||
|ecommerce.payment_frequency|string|Captures the recurring frequency of donation \(i.e. one-time, monthly\).|One Time, Monthly|||||||
|ecommerce.payment_id|string|Captures a unique payment ID for a transaction.||ZPH-87698-098||||||
|ecommerce.payment_method|string|Captures the payment methods used for a transaction \(i.e. credit card, Visa, MasterCard, Amex, Paypal, purchase order, etc\).|Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|ecommerce.thank_you_card_type|string|Captures the type of card requested with a donation \(i.e. email, physical, e-card1, e-card2\).|Electronic, Physical|||||||
|ecommerce.transaction_id|string|The unique identifier of a transaction.|T\_12345, 19283j2nm9jdjs|^[a-zA-Z0-9]{6,20}$|6|20||||
|ecommerce.type|string|Captures the type of donation made \(i.e. Luminaria, Participant, Team, Event\).|Luminaria, Participant, Team, Event|||||||
|ecommerce.value|number|The monetary value of the event. If no value is yet available, set to 0.|7.77, 239.55, 659|||||||




