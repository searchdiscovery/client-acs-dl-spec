# Content Listing Displayed

Fire whenever a list of content that can or has been searched, filtered, or otherwise dynamically changed is displayed. For registration pages, fire when list of events is displayed.

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "Content Listing Displayed",
    "resultsCount": "<resultsCount>",
    "searchTerm": "<searchTerm>",
  }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|resultsCount|integer|The total number of items returned that matched the search criteria.|10|
|searchTerm|string|Describes the search keyword used after auto-correct, auto-complete, or keyword suggestion.|bluth, blue, red lobster|