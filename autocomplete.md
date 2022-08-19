---
title: Autocomplete
description: Displays a list of places from few typed letters
layout: libdoc/page
order: 200
---

* 
{:toc}

SEEMAP integrates [Leaflet.Autocomplete](https://github.com/tomik23/Leaflet.Autocomplete) that brings an easy way to find a place or a city thanks to [Nominatim](https://nominatim.openstreetmap.org/ui/search.html) which is the OpenStreetMap search engine. Since autocomplete is based on [GeoJSON](https://geojson.org/) format, it is possible to set any other similar search engine or even your own GeoJSON.

```html
<SEEMAP_FILE_URL>?autocomplete=<true or false>
```

* If [default autocomplete](settings.html) is set to `true`, just add GET parameter `autocomplete=false` to disable autocomplete.
* If default autocomplete is set to `false`, just add GET parameter `autocomplete=true` to enable autocomplete.


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
{:.playground title="Autocomplete enabled"}

## Autocomplete disabled

You can disable autocomplete features through [API](api.html).

```html
<SEEMAP_FILE_URL>?autocomplete=false
```

```html
<iframe src="../../seemap.html?autocomplete=false"></iframe>
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

## Autocomplete zoom

It is possible to adjust the map zoom level applied when an autocomplete choice is done. Autocomplete zoom is set to 12 by default, like any other parameter, it is possible to override it through URL GET parameters.

```html
<SEEMAP_FILE_URL>?autocompleteZoom=<integer or false or null>
```

```html
<iframe src="../../seemap.html?autocompleteZoom=false"></iframe>
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
{:.playground title="Autocomplete zoom disabled"}

```html
<iframe src="../../seemap.html?autocompleteZoom=16"></iframe>
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
{:.playground title="Autocomplete zoom set to 16"}


