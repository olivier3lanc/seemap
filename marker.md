---
title: Single marker
description: Adding a single marker on the map through URL GET parameters
layout: libdoc/page-split
order: 500
---

A marker is defined as follows through URL GET parameters: Latitude, comma, longitude, comma, optional text content for popup.

```html
<SEEMAP_FILE_URL>?marker=<lat>,<lng>[,<popup content>]
```

* `<lat>` - *mandatory* - Latitude, for ex. *45.1234*
* `<lng>` - *mandatory* - Longitude, for ex. *2.4321*
* `<content>` - *optional* - Text string to display on marker popup.

```html
<iframe src="../../seemap.html?marker=48.85830,2.29435,Optional text to display"></iframe>
<!-- DEMO ONLY -->
<style>
    iframe {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        border: none;
    }
</style>
```
{:.playground title="?marker=48.85830,2.29435,Optional text to display"}
