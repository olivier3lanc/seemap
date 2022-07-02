---
title: Autocomplete
description: Displays a list of places from few typed letters
layout: libdoc/page
---
SEEMAP integrates [Leaflet.Autocomplete](https://github.com/tomik23/Leaflet.Autocomplete) that brings an easy way to find a place or a city thanks to [Nominatim](https://nominatim.openstreetmap.org/ui/search.html) which is the OpenStreetMap search engine. 

```html
<SEEMAP_FILE_URL>?autocomplete=<true or false>
```

* If [default autocomplete](settings.html) is set to `true`, just add GET parameter `autocomplete=false` to disable autocomplete.
* If default autocomplete is set to `false`, just add GET parameter `autocomplete=true` to enable autocomplete.


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
{:.playground title="Autocomplete enabled"}

```html
<iframe src="../seemap.html?autocomplete=false"></iframe>
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
{:.playground title="Autocomplete disabled"}
