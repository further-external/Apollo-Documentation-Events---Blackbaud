# Registration Step Completed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "registration_step_completed",
  "detailed_event": "Registration Step Completed",
    "event_data": {
        "name": "<name>",
        "step_name": "<step_name>",
        "step_number": <step_number>,
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.name|string|Captures the human-friendly name of the form. If for event registration, this should capture the name or unique ID of the event for which the user is registering.|Relay for Life|||||||
|event_data.step_name|string|Captures the name \/ id of each user registration step encountered.||||||||
|event_data.step_number|integer|Captures the number of the step number in the event registration process|1, 2, 3, 4||||1|||
|event_data.type|string|Captures whether or not the registration form is pre-populated with the user's information|Pre-Populated or Not Pre-Populated|||||||




