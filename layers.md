---
title: Layers
description: Set your Leaflet tile provider
layout: libdoc/page-split
order: 100
---

SEEMAP comes with common [Leaflet tile providers](https://github.com/leaflet-extras/leaflet-providers) that are ready to be used without an API key. Just add the GET parameter `layer=<tileProviderName>` into the URL.

```html
<SEEMAP_FILE_URL>?layer=<tileProviderName>
```

Layers which do not require API key:

* [OpenStreetMap_Mapnik](seemap.html?layer=OpenStreetMap_Mapnik){: target="_blank"}
* [OpenStreetMap_DE](seemap.html?layer=OpenStreetMap_DE){: target="_blank"}
* [OpenStreetMap_CH](seemap.html?layer=OpenStreetMap_CH){: target="_blank"}
* [OpenStreetMap_France](seemap.html?layer=OpenStreetMap_France){: target="_blank"}
* [OpenStreetMap_HOT](seemap.html?layer=OpenStreetMap_HOT){: target="_blank"}
* [OpenStreetMap_BZH](seemap.html?layer=OpenStreetMap_BZH){: target="_blank"}
* [OPNVKarte](seemap.html?layer=OPNVKarte){: target="_blank"}
* [OpenTopoMap](seemap.html?layer=OpenTopoMap){: target="_blank"}
* [CyclOSM](seemap.html?layer=CyclOSM){: target="_blank"}
* [CartoDB_Voyager](seemap.html?layer=CartoDB_Voyager){: target="_blank"}
* [CartoDB_VoyagerLabelsUnder](seemap.html?layer=CartoDB_VoyagerLabelsUnder){: target="_blank"}
* [CartoDB_Positron](seemap.html?layer=CartoDB_Positron){: target="_blank"}
* [CartoDB_PositronNoLabels](seemap.html?layer=CartoDB_PositronNoLabels){: target="_blank"}
* [CartoDB_DarkMatter](seemap.html?layer=CartoDB_DarkMatter){: target="_blank"}
* [CartoDB_VoyagerNoLabels](seemap.html?layer=CartoDB_VoyagerNoLabels){: target="_blank"}
* [GeoportailFrance_plan](seemap.html?layer=GeoportailFrance_plan){: target="_blank"}
* [GeoportailFrance_orthos](seemap.html?layer=GeoportailFrance_orthos){: target="_blank"}
* [Stamen_TonerLite](seemap.html?layer=Stamen_TonerLite){: target="_blank"}
* [Stamen_Terrain](seemap.html?layer=Stamen_Terrain){: target="_blank"}
* [Stamen_Watercolor](seemap.html?layer=Stamen_Watercolor){: target="_blank"}
* [Esri_WorldStreetMap](seemap.html?layer=Esri_WorldStreetMap){: target="_blank"}
* [Esri_DeLorme](seemap.html?layer=Esri_DeLorme){: target="_blank"}
* [Esri_WorldTopoMap](seemap.html?layer=Esri_WorldTopoMap){: target="_blank"}
* [Esri_WorldImagery](seemap.html?layer=Esri_WorldImagery){: target="_blank"}
* [Esri_WorldTerrain](seemap.html?layer=Esri_WorldTerrain){: target="_blank"}
* [Esri_WorldShadedRelief](seemap.html?layer=Esri_WorldShadedRelief){: target="_blank"}
* [Esri_OceanBasemap](seemap.html?layer=Esri_OceanBasemap){: target="_blank"}
* [Esri_NatGeoWorldMap](seemap.html?layer=Esri_NatGeoWorldMap){: target="_blank"}
* [Esri_WorldGrayCanvas](seemap.html?layer=Esri_WorldGrayCanvas){: target="_blank"}
* [MtbMap](seemap.html?layer=MtbMap){: target="_blank"}
* [NASAGIBS_ViirsEarthAtNight2012](seemap.html?layer=NASAGIBS_ViirsEarthAtNight2012){: target="_blank"}
* [USGS_USTopo](seemap.html?layer=USGS_USTopo){: target="_blank"}
* [USGS_USImagery](seemap.html?layer=USGS_USImagery){: target="_blank"}
* [USGS_USImageryTopo](seemap.html?layer=USGS_USImageryTopo){: target="_blank"}

Paid layers which are free to use locally for development purpose:

* [Stadia_AlidadeSmooth](seemap.html?layer=Stadia_AlidadeSmooth){: target="_blank"}
* [Stadia_AlidadeSmoothDark](seemap.html?layer=Stadia_AlidadeSmoothDark){: target="_blank"}
* [Stadia_OSMBright](seemap.html?layer=Stadia_OSMBright){: target="_blank"}
* [Stadia_Outdoors](seemap.html?layer=Stadia_Outdoors){: target="_blank"}

Presets of paid layers which require API keys are ready to be used: Enter your own API key into seemap.html at the specified tile provider object into `seemap.defaults.layers.TILE_PROVIDER`

* [Thunderforest_OpenCycleMap](seemap.html?layer=Thunderforest_OpenCycleMap){: target="blank"}
* [Thunderforest_Transport](seemap.html?layer=Thunderforest_Transport){: target="blank"}
* [Thunderforest_SpinalMap](seemap.html?layer=Thunderforest_SpinalMap){: target="blank"}
* [Thunderforest_Landscape](seemap.html?layer=Thunderforest_Landscape){: target="blank"}
* [Thunderforest_Outdoors](seemap.html?layer=Thunderforest_Outdoors){: target="blank"}
* [Thunderforest_Pioneer](seemap.html?layer=Thunderforest_Pioneer){: target="blank"}
* [Thunderforest_MobileAtlas](seemap.html?layer=Thunderforest_MobileAtlas){: target="blank"}
* [Thunderforest_Neighbourhood](seemap.html?layer=Thunderforest_Neighbourhood){: target="blank"}
* [Jawg_Streets](seemap.html?layer=Jawg_Streets){: target="blank"}
* [Jawg_Terrain](seemap.html?layer=Jawg_Terrain){: target="blank"}
* [Jawg_Sunny](seemap.html?layer=Jawg_Sunny){: target="blank"}
* [Jawg_Dark](seemap.html?layer=Jawg_Dark){: target="blank"}
* [Jawg_Matrix](seemap.html?layer=Jawg_Matrix){: target="blank"}


```html
<iframe src="../../seemap.html"></iframe>
<nav id="selects">
    <label for="no-api-required">NO API KEY REQUIRED</label>
    <select id="no-api-required" onchange="document.querySelector('iframe').src = this.value">
        <option value="../../seemap.html">Default</option>
        <option value="../../seemap.html?layer=OpenStreetMap_Mapnik">OpenStreetMap_Mapnik</option>
        <option value="../../seemap.html?layer=OpenStreetMap_DE">OpenStreetMap_DE</option>
        <option value="../../seemap.html?layer=OpenStreetMap_CH">OpenStreetMap_CH</option>
        <option value="../../seemap.html?layer=OpenStreetMap_France">OpenStreetMap_France</option>
        <option value="../../seemap.html?layer=OpenStreetMap_HOT">OpenStreetMap_HOT</option>
        <option value="../../seemap.html?layer=OpenStreetMap_BZH">OpenStreetMap_BZH</option>
        <option value="../../seemap.html?layer=OPNVKarte">OPNVKarte</option>
        <option value="../../seemap.html?layer=OpenTopoMap">OpenTopoMap</option>
        <option value="../../seemap.html?layer=CyclOSM">CyclOSM</option>
        <option value="../../seemap.html?layer=CartoDB_Voyager">CartoDB_Voyager</option>
        <option value="../../seemap.html?layer=CartoDB_VoyagerLabelsUnder">CartoDB_VoyagerLabelsUnder</option>
        <option value="../../seemap.html?layer=CartoDB_Positron">CartoDB_Positron</option>
        <option value="../../seemap.html?layer=CartoDB_PositronNoLabels">CartoDB_PositronNoLabels</option>
        <option value="../../seemap.html?layer=CartoDB_DarkMatter">CartoDB_DarkMatter</option>
        <option value="../../seemap.html?layer=CartoDB_VoyagerNoLabels">CartoDB_VoyagerNoLabels</option>
        <option value="../../seemap.html?layer=GeoportailFrance_plan">GeoportailFrance_plan</option>
        <option value="../../seemap.html?layer=GeoportailFrance_orthos">GeoportailFrance_orthos</option>
        <option value="../../seemap.html?layer=Stamen_TonerLite">Stamen_TonerLite</option>
        <option value="../../seemap.html?layer=Stamen_Terrain">Stamen_Terrain</option>
        <option value="../../seemap.html?layer=Stamen_Watercolor">Stamen_Watercolor</option>
        <option value="../../seemap.html?layer=Esri_WorldStreetMap">Esri_WorldStreetMap</option>
        <option value="../../seemap.html?layer=Esri_DeLorme">Esri_DeLorme</option>
        <option value="../../seemap.html?layer=Esri_WorldTopoMap">Esri_WorldTopoMap</option>
        <option value="../../seemap.html?layer=Esri_WorldImagery">Esri_WorldImagery</option>
        <option value="../../seemap.html?layer=Esri_WorldTerrain">Esri_WorldTerrain</option>
        <option value="../../seemap.html?layer=Esri_WorldShadedRelief">Esri_WorldShadedRelief</option>
        <option value="../../seemap.html?layer=Esri_OceanBasemap">Esri_OceanBasemap</option>
        <option value="../../seemap.html?layer=Esri_NatGeoWorldMap">Esri_NatGeoWorldMap</option>
        <option value="../../seemap.html?layer=Esri_WorldGrayCanvas">Esri_WorldGrayCanvas</option>
        <option value="../../seemap.html?layer=MtbMap">MtbMap</option>
        <option value="../../seemap.html?layer=NASAGIBS_ViirsEarthAtNight2012">NASAGIBS_ViirsEarthAtNight2012</option>
        <option value="../../seemap.html?layer=USGS_USTopo">USGS_USTopo</option>
        <option value="../../seemap.html?layer=USGS_USImagery">USGS_USImagery</option>
        <option value="../../seemap.html?layer=USGS_USImageryTopo">USGS_USImageryTopo</option>
    </select>

    <label for="local-api">API KEY REQUIRED BUT WORKS LOCALLY</label>
    <select id="local-api" onchange="document.querySelector('iframe').src = this.value">
        <option value="../../seemap.html">Default</option>
        <option value="../../seemap.html?layer=Stadia_AlidadeSmooth">Stadia_AlidadeSmooth</option>
        <option value="../../seemap.html?layer=Stadia_AlidadeSmoothDark">Stadia_AlidadeSmoothDark</option>
        <option value="../../seemap.html?layer=Stadia_OSMBright">Stadia_OSMBright</option>
        <option value="../../seemap.html?layer=Stadia_Outdoors">Stadia_Outdoors</option>
    </select>

    <label for="api-required">API KEY REQUIRED</label>
    <select id="api-required" onchange="document.querySelector('iframe').src = this.value">
        <option value="../../seemap.html">Default</option>
        <option value="../../seemap.html?layer=Thunderforest_OpenCycleMap">Thunderforest_OpenCycleMap</option>
        <option value="../../seemap.html?layer=Thunderforest_Transport">Thunderforest_Transport</option>
        <option value="../../seemap.html?layer=Thunderforest_SpinalMap">Thunderforest_SpinalMap</option>
        <option value="../../seemap.html?layer=Thunderforest_Landscape">Thunderforest_Landscape</option>
        <option value="../../seemap.html?layer=Thunderforest_Outdoors">Thunderforest_Outdoors</option>
        <option value="../../seemap.html?layer=Thunderforest_Pioneer">Thunderforest_Pioneer</option>
        <option value="../../seemap.html?layer=Thunderforest_MobileAtlas">Thunderforest_MobileAtlas</option>
        <option value="../../seemap.html?layer=Thunderforest_Neighbourhood">Thunderforest_Neighbourhood</option>
        <option value="../../seemap.html?layer=Jawg_Streets">Jawg_Streets</option>
        <option value="../../seemap.html?layer=Jawg_Terrain">Jawg_Terrain</option>
        <option value="../../seemap.html?layer=Jawg_Sunny">Jawg_Sunny</option>
        <option value="../../seemap.html?layer=Jawg_Dark">Jawg_Dark</option>
        <option value="../../seemap.html?layer=Jawg_Matrix">Jawg_Matrix</option>
    </select>
</nav>
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
    #selects {
        position: fixed;
        top: 1em;
        right: 1em;
        max-width: 16em;
    }
    label, select {
        display: block;
        width: 100%;
    }
    label {
        font-size: 10px;
        font-family: -apple-system, BlinkMacSystemFont, avenir next, avenir, segoe ui, helvetica neue, helvetica, Cantarell, Ubuntu, roboto, noto, arial, sans-serif; 
        font-weight: bold;
        padding: 0.5em;
        background-color: #FFF;
    }
    select {
        margin-bottom: 1em;
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
