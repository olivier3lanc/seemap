---
title: Markers clusters
description: Get beautiful animated marker clustering
layout: libdoc/page
---
SEEMAP integrates [Leaflet Marker Cluster](https://github.com/Leaflet/Leaflet.markercluster).

If [default marker cluster](settings.html) is set to `true`, just add GET parameter `cluster=false` to disable marker cluster.

If default marker cluster is set to `false`, just add GET parameter `cluster=true` to enable marker cluster.


```html
<iframe src="../seemap.html?marker=48.852855084244275,2.3482764253351434,Paris&marker=47.05692600913301,2.309900469185777&marker=43.348569315109174,5.374661932049889,Marseille&zoom=2"></iframe>
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
{:.playground title="With marker cluster"}

```html
<iframe src="../seemap.html?cluster=false&marker=48.852855084244275,2.3482764253351434,Paris&marker=47.05692600913301,2.309900469185777&marker=43.348569315109174,5.374661932049889,Marseille&zoom=2"></iframe>
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
{:.playground title="Without marker cluster"}

