# User Registered

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "sign_up",
  "detailed_event": "User Registered",
    "event_data": {
        "method": "<method>",
        "name": "<name>",
        "step_name": "<step_name>",
        "step_number": <step_number>
    },
    "page_data": {
        "user_login_state": "<user_login_state>"
    },
    "user_data": {
        "user_city": "<user_city>",
        "user_country": "<user_country>",
        "user_id": "<user_id>",
        "user_registration_status": "<user_registration_status>",
        "user_state_or_province": "<user_state_or_province>",
        "user_type": "<user_type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.method|string|Captures the website method \(i.e. search, top nav\) used to find each product.|email, facebook, twitter|||||||
|event_data.name|string|Captures the human-friendly name of the form. If for event registration, this should capture the name or unique ID of the event for which the user is registering.|Relay for Life|||||||
|event_data.step_name|string|Captures the name \/ id of each user registration step encountered.||||||||
|event_data.step_number|integer|Captures the number of the step number in the event registration process|1, 2, 3, 4||||1|||
|page_data.user_login_state|string|Captures the current sign in status for the user \(i.e. signed\_out, signed\_in, unknown\).|logged in, logged out, guest|||||||
|user_data.user_city|string|Captures the city associated with the user.||||||||
|user_data.user_country|string|Captures the country associated with the user.|USA, Canada|||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated.|123456, abc123|||||||
|user_data.user_registration_status|string|Captures the current registration status of the user.|registered|||||||
|user_data.user_state_or_province|string|Captures the state or province associated with a tranaction or significant user action.||||||||
|user_data.user_type|string|Captures the type associated with the user \(participant, team leader, etc.\) if known|participant, team lead|||||||

## Attached Notes

<p>Fires on the final step of the registration process.</p>
