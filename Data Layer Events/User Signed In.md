# User Signed In

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "login",
  "detailed_event": "User Signed In",
    "user_data": {
        "user_type": "<user_type>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|user_data.user_type|string|Captures the type associated with the user \(participant, team leader, etc.\) if known|participant, team lead|||||||




