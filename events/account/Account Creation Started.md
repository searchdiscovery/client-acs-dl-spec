# Account Creation Started

Fire whenever a user begins account creation.

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "Account Creation Started",
  "authentication": {
    "method": "<method>",
  }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|method|string|The method used to authenticate|email, facebook, google, apple, etc|
