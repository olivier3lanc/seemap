---
title: Settings
description: List and description of all available and editable default settings
layout: libdoc/page
order: 10
---

Here are the default settings located at the top of the page `seemap.html`, feel free to edit them according to your needs.

| Name | Default | Type | Description |
| :- | :- | :- | :- |
| lat | *46.3396952* | *Float* or *null* | Default latitude |
| lng | *2.6072057* | *Float* or *null* | Default longitude |
| zoom | *4* | *Integer* or *null* | Default map zoom level |
| zoomControl | *true* | *Boolean* | Enable or disable map zoom control |
| viewResetControl | *true* | *Boolean* | Enable or disable map view reset control |
| viewResetGoesToFirstView | *true* | *Boolean* | If true, the destination of view reset is the first view, if false, destination is based on user settings (lat, lng, zoom) |
| layer | *CartoDB_Voyager* | *String* | Default tile provider applied, [view all available](layers.html) |
| gesture | *true* | *Boolean* | Enable or disable gesture handling |
| fit | *true* | *Boolean* | Enable or disable automatic fit to the view of markers bounds |
| cluster | *true* | *Boolean* | Enable or disable marker cluster |
| routing | *false* | *Boolean* | Enable or disable routing by default - Requires at least 2 markers |
| autocomplete | *true* | *Boolean* | Enable or disable autocomplete search |
| autocompleteZoom | *12* | *Integer* or *null* | Zoom level applied on autocomplete selection |
| routingBackLineColor | *dodgerblue* | *String* | Routing style back line CSS color |
| routingBackLineOpacity | *0* |  *Number* | Routing style back line CSS opacity |
| routingBackLineWeight | *10* |  *Number* | Routing style back line CSS weight |
| routingMidLineColor | *dodgerblue* | *String* | Routing style middle line CSS color |
| routingMidLineOpacity | *0.5* | *Number* | Routing style middle line CSS opacity |
| routingMidLineWeight | *6* | *Number* | Routing style middle line CSS weight |
| routingFrontLineColor | *fuchsia* | *String* | Routing style front line CSS color |
| routingFrontLineOpacity | *1* | *Number* | Routing style front line CSS opacity |
| routingFrontLineWeight | *2* | *Number* | Routing style front line CSS weight |
| markerIconUrl | *data:image/svg+xml;base64, ...* | *String* | Marker icon URL, can be base64 (recommended) or public remote URL |
| markerIconSize | *[25, 40]* | *Array* | Marker icon size [x, y] in pixels |
| markerIconAnchor | *[12, 40]* | *Array* | Marker icon anchor position [x, y]. Origin is top left. |
| markerPopupAnchor | *[0, -40]* | *Array* | Marker popup anchor position [x, y]. Origin is bottom center. |
| markerShadowUrl | *data:image/png;base64,...* | *String* | Marker shadow URL, can be base64 (recommended) or public remote URL |
| markerShadowSize | *[25, 40]* | *Array* | Marker shadow size [x, y] in pixels |
| markerShadowAnchor | *[4, 40]* | *Array* | Marker shadow anchor position. Origin is top left. |
| language | *en_GB* | *String* | Interface language |
| i18n | - | *Object* | Object containing languages strings tokens |
