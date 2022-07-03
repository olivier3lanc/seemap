---
title: API
description: Overridable default parameters through URL GET parameters and Leaflet instance
layout: libdoc/page
---

## URL GET parameters

Override your default settings through URL GET parameters:

| GET parameters and format | Description | Examples |
| :- | :- | :- |
| `view=<lat>,<lng>` | Center the view to specified latitude and longitude | [view](seemap.html?view=45.123456,3.456789){: target="_blank"} |


| zoom | *2* | *Integer* or *null* | Default map zoom level |
| layer | *CartoDB_Voyager* | *String* | Default tile provider applied, [view all available](layers.html) |
| gesture | *true* | *Boolean* | Enable or disable gesture handling |
| fit | *true* | *Boolean* | Enable or disable automatic fit to the view of markers bounds |
| cluster | *true* | *Boolean* | Enable or disable marker cluster |
| routing | *false* | *Boolean* | Enable or disable routing by default - Requires at least 2 markers |
| autocomplete | *true* | *Boolean* | Enable or disable autocomplete search |

## Leaflet instance

