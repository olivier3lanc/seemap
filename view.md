---
title: View
description: Center the view to specific latitude and longitude
layout: libdoc/page-split
---

Discrete from marker and zoom, it is possible to adjust the center of the view on specific latitude and longitude coordinates.

```html
<SEEMAP_FILE_URL>?view=<lat>,<lng>
```

* `<lat>` - *mandatory* - Latitude, for ex. *45.1234*
* `<lng>` - *mandatory* - Longitude, for ex. *2.4321*

```html
<iframe src="../seemap.html?view=48.85830,2.29435"></iframe>
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
{:.playground title="?view=48.85830,2.29435"}
