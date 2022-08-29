---
title: Routing
description: Get distance and itinerary between multiple markers
layout: libdoc/page
order: 800
---
SEEMAP integrates [Leaflet Routing Machine](https://github.com/perliedman/leaflet-routing-machine) based on [OSRM](http://map.project-osrm.org) (Open Source Routing Machine). Routing requires at least 2 markers to work. **Important note:** SEEMAP use default settings for Leaflet Routing Machine, please respect the [usage policy of OSRM](https://github.com/Project-OSRM/osrm-backend/wiki/Api-usage-policy) or use any other routing machine.
```html
<SEEMAP_FILE_URL>?routing=<true or false>
```

* If [default routing](settings.html) is set to `false`, just add GET parameter `routing=true` to enable routing.
* If default routing is set to `true`, just add GET parameter `routing=false` to disable routing.

```html
<iframe src="../../seemap.html?routing=true&marker=48.852855084244275,2.3482764253351434,Paris&marker=44.742734018656435,-0.5371049978895037,Bordeaux&marker=41.892069845070736,12.514922686644816,Rome&marker=41.84400446089234,12.564361163207316,Rome 2"></iframe>
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
<iframe src="../../seemap.html?&marker=48.852855084244275,2.3482764253351434,Paris&marker=44.742734018656435,-0.5371049978895037,Bordeaux&marker=41.892069845070736,12.514922686644816,Rome&marker=41.84400446089234,12.564361163207316,Rome 2"></iframe>
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


