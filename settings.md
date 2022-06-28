---
title: Settings
description: List and description of all available settings
layout: libdoc/page
---

[Download SEEMAP](installation-and-usage.html), adjust the default settings located at the top of the page according to your needs.


## Overridable parameters

| Name | Type | GET parameter | Description |
| :- | :- | :- | :- |
| lat | Float | `?lat=<Float>` | Latitude applied if no GET view parameter `view=` is set nor any marker |
| lng | Float | `?lng=<Float>` | Longitude applied if no GET view parameter `view=` is set nor any marker |
| zoom | Integer | `?zoom=<Number>` | Zoom level |
| layer | String | `?layer=<LAYER_NAME>` | Tile provider applied - [view all](layers.html) |
| gesture | Boolean | `?gesture=<true or false>` | [Gesture handling](gesture-handling.html) |
| fit | Boolean | `?fit=<true or false>` | Fit to markers bounds |
| cluster | Boolean | `?cluster=<true or false>` | [Marker cluster](marker-cluster.html) |
| routing | Boolean | `?routing=<true or false>` | [Routing](routing.html) |
| autocomplete | Boolean | `?autocomplete=<true or false>` | [Autocomplete](autocomplete.html) |

## Others parameters

| Name | Type | Description |
| :- | :- | :- |
| routingBackLineColor | String | Routing style back line CSS color |
| routingBackLineOpacity | Float | Routing style back line CSS opacity |
| routingBackLineWeight | Integer | Routing style back line CSS weight |
| routingMidLineColor | String | Routing style middle line CSS color |
| routingMidLineOpacity | Float | Routing style middle line CSS opacity |
| routingMidLineWeight | Integer | Routing style middle line CSS weight |
| routingFrontLineColor | String | Routing style front line CSS color |
| routingFrontLineOpacity | Float | Routing style front line CSS opacity |
| routingFrontLineWeight | Integer | Routing style front line CSS weight |
| markerIconUrl | String | Marker icon URL, can be base64 (recommended) or public remote URL |
| markerIconSize | Array | Marker icon size [x, y] in pixels |
| markerIconAnchor | Array | Marker icon anchor position [x, y]. Origin is top left. |
| markerPopupAnchor | Array | Marker icon anchor position [x, y]. Origin is top left. |
| markerShadowUrl | String | Shadow icon URL, can be base64 (recommended) or public remote URL |
| markerShadowSize | Array | Marker shadow size [x, y] in pixels |
| markerShadowAnchor | Array | Marker shadow anchor position [x, y]. Origin is top left. |
