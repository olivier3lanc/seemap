---
title: Reset view
description: Reinitialize the view of the map
layout: libdoc/page
order: 790
---
Reset view control button allows visitors to go back to the very first view of their current session, or to the SEEMAP's default settings. 

On the following example, navigate and zoom through maps and click on the reset view/home button to see the difference.

```html
<iframe src="../../seemap.html?view=45.433153642271414,6.690673828125001&zoom=7"></iframe>
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
{:.playground title="Reset to the first view (default)<br><sup>Navigate, zoom and click on home button.</sup>"}

```html
<iframe src="../../seemap.html?viewResetGoesToFirstView=false&view=45.433153642271414,6.690673828125001&zoom=7"></iframe>
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
{:.playground title="Reset to defaults<br><sup>Navigate, zoom and click on home button.</sup>"}
