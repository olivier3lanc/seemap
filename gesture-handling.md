---
title: Gesture handling
description: Feature that prevents users from getting trapped on the map when scrolling a long page
layout: libdoc/page
order: 300
---
SEEMAP integrates [Leaflet Gesture Handling](https://github.com/elmarquis/Leaflet.GestureHandling) that brings the basic functionality of Google Maps Gesture Handling into Leaflet. Useful for iframe embedded maps, gesture handling prevents users from getting trapped on the map when scrolling a long page. 

```html
<SEEMAP_FILE_URL>?gesture=<true or false>
```

* If [default gesture handling](settings.html) is set to `false`, just add GET parameter `gesture=true` to enable gesture handling.
* If default gesture handling is set to `true`, just add GET parameter `gesture=false` to disable gesture handling.

```html
<iframe src="../../seemap.html"></iframe>
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
{:.playground title="Gesture handling disabled (default)"}

```html
<iframe src="../../seemap.html?gesture=true"></iframe>
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
{:.playground title="Gesture handling enabled"}
