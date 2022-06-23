---
title: Gesture handling
description: How to install and use SEEMAP
layout: libdoc/page
---
SEEMAP integrates [Leaflet Gesture Handling](https://github.com/elmarquis/Leaflet.GestureHandling) that brings the basic functionality of Google Maps Gesture Handling into Leaflet. Prevents users from getting trapped on the map when scrolling a long page. 

```html
<iframe src="../seemap.html"></iframe>
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

```html
<iframe src="../seemap.html?gesture=false"></iframe>
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
{:.playground title="Gesture handling disabled"}