---
layout: libdoc/page-split
permalink: index.html
unlisted: true
---
<abbr title="Standalone EmbEddable Map">SEEMAP</abbr> *for Standalone EmbEddable Map* is single HTML file bundled of useful and popular Leaflet/OpenStreetMap resources in a easy way to embed.

## Key features

* **One single HTML file** Ready to embed via *iframe* tag or directly through the browser, every feature is included.
* **Customizable** Set your own default [settings](settings).
* **API through URL GET parameters** Override your default parameters through [URL GET parameters](api.html).
* **View** Set a default [view](view.html) and override the map geographical center through [API](api.html).
* **Markers** Add as much markers with latitude and longitude through URL GET parameters.
* **Marker clusters** When markers density is to high, provides beautiful animated marker clustering.
* **Gesture handling** Brings the basic functionality of Google Maps Gesture Handling into Leaflet. Prevents users from getting trapped on the map when scrolling a long page. 
* **Routing Machine** Easy way to get distance and itinerary between multiple markers.
* **Autocomplete** OpenStreetMap search engine available into a simple autocompletion list.

## Bundle

SEEMAP concatenates the great following resources:

* [Leaflet.js](https://leafletjs.com/) an open-source JavaScript library
for mobile-friendly interactive maps
* [Leaflet Gesture Handling](https://github.com/elmarquis/Leaflet.GestureHandling) Brings the basic functionality of Google Maps Gesture Handling into Leaflet. Prevents users from getting trapped on the map when scrolling a long page. 
* [Leaflet Marker Cluster](https://github.com/Leaflet/Leaflet.markercluster) Provides Beautiful Animated Marker Clustering functionality for Leaflet, a JS library for interactive maps.
* [Leaflet Routing Machine](https://github.com/perliedman/leaflet-routing-machine) or [Official website](https://www.liedman.net/leaflet-routing-machine/) Provides Beautiful Animated Marker Clustering functionality for Leaflet, a JS library for interactive maps.
* [Leaflet.Autocomplete](https://github.com/tomik23/Leaflet.Autocomplete) OpenStreetMap search engine available into a simple autocompletion list.
* [LeafLet Providers](https://github.com/leaflet-extras/leaflet-providers) An extension to Leaflet that contains configurations for various free and paid tile providers.


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
{:.playground title="SEEMAP"}
