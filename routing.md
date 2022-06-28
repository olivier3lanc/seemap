---
title: Routing
description: Get distance and itinerary between multiple markers
layout: libdoc/page
---
SEEMAP integrates [Leaflet Routing Machine](https://github.com/perliedman/leaflet-routing-machine). Routing requires at least 2 markers to work. 

```html
<SEEMAP_FILE_URL>?routing=<true or false>
```

* If [default routing](settings.html) is set to `false`, just add GET parameter `routing=true` to enable routing.
* If default routing is set to `true`, just add GET parameter `routing=false` to disable routing.

```html
<iframe src="../seemap.html?routing=true&marker=48.852855084244275,2.3482764253351434,Paris&marker=47.05692600913301,2.309900469185777&marker=43.348569315109174,5.374661932049889,Marseille"></iframe>
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
{:.playground title="With routing"}

```html
<iframe src="../seemap.html?marker=48.852855084244275,2.3482764253351434,Paris&marker=47.05692600913301,2.309900469185777&marker=43.348569315109174,5.374661932049889,Marseille"></iframe>
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
{:.playground title="No routing"}

