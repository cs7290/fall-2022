
# 03-Brush

# Homework

* Set up a github pages site
* Raw HTML recommended
* [stinky2](ds5110.github.io/stinky2)

# Vote

Collect the candidates

## Case study

* Remarkable cartography: Projection transitions](https://observablehq.com/@d3/projection-transitions)

# Brushable earthquakes

### Step 1 -- Airports to Earthquakes

* [World Airports](https://observablehq.com/@pbogden/earthquakes)
* Get the earthquake data
  * `d3.json('https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/2.5_month.geojson')`
* Get the earthquakes
  ```
  quakes = data.features.map(d => ({
        name: d.properties.title,
        longitude: d.geometry.coordinates[0],
        latitude: d.geometry.coordinates[1],
        datum: d, // Save a copy of the entire earthquake datum for other data-driven features
    }))
  ```
* Get the world map with earthquakes instead of airports
  * `import {map} with {quakes as data} from "@d3/world-airports"`

### Step 2 -- Earthquakes with projection

* [d3-geo](https://observablehq.com/collection/@d3/d3-geo) collection
* [d3-geo-projection](https://observablehq.com/collection/@d3/d3-geo-projection) collection

### Step 3 -- Earthquakes with style

* You did this already?

### Step 4 -- Add a range slider

* [Introduction to views](https://observablehq.com/@observablehq/views)
* First "view" demo is an [Observable range input](https://observablehq.com/@observablehq/input-range)
* This other demos show how to create a "view" out of just about any DOM element
* What's a DOM? See: [Introduction to HTML](https://observablehq.com/@observablehq/introduction-to-html)
* Note that the rendered DOM elements all use the "viewof" keyword
* [A brief introduction to viewof](https://observablehq.com/@observablehq/a-brief-introduction-to-viewof)

### Step 5 -- Create a brush view

* [Brushable Scatterplot Matrix](https://observablehq.com/@d3/brushable-scatterplot-matrix?collection=@d3/d3-brush)
  * Just try doing this with [Seaborn!](https://seaborn.pydata.org/examples/scatterplot_matrix.html)
* Earthquake hint: [Focus + Context](https://observablehq.com/@d3/focus-context?collection=@d3/d3-brush)
* Start with [Click to recenter brush](https://observablehq.com/@d3/click-to-recenter-brush)
* Some new components that you may want to grok
  * [d3-scale](https://github.com/d3/d3-scale)
  * [d3-scale](https://observablehq.com/collection/@d3/d3-scale) -- collection
  * [d3-axis](https://github.com/d3/d3-axis)
  * [d3-axis](https://observablehq.com/collection/@d3/d3-axis) -- collection
  * d3.pointer events in [d3-selection-2-0](https://observablehq.com/@d3/d3-selection-2-0) 
  * [event listeners](https://observablehq.com/@mbostock/event-listeners)
* Data are generated with a random number generator -- need to turn this into earthquake data
  * Expose the data element so it can be overridden
* Fix the initial condition, which is hard-wired to [3, 5]

### Step 6 -- Add a brush to the earthquakes (linked)

* This should be minor modification of Step 4 using result from Step 5

# Next

* Embedding into a website
* Slippy map -- MapLibre
