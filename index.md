---
layout: libdoc/page-split
permalink: index.html
unlisted: true
---
A single HTML map file bundled with customizable popular Leaflet plugins, map providers and its own API. <abbr title="Standalone EmbEddable Map">SEEMAP</abbr> *for Standalone EmbEddable Map* is **a single HTML file** bundled of useful and popular Leaflet/OpenStreetMap resources in a easy way to embed.

| Description |  |
| :- | :- |
| Download link to the latest version of SEEMAP | **[Download](seemap.html){: download="" title="Download the latest version of seemap.html"}** |
| Uncompressed page size | **1.6Mb** |
| Compressed page size (through HTTP2 or ZIP) | **190Kb** |
| Typical embed size through an iframe (with tiles) | **500Kb** |
| PageSpeed Insights test on mobile | [Test now](https://pagespeed.web.dev/report?url=https%3A%2F%2Folivier3lanc.github.io%2Fseemap%2Fseemap.html&form_factor=mobile) |
| PageSpeed Insights test on desktop | [Test now](https://pagespeed.web.dev/report?url=https%3A%2F%2Folivier3lanc.github.io%2Fseemap%2Fseemap.html&form_factor=desktop) |

<br>

* **One single HTML file** <br>Ready to embed via *iframe* tag or directly through the browser, every feature is included.
* **Customizable** <br>Set your own default [settings](settings.html).
* **API through URL GET parameters** <br>Override your default parameters through [URL GET parameters](api.html).
* **View** <br>Set a default [view](view.html) and override the map geographical center through [API](api.html)
* **Markers** <br>Add as much markers with latitude and longitude through URL GET parameters.
* **Marker clusters** <br>When markers density is to high, provides beautiful animated marker clustering.
* **Gesture handling** <br>Brings the basic functionality of Google Maps Gesture Handling into Leaflet. Prevents users from getting trapped on the map when scrolling a long page. 
* **Routing Machine** <br>Easy way to get distance and itinerary between multiple markers.
* **Autocomplete** <br>OpenStreetMap search engine available into a simple autocompletion list.
* **Permalink** <br>Permalink control button allows visitors to always get the direct link to the current view, useful to share the map view [Learn more](permalink.html)
* **Reset view** <br>Reset view control button allows visitors to go back to the very first view of their current session, or to the SEEMAP's default settings [Learn more](reset-view.html)

## Use cases

As a web developer/designer/redactor, you have multiple project onto which quickly embed map without reinstall and configure Leaflet and common plugins each time.

As a web developer/designer/redactor, you have one or multiple coordinates to quickly place on an embedded map.

The following code is the featured example:

```html
<!-- Include SEEMAP as an iframe tag -->
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
{:.playground title="SEEMAP"}
