---
title: Settings
description: List and description of all available settings
layout: libdoc/page
---

Once [downloaded](installation-and-usage.html), edit the settings - located at the bottom of the page - according to your needs. Global principle is: Default settings can be overridden by URL GET parameters.

| Name | Type | Description |
| :- | :- | :- |
| lat | Float | Default latitude applied if no GET view parameter `view=` is set nor any marker |
| lng | Float | Default longitude applied if no GET view parameter `view=` is set nor any marker |
| zoom | Integer | Default zoom level applied if GET parameter `zoom=` is not set into URL |
| layer | String | Default tile provider applied - [view all](layers.html) - if GET parameter `layer=` is not set into URL |
| gesture | Boolean | Default [gesture handling](gesture-handling.html) setting applied if GET parameter `gesture=` is not set into URL |
| fit | Boolean | Default fit to markers bounds setting applied if GET parameter `fit=` is not set into URL |
| cluster | Boolean | Default [marker cluster](marker-cluster.html) setting applied if GET parameter `cluster=` is not set into URL |
| routing | Boolean | Default [routing](routing.html) setting applied if GET parameter `routing=` is not set into URL |
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
