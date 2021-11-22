# Specific Carousel Slide

Fire whenever a user interacts with the specific carousel slide control

## HTML Data Attributes

```html
<a href="<link_url>"
  data-layer-event="specific_carousel_slide"
  data-layer-carousel_id="<carousel_id>"
  data-layer-carousel_name="<carousel_name>"
  data-layer-slot="<slot>"
  data-layer-target_slot="<target_slot>"
>
```

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  event: 'specific_carousel_slide',
  event_data: {
    event_specific_id: "<carousel_id>",
    event_specific_name: "<carousel_name>",
    slot: "<slot>",
    target_slot: "<target_slot>"
  }
});
```

## Variable Definitions

|Field|Type|Required|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_specific_id|string|required|The computer-readable machine name of the carousel. Use UUID provided by the component|12345abcde12345|
|event_specific_name|string|recommended|The human-readable name of the carousel. If user does not input one, populate with numerical index of which carousel this is on the page (1-indexed)|Most Popular Blog Posts, 2|
|slot|integer|recommended|The slide # the carousel is on at time of interaction (1-indexed)|1||1||1
|target_slot|integer|recommended|The slide # of the target slide (1-indexed)|2||1||1|