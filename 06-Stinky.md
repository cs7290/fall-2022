
# 06-Stinky

# Updated timeline

* [plan.md](plan.md)

# Stinky plan

* [Stinky Plan](https://observablehq.com/d/5b62069ac02499e1) -- notebook
  * Radial brush seems to be making progress
  * [Radial Area Chart](https://observablehq.com/@d3/radial-area-chart?collection=@d3/d3-shape)
  * Schools -- collected some data
* Submissions
  * [Stinky with MapLibre](https://observablehq.com/d/f6ad19f1d33ad186)
    * [Geocoding schools](https://observablehq.com/d/f305f4a853afe835)
  * [Stinkfinder Libre](https://observablehq.com/d/b9e12b358c4f1ee3@275) 
    * Uses the geocoding -- automatically creates dropdown with schools schools near Portland
    * Flies to selected school
  * [MapLibre Stinky](https://observablehq.com/d/08ecb9885b4b868c@197)
    * Heatmap -- still working on color scale for density
  * [Radial Histogram](https://observablehq.com/d/271570a96e6dcedf)
  * [Radial area chart with brush](https://observablehq.com/d/195b555c676fc016)
    * This is the "canonical version" as of this evening

## d3.area

* [d3-line](https://observablehq.com/@d3/d3-line?collection=@d3/d3-shape)
  * [D3 Area Chart](https://observablehq.com/@d3/area-chart)
  * A reusable chart that's built with d3.area() -- a D3 "area generator"
  * The [d3-shape](https://github.com/d3/d3-shape) module provides a variety of shape generators, including `d3.area()`
  * [d3-areaRadial()](https://github.com/d3/d3-shape#areaRadial) is also in the github API reference on github
* [d3.lineRadial](https://observablehq.com/@d3/d3-lineradial) -- observable notebook
  * the animation uses [now](https://observablehq.com/@observablehq/stdlib#nowSection), which is part of the [Standard Library](https://observablehq.com/@observablehq/stdlib)
  * the animation draws on canvas, which doesn't have selectable elements
  * to do the same thing on SVG, you'd use `d3.lineRadial()(spiral)` with a "path" element's "d" attribute
  * the canvas vs SVG distinction is clearer from the [d3-shape](https://github.com/d3/d3-shape) API reference on github
  * See: [Introducing D3 shape](https://medium.com/@mbostock/introducing-d3-shape-73f8367e6d12) (2015) by Mike Bostock
  * And: [Introucing D3 scale](https://medium.com/@mbostock/introducing-d3-scale-61980c51545f) (2015) by Mike Bostock
  * Don't forget string interpolation with Observable's [Hyptertext Literal](https://observablehq.com/@observablehq/htl)
* [d3-area](https://observablehq.com/d/7f87fe58cc0c81e5) -- my notebook with examples

## Pies

* [d3-pie](https://github.com/d3/d3-shape/blob/main/README.md#pies) -- d3.pie
  * The pie generator does not produce a shape directly, 
  * but instead computes the necessary angles to represent a tabular dataset as a pie or donut chart; 
  * these angles can then be passed to an arc generator.
* [Pie Settings](https://observablehq.com/@d3/pie-settings?collection=@d3/d3-shape) -- observable notebook
* [Pie Chart Update, II](https://bl.ocks.org/mbostock/1346410) -- mbostock bl.ock
* [donut transitions](https://bl.ocks.org/mbostock/4341417) -- a classic bl.ock from mbostock
