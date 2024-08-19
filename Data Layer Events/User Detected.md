# User Detected

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "detect_user",
  "detailed_event": "User Detected",
    "event_data": {
        "caregiverStatus": "<caregiverStatus>",
        "donorStatus": "<donorStatus>",
        "individualStatus": "<individualStatus>",
        "survivorStatus": "<survivorStatus>",
        "teamCaptainStatus": "<teamCaptainStatus>",
        "teamMemberStatus": "<teamMemberStatus>"
    },
    "page_data": {
        "user_login_state": "<user_login_state>"
    },
    "user_data": {
        "user_id": "<user_id>",
        "user_registration_status": "<user_registration_status>"
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
|page_data.user_login_state|string|Captures the current sign in status for the user \(i.e. signed\_out, signed\_in, unknown\).|logged in, logged out, guest|||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated.|123456, abc123|||||||
|user_data.user_registration_status|string|Captures the current registration status of the user.|registered|||||||

## Attached Notes

<p>This should occur before the Page View event.</p>
