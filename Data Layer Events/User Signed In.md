# User Signed In

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "login",
  "detailed_event": "User Signed In",
    "event_data": {
        "caregiverStatus": "<caregiverStatus>",
        "donorStatus": "<donorStatus>",
        "individualStatus": "<individualStatus>",
        "survivorStatus": "<survivorStatus>",
        "teamCaptainStatus": "<teamCaptainStatus>",
        "teamMemberStatus": "<teamMemberStatus>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.caregiverStatus|string|Whether or the not the current user is a caregiver|yes, no, leave as empty string if unknown|||||||
|event_data.donorStatus|string|Describes if the user is a donor|yes, no, leave as empty string if unknown|||||||
|event_data.individualStatus|string|Describes whether the current user is considered an individual|yes, no, leave as empty string if unknown|||||||
|event_data.survivorStatus|string|Describes whether the current user is a survivor|yes, no, leave as empty string if unknown|||||||
|event_data.teamCaptainStatus|string|Describes whether the user is a team captain|yes, no, leave as empty string if unknown|||||||
|event_data.teamMemberStatus|string|Describes whether the current user is a Team Member|yes, no, leave as empty string if unknown|||||||




