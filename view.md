---
title: View
description: Center the view to specific latitude and longitude
layout: libdoc/page-split
order: 100
---

Discrete from marker and zoom, it is possible to adjust the center of the view on specific latitude and longitude coordinates.

```html
<SEEMAP_FILE_URL>?view=<lat>,<lng>
```

* `<lat>` - *mandatory* - Latitude, for ex. *-71.5249090*
* `<lng>` - *mandatory* - Longitude, for ex. *290.99487*

```html
<iframe src="../../seemap.html?view=-71.5249090,290.99487"></iframe>
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
{:.playground title="?view=-71.5249090,290.99487"}

