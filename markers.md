---
title: Markers
description: Adding multiple a single markers on the map through URL GET parameters
layout: libdoc/page-split
---

Multiple markers can be set just by repeating [single marker](marker.html) process.

```html
<SEEMAP_FILE_URL>?marker=<lat1>,<lng1>[,<popup content1>]&marker=<lat2>,<lng2>[,<popup content2>]...
```

```html
<iframe src="../seemap.html?marker=9.560848765401868,21.086687601255335,Africa&marker=47.5560319708231,7.587505743403426,Europe&marker=49.00152071512122,-98.18920038991718,North America&marker=-7.234993322606072,-58.15254292353319,South America&marker=58.07674787016387,93.90539734591425,Asia&marker=-25.16710479424436,134.68664734591425,Oceania&marker=-78.49097744719846,8.124147345914253,Antartica"></iframe>
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
{:.playground title="Multiple markers"}
