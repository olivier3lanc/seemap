---
title: Layers
description: Set your Leaflet tile provider
layout: libdoc/page-split
---

SEEMAP comes with common [Leaflet tile providers](https://github.com/leaflet-extras/leaflet-providers) that are ready to be used without an API key. Just add the GET parameter `layer=tileProviderName` into the URL.

```html
<SEEMAP_FILE_URL>?layer=<tileProviderName>
```

 Here are the available tile providers:

* OpenStreetMap_Mapnik
* OpenStreetMap_DE
* OpenStreetMap_CH
* OpenStreetMap_France
* OpenStreetMap_HOT
* OpenStreetMap_BZH
* OPNVKarte
* OpenTopoMap
* CyclOSM
* CartoDB_Voyager
* GeoportailFrance_plan
* GeoportailFrance_orthos
* Stamen_TonerLite
* Stamen_Terrain
* Stamen_Watercolor

```html
<iframe src="../seemap.html"></iframe>
<select onchange="document.querySelector('iframe').src = this.value">
    <option value="../seemap.html?layer=OpenStreetMap_Mapnik">OpenStreetMap_Mapnik</option>
    <option value="../seemap.html?layer=OpenStreetMap_DE">OpenStreetMap_DE</option>
    <option value="../seemap.html?layer=OpenStreetMap_CH">OpenStreetMap_CH</option>
    <option value="../seemap.html?layer=OpenStreetMap_France">OpenStreetMap_France</option>
    <option value="../seemap.html?layer=OpenStreetMap_HOT">OpenStreetMap_HOT</option>
    <option value="../seemap.html?layer=OpenStreetMap_BZH">OpenStreetMap_BZH</option>
    <option value="../seemap.html?layer=OPNVKarte">OPNVKarte</option>
    <option value="../seemap.html?layer=OpenTopoMap">OpenTopoMap</option>
    <option value="../seemap.html?layer=CyclOSM">CyclOSM</option>
    <option value="../seemap.html?layer=CartoDB_Voyager">CartoDB_Voyager</option>
    <option value="../seemap.html?layer=GeoportailFrance_plan">GeoportailFrance_plan</option>
    <option value="../seemap.html?layer=GeoportailFrance_orthos">GeoportailFrance_orthos</option>
    <option value="../seemap.html?layer=Stamen_TonerLite">Stamen_TonerLite</option>
    <option value="../seemap.html?layer=Stamen_Terrain">Stamen_Terrain</option>
    <option value="../seemap.html?layer=Stamen_Watercolor">Stamen_Watercolor</option>
</select>
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
    select {
        position: fixed;
        top: 1em;
        right: 1em;
    }
</style>
```
{:.playground title="Layers ready to use"}

## Add your own layer

Simply add your layers into the object `seemap.defaults.layers` just like others.

```javascript
const seemap = {
    defaults: {
        layers: {
            OpenStreetMap_Mapnik: L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
                maxZoom: 19,
                attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
            }),
            OpenStreetMap_DE: L.tileLayer('https://{s}.tile.openstreetmap.de/{z}/{x}/{y}.png', {
                maxZoom: 18,
                attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
            }),
            layer_id: L.tileLayer('https://{s}.your.tileprovider.org/{z}/{x}/{y}.png', {
                maxZoom: 19,
                attribution: '&copy; <a href="https://www.tileprovider.org/copyright">Your copyright</a> etc'
            })
        }
    }
}
```

Then apply the `layer_id` into SEEMAP settings:

```javascript
const seemap = {
    defaults: {
        //...
        layer: 'layer_id'
        //...
    }
}
```
