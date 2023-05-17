# Form Submission Failed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "form_error",
  "detailed_event": "Form Submission Failed",
    "event_data": {
        "error_message": "<error_message>",
        "form_field_error_message": "<form_field_error_message>",
        "form_field_id": "<form_field_id>",
        "fundraiserID": "<fundraiserID>",
        "identifier": "<identifier>",
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
|event_data.error_message|string|Captures the form error code or message associated with form errors.|Credit card declined, Required entries missing, EC3456, EC8976|||||||
|event_data.form_field_error_message|string|Captures the form field error code or message associated with form field errors.|email address invalid, date required. EC987767, EC4567|||||||
|event_data.form_field_id|string|Captures the ID of each field contained on a form.||||||||
|event_data.fundraiserID|string|Provides the name or ID of the fundraiser||||||||
|event_data.identifier|string|Captures the unique ID of the form.|F-0113, 2543, CU001, PI-0988|||||||
|event_data.name|string|Captures the human-friendly name of the form. If for event registration, this should capture the name or unique ID of the event for which the user is registering.|Relay for Life|||||||
|event_data.step_name|string|Captures the name \/ id of each user registration step encountered.||||||||
|event_data.step_number|integer|Captures the number of the step number in the event registration process|1, 2, 3, 4||||1|||
|event_data.type|string|Captures whether or not the registration form is pre-populated with the user's information|Pre-Populated or Not Pre-Populated|||||||




