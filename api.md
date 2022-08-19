---
title: API
description: Overridable default parameters through URL GET parameters and Leaflet instance
layout: libdoc/page
order: 100
---
* 
{:toc}

## URL GET parameters

Override your default settings through URL GET parameters:

| GET parameters and format | Description |
| :- | :- |
| `view=<lat>,<lng>` | Center the view to specified latitude and longitude.<br>Example:<br>[center view on Madagascar](seemap.html?view=-18.47960905583197,46.05468750000001){: target="_blank"} |
| `zoom=<Integer or null>` | Set the map zoom level.<br>Example:<br>[zoom in](seemap.html?zoom=12){: target="_blank"} |
| `zoomControl=<Integer>` | Enable or disable map zoom control.<br>Examples:<br>[Enable](seemap.html?zoomControl=true){: target="_blank"} or [Disable](seemap.html?zoomControl=false){: target="_blank"} |
| `viewResetControl=<Boolean>` | Enable or disable map view reset control.<br>Examples:<br>[Enable](seemap.html?viewResetControl=true){: target="_blank"} or [Disable](seemap.html?viewResetControl=false){: target="_blank"} |
| `viewResetGoesToFirstView=<Boolean>` | If true, the destination of view reset is the first view of the visitor. If false, destination is based on SEEMAP user settings (lat, lng, zoom).<br>Examples (move and zoom to see the difference):<br>[Enable](seemap.html?view=45,3&zoom=7&viewResetGoesToFirstView=true){: target="_blank"} or [Disable](seemap.html?view=45,3&zoom=7&viewResetGoesToFirstView=false){: target="_blank"} |
| `layer=<String>` | Set the tile provider. [View all](layers.html) <br>Example:<br>[Stamen_TonerLite](seemap.html?layer=Stamen_TonerLite){: target="_blank"} |
| `gesture=<Boolean>` | Enable or disable gesture handling.<br>Examples:<br>[Enable](seemap.html?gesture=true){: target="_blank"} or [Disable](seemap.html?gesture=false){: target="_blank"} |
| `fit=<Boolean>` | Enable or disable automatic fit to the view of markers bounds.<br>Examples:<br>[Enable](seemap.html?fit=true&marker=45,3&marker=46,2&marker=47,3){: target="_blank"} or [Disable](seemap.html?fit=false&marker=45,3&marker=46,2&marker=47,3){: target="_blank"} |
| `cluster=<Boolean>` | Enable or disable marker cluster.<br>Examples:<br>[Enable](seemap.html?cluster=true&marker=45,3&marker=46,2&marker=47,3&fit=false){: target="_blank"} or [Disable](seemap.html?cluster=false&marker=45,3&marker=46,2&marker=47,3&fit=false){: target="_blank"} <br>Note that *fit* is set to *false* to bypass auto fit to marker bounds, only to display a relevant demo of marker cluster |
| `routing=<Boolean>` | Enable or disable routing - Requires at least 2 markers.<br>Examples:<br>[Enable](seemap.html?routing=true&marker=45,3&marker=46,2){: target="_blank"} or [Disable](seemap.html?routing=false&marker=45,3&marker=46,2){: target="_blank"} |
| `autocomplete=<Boolean>` | Enable or disable autocomplete search.<br>Examples:<br>[Enable](seemap.html?autocomplete=true){: target="_blank"} or [Disable](seemap.html?autocomplete=false){: target="_blank"} |
| `autocompleteZoom=<Integer or null or false>` | Set or disable autocomplete map zoom level on autocompletion item click.<br>Example:<br>[Set to 8](seemap.html?autocompleteZoom=8){: target="_blank"} or [Disable](seemap.html?autocompleteZoom=false){: target="_blank"} |
| `language=<String>` |  Set the interface language.<br>Example:<br>[Set to french](seemap.html?language=fr_FR){: target="_blank"} |


## Leaflet instance

SEEMAP is a helper for Leaflet, the whole [Leaflet API](https://leafletjs.com/reference.html) of the instance is available at:

```javascript
seemap.instance
```

## Leaflet markers

All Leaflet markers are set at:

```javascript
seemap.markers
```

## SEEMAP methods

The SEEMAP specific helper methods.

### addMarker

Create a marker on the map.

```javascript
/**
  * @function addMarker
  * @description Create a marker on the map
  * @param {Object} options - Marker data
  * @param {Float} options.lat - The latitude of the marker
  * @param {Float} options.lng - The longitude of the marker
  * @param {String} options.content - The text or HTML of the marker popup
*/
seemap.addMarker(options)
```

Example of a marker creation:

```javascript
seemap.addMarker({
  lat: 45.12047878,
  lng: 2.389058,
  content: 'I am the marker popup content!'
})
```

### getCurrentViewSettings

Returns an object with all parameters applied for the current view.

```javascript
/**
 * @function getCurrentViewSettings
 * @description Returns an object with all parameters applied for the current view
 * @return {Object}
*/
seemap.getCurrentViewSettings()
```

Example returned

```javascript
{
  "center": {
    "lat": 45,
    "lng": 2.499999999999991
  },
  "zoom": 11,
  "zoomControl": true,
  "viewResetControl": true,
  "viewResetGoesToFirstView": true,
  "cluster": true,
  "layer": "OpenStreetMap_Mapnik",
  "gesture": false,
  "routing": true,
  "autocomplete": true,
  "autocompleteZoom": 12,
  "fit": true,
  "markers": [
    {
      "lat": 45,
      "lng": 3,
      "content": ""
    },
    {
      "lat": 45,
      "lng": 2,
      "content": ""
    }
  ],
  "language": "en_GB"
}
```

### getParameter

Get the specified URL search parameter. Returns empty string or value of the specified parameter.

```javascript
/**
 * @function getParameter
 * @description Get the specified URL search parameter 
 * @param {String} str - The parameter name
 * @return {String}
*/
seemap.getParameter(str)
```
### text

Returns SEEMAP interface text/message string from its specified id.

```javascript
/**
 * @function text
 * @description Returns SEEMAP interface text/message string from its specified id
 * @param {String} string_id - The id of the interface text element
 * @return {String}
*/
seemap.text(string_id)
```

### update

Initializes SEEMAP.

```javascript
/**
  * @function update
  * @description Initializes SEEMAP
*/
seemap.update()
```

### updatePermalink

Create the link to the view currently applied.

```javascript
/**
 * @function updatePermalink
 * @description Create the link to the view currently applied
 * @return {String}
*/
seemap.updatePermalink()
```
