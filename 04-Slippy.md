
# 04-Slippy

* Embedding
* Introduce slippy maps
* Interact with data added to slippy maps

## Brushable earthquakes

* Review results from brushable-earthquakes assignment
* My [Brushable Earthquakes](https://observablehq.com/@pbogden/brushable-earthquakes)
* [Click to Recenter Brush II](https://observablehq.com/@pbogden/click-to-recenter-brush-ii)
  * A couple changes made so that it's reusable
  * Among other things -- creates a data array using "await" when fetching the data
  * See discussion of promises below
* [Human-Induced Earthquakes](https://observablehq.com/@pbogden/man-made-earthquakes?collection=@pbogden/earthquakes)

## Promises

* [Introduction to Promises](https://observablehq.com/@observablehq/introduction-to-promises)
  * "A promise represents a value that is not yet known"
  * "Promises are often not created by you. Instead, an asynchronous library method might return a promise, and you need to wait for the promise to resolve (or reject)."
  * "D3’s d3.csv is just such a function: it fetches a file from another server, parsing comma-separated values into a structured array of objects. d3.csv can’t return the array right away, so it instead returns a Promise."
  * [Did you see the promise?](https://observablehq.com/@observablehq/introduction-to-promises#cell-71)
    * "Observable implicitly awaits promises across cell boundaries"...
    * "so you often don’t need to deal with a promise directly."
    * "**Cells can return promises**,"... 
    * "and **other cells can simply refer to the values and they’ll run when the promise resolves**."
  * [You can use the `await` keyword](https://observablehq.com/@observablehq/introduction-to-promises#cell-112)
    * "The implicit await of promises only happens across cell boundaries. 
    * **Gotcha**: "So, if you create a promise and then refer to it within the same cell, you’ll see the Promise object and not the resolved value."
  * You can use await to pause execution or (equivalently) you can use Promise.then() to chain promises
* [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) -- MDN
  * Promises are part of JavaScript (HTML5)
  * [Using Promises](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises) -- MDN
  * Observablehq makes promises relatively intuitive.

## Embedding Notebooks

* [Embedding Notebooks](https://observablehq.com/collection/@observablehq/embedding-notebooks) -- collection
  * Collection with the following notebooks...
* [Introduction to Embedding](https://observablehq.com/@observablehq/embeds)
  * iframe embedding into an HTML page
  ```
  <!DOCTYPE html>
  <body>
  <iframe width="100%" height="635" frameborder="0"
    src="https://observablehq.com/embed/@d3/sortable-bar-chart?cell=viewof+order&cell=chart"></iframe>
  ```
* Demo -- create an "index.html" file containing the code above and then run the following from the command line
  ```
  python -m http.server
  ```
  Then browse to http://localhost:8000
* Ref: [http.server](https://docs.python.org/3/library/http.server.html) -- python.org
* [Advanced embedding and downloading](https://observablehq.com/@observablehq/advanced-embeds)
  * 3-circles demo shows how to get the "Runtime with JavaScript" embedding code
  * Mentions using the version to lock the embed code
  * "Rendering Cells"
    * The "My Neat Notebook" demo notebook: https://observablehq.com/@jashkenas/my-neat-notebook
    * talks about importance of rendering all cells on which the visualization depends
    * side effects must "return true" if they don't actually render into a cell

## Step 1: Stinky2 -- Under the hood

Investigate what's going on in the source

* Where's the map being injected?
  * observablehq-map-c6323fcd
  * observablehq-brush-c6323fcd
* Where's the map coming from?
  * This is the one -- 095056cccbc4d2e6
  * https://observablehq.com/d/095056cccbc4d2e6
* Note that my notebook isn't the published version
  * https://observablehq.com/d/095056cccbc4d2e6@678 (this is published version as of 3 Oct)

## Zoomable Raster & Vector

* [Zoomable Raster & Vector](https://observablehq.com/@d3/zoomable-raster-vector)
* [d3-tile](https://observablehq.com/collection/@d3/d3-tile) -- collection
  * This is looking under the hood
* [d3-zoom](https://observablehq.com/@d3/zoomable-raster-vector?collection=@d3/d3-zoom)
  * Ditto

## Slippy Maps

* [Hello, Leaflet](https://observablehq.com/@observablehq/hello-leaflet)
  * [Leaflet](https://observablehq.com/@tmcw/leaflet)
* [Hello, Mapbox GL](https://observablehq.com/@observablehq/hello-mapbox-gl)
* [Hello, MapLibre](https://observablehq.com/@neocartocnrs/hello-maplibre)
* [Hello, Deck.gl](https://observablehq.com/@pbogden/hello-deck-gl)
  * [Deck.gl playground](https://observablehq.com/@pessimistress/deck-gl-playground)

## Earthquakes on Leaflet

* [D3 + Leaflet](https://bost.ocks.org/mike/leaflet/) -- the classic
* [D3 + Leaflet](https://observablehq.com/@pbogden/d3-leaflet?collection=@pbogden/leaflet) -- ported to Observable
* [Dots on a map: setup-gl](https://bl.ocks.org/enjalot/dc1ce756527c072885dc) -- enjalot bl.ock
* [Mapbox + D3 SVG overlay](https://bl.ocks.org/enjalot/dc1ce756527c072885dc) -- enjalot gist
* [D3 + Mapbox](https://observablehq.com/@john-guerra/mapbox-d3) -- john-guerra notebook

## Exercise -- Earthquakes on MapLibre

* Add earthquakes to the MapLibre map
  * Leaflet and MapLibre have similar APIs.
  * This presents one approach -- it's a classic: [D3 + Leaflet](https://bost.ocks.org/mike/leaflet/)
  * This might be helpful: [Earthquakes on Leaflet](https://observablehq.com/@pbogden/earthquakes-on-leaflet)
* Add an interactive filter with [Inputs.range()](https://github.com/observablehq/inputs#Range)

## Looking ahead

* Programmatic interactions with the map


