# User Detected

Fire whenever an authenticated user is detected on each page.

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "User Detected",
  "user": {
    "custKey": "<custKey>",
  }
});
```
## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|custKey|string|Unique user ID generated by the site|
