# Event Registration Completed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "registration_completed",
  "detailed_event": "Event Registration Completed",
    "event_data": {
        "caregiverStatus": "<caregiverStatus>",
        "donorStatus": "<donorStatus>",
        "individualStatus": "<individualStatus>",
        "name": "<name>",
        "survivorStatus": "<survivorStatus>",
        "teamCaptainStatus": "<teamCaptainStatus>",
        "teamMemberStatus": "<teamMemberStatus>",
        "type": "<type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.caregiverStatus|string|Whether or the not the current user is a caregiver|yes, no, leave as empty string if unknown|||||||
|event_data.donorStatus|string|Describes if the user is a donor|yes, no, leave as empty string if unknown|||||||
|event_data.individualStatus|string|Describes whether the current user is considered an individual|yes, no, leave as empty string if unknown|||||||
|event_data.name|string|Captures the human-friendly name of the form. If for event registration, this should capture the name or unique ID of the event for which the user is registering.|Relay for Life|||||||
|event_data.survivorStatus|string|Describes whether the current user is a survivor|yes, no, leave as empty string if unknown|||||||
|event_data.teamCaptainStatus|string|Describes whether the user is a team captain|yes, no, leave as empty string if unknown|||||||
|event_data.teamMemberStatus|string|Describes whether the current user is a Team Member|yes, no, leave as empty string if unknown|||||||
|event_data.type|string|Captures whether or not the registration form is pre-populated with the user's information|Pre-Populated or Not Pre-Populated|||||||

