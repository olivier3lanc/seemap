---
title: API
description: Overridable default parameters through URL GET parameters and Leaflet instance
layout: libdoc/page
---

## URL GET parameters

Override your default settings through URL GET parameters:

| GET parameters and format | Description | Examples |
| :- | :- | :- |
| `view=<lat>,<lng>` | Center the view to specified latitude and longitude | [center view on Madagascar](seemap.html?view=-18.47960905583197,46.05468750000001){: target="_blank"} |
| `zoom=<Integer>` | Set the map zoom level | [zoom in](seemap.html?zoom=12){: target="_blank"} |
| `zoomControl=<Integer>` | Enable or disable map zoom control | [Enable](seemap.html?zoomControl=true){: target="_blank"} [Disable](seemap.html?zoomControl=false){: target="_blank"} |
| `layer=<String>` | Set the tile provider | [OpenStreetMap_Mapnik](seemap.html?layer=OpenStreetMap_Mapnik){: target="_blank"} |
| `gesture=<Boolean>` | Enable or disable gesture handling | [Enable](seemap.html?gesture=true){: target="_blank"} [Disable](seemap.html?gesture=false){: target="_blank"} |
| `fit=<Boolean>` | Enable or disable automatic fit to the view of markers bounds | [Enable](seemap.html?fit=true&marker=45,3&marker=46,2&marker=47,3){: target="_blank"} [Disable](seemap.html?fit=false&marker=45,3&marker=46,2&marker=47,3){: target="_blank"} |
| `cluster=<Boolean>` |  Enable or disable marker cluster | [Enable](seemap.html?cluster=true&marker=45,3&marker=46,2&marker=47,3&fit=false){: target="_blank"} [Disable](seemap.html?cluster=false&marker=45,3&marker=46,2&marker=47,3&fit=false){: target="_blank"} - Note that *fit* is set to *false* to bypass auto fit to marker bounds, only to display a relevant demo of marker cluster |
| `routing=<Boolean>` |  Enable or disable routing by default - Requires at least 2 markers | [Enable](seemap.html?routing=true&marker=45,3&marker=46,2){: target="_blank"} [Disable](seemap.html?routing=false&marker=45,3&marker=46,2){: target="_blank"} |
| `autocomplete=<Boolean>` |  Enable or disable autocomplete search | [Enable](seemap.html?autocomplete=true){: target="_blank"} [Disable](seemap.html?autocomplete=false){: target="_blank"} |


## Leaflet instance

```javascript
seemap.instance
```

## Leaflet markers

```javascript
seemap.markers
```
