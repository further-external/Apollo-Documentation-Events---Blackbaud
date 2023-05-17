# Onsite Search Failed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "view_search_results",
  "detailed_event": "Onsite Search Failed",
    "event_data": {
        "search_term": "<search_term>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.search_term|string|Captures the search text used in on-site searches.|dallas, 75248, Carroll High School|||||||
|event_data.type|string|Captures the type of on-site search performed \(event, etc.\)|event|||||||




