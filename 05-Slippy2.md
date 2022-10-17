
# 05-Slippy2

## Goals

* Review submissions (MapLibre + interactive filter with `Inputs.range()`)
  * Create an interactive SVG layer (if one hasn't already been submitted)
* Review the MapLibre capabilities
  * Introduce animation
* Create an interactive stinky demo that showcases key features
  * Create a project plan then divvy up the goals

## Demo goal

Goal for today is to create a prototype that showcases key features

* Create a UI that makes it super easy to showcase key features in the dataset
* Locations -- for example, South Portland, West End
* Consider highlighting schools
* Filter key elements in the data, e.g., southerly winds and west-end complaints

## Review submissions

* TODO #1 

## MapLibre Basics

* [Hello, MapLibre](https://observablehq.com/@pbogden/hello-maplibre)
* Note how you get a handle to the map object

## Interactive filter

You have 2 choices with WebGL maps, each with some pros & cons...

* (1) Use the map application's API and fina a good use case
  * [Earthquakes on MapLibre](https://maplibre.org/maplibre-gl-js-docs/example/timeline-animation/) -- maplibre.org
    * Uses the API to create a map layer
    * Map has an "input" eventlistener that filters the visible quakes
  * [Earthquakes on MapLibre](https://observablehq.com/d/6cc3d08406450b42)
    * Observable version of the MapLibre demo
    * Doesn't use [Observable Inputs](https://observablehq.com/@observablehq/inputs) -- my notebook
* (2) Add a custom SVG layer, then you get direct access to the data
  * For example: [D3 + Leaflet](https://bost.ocks.org/mike/leaflet/) (the classic) -- bost.ocks.org
    * Adds an SVG to the map (custom layer!)
    * There have been many more modern implementations of this classic.
  * [Maplibre stinky](https://observablehq.com/d/d0d6b1f28ef7e5a5)
    * Uses the same technique (custom SVG layer)
    * Have yet to implement the interaction, but we've done that already with brushable earthquakes.

## Synchronized inputs

This is mostly FYI

* [Synchronized Inputs](https://observablehq.com/@observablehq/synchronized-inputs)

## Layers and mouse events

This addresses a question from the last assignment

* [MapLibre Layers](https://observablehq.com/d/3eeba0a0e28dd063)

## Fly To

This uses a built in map animation

* [Hello, MapLibre](https://observablehq.com/@neocartocnrs/hello-maplibre)
  * We saw this last time
  * Shows how to add a marker (using the API)
  * Shows how to use "Fly To" -- (with hard-wired geocoder)
* [Mapbox Fly To](https://observablehq.com/@mbostock/mapbox-fly-to) -- mbostock notebook
  * Note the container.value in mbostock's notebook
  * Note also [Invalidation](https://observablehq.com/@observablehq/invalidation)
    * frees up resources when the cell is re-evaluated
  * [Invalidation](https://observablehq.com/@fil/invalidation)
    * This has a nice visualization of invalidation, or lack thereof

## Animation

This is general animation -- several methods, each with its own pros & cons

* [Animation Loops](https://observablehq.com/@observablehq/animation-loops)

## Stinky

* [MapLibre stinky](https://observablehq.com/d/d0d6b1f28ef7e5a5)
  * TODO #2 -- Create a project plan for the prototype
  * TODO #3 -- Start on it...
