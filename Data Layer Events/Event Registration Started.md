# Event Registration Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "registration_started",
  "detailed_event": "Event Registration Started",
    "event_data": {
        "name": "<name>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.name|string|Captures the human-friendly name of the form. If for event registration, this should capture the name or unique ID of the event for which the user is registering.|Relay for Life|||||||
|event_data.type|string|Captures whether or not the registration form is pre-populated with the user's information|Pre-Populated or Not Pre-Populated|||||||




