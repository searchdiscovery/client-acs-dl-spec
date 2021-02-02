# User Registered

Fire whenever a user completes the process of registering for an account.

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "User Registered",
  "authentication": {
    "method": "<method>",
  }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|method|string|The method used to authenticate|email, facebook, google, apple, etc|
