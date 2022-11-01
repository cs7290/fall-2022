
# 07-Embed

Embedding with style

## Assignment (due 7 Nov)

Choose one or more of the following projects...

* bioscience map
  * create a notebook to create an interactive map map of mainefrom [this data](./data)
  * excel resources: [excel](https://observablehq.com/collection/@observablehq/excel) -- observable collection
  * build on the MapLibre capabilities we've explored in class
  * consider creating a github-pages version with bootstrap styling
  * note that there are several tabs in the excel file
* stinky3 dashboard
  * adapt [this notebook](https://observablehq.com/d/c715e75b5b4c5cfd) to maplibre
  * this can be an independent implementation (working on your own) or work with the group that formed in class
  * integrate the larger dataset: https://github.com/ds5110/stinky2/blob/main/output_data/smc_data.csv
  * tell the story, better -- integrate it into an html page with bootstrap styling

## polleverywhere

* [pollev](http://pollev.com/pbogden)

## Remember the plan

* [plan](plan.md)
* [lh](https://observablehq.com/d/40eebddc9b8eba2d@244)
* [pm](https://observablehq.com/d/271570a96e6dcedf@940)
* [nw](https://observablehq.com/d/ecc6cb841de8b550@632)

## Exercise #1

bootstrap intro

* Create a "docs" directory
* Make a copy of the [bootstrap example](https://www.w3schools.com/bootstrap/) in this (old) tutorial
  ```
  python -m http.server
  ```
* Browse to http://localhost:8000 (same as http://127.0.0.1:8000)
* [docs/index3.html](http://localhost:8000/docs/index3.html)

## Noteworthy

* Noteworthy
  * v3 uses jquery.js
  * v4 & v5 use popper.js
  * bootstrap v5 puts all the js in a bundle...
  * the jumbotron class (in the example) no longer exists in v5 -- but they show you how to make one!
* Bootstrap 5
  * [bootstrap 5 getting started](https://getbootstrap.com/docs/5.2/getting-started/introduction/)
  * This page is worth looking at in detail!
    * [link integrity crossorigin](https://stackoverflow.com/questions/32039568/what-are-the-integrity-and-crossorigin-attributes) -- sfo post
    * [integrity](https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity) -- mdn
    * [crossorigin](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/crossorigin) -- mdn
    * [subresource integrity (SRI)](https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity)
    * [`<main>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/main)
  * You can't simply replace v3 with v5, for example:
    * [my docs5/index3.html](http://localhost:8000/index3.html) -- v3
    * [my docs5/index5.html](http://localhost:8000/index5.html) -- v5 (nothing else changed)
* Bootstrap 5 examples
  * [v5 examples](https://getbootstrap.com/docs/5.2/examples/)
  * [jumbotron in v5](https://getbootstrap.com/docs/5.2/examples/jumbotron/)
  * [typography](https://getbootstrap.com/docs/5.2/content/typography/)

## Exercise #2

Migrate the demo above to bootstrap 5

* Convert the [jumbotron v3 tutorial](https://www.w3schools.com/bootstrap/) to v5
* [step 1](http://localhost:8000/index4.html) -- changing only bootstrap's version number
* [step 2](http://localhost:8000/index5.html) -- adding a v5 bootstrap-examples jumbotron
* [my solution #1](http://localhost:8000/index6.html) -- adapting the w3schools v3 demo
* [my solution #2](http://localhost:8000/index7.html) -- adapting the w3schools v5 demo

## Embedding (review)

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
* [Advanced Embedding and Downloading](https://observablehq.com/@observablehq/advanced-embeds)

## Exercise #2

Embed some earthquakes

* [Brushable earthquakes II](https://observablehq.com/@pbogden/brushable-earthquakes-ii)
* [my solution](http://localhost:8000/docs/index0.html) -- entire embed
* [my solution](http://localhost:8000/docs/index1.html) -- selected embed

## Exercise #3

Put the earthquakes in a dashboard

* [my solution](http://localhost:8000/docs/index2.html) -- localhost
* [my solution](http://cs7290.github.io/fall-2022/index2.html) -- github.io
* tidbits
  * [Dashboard](https://observablehq.com/@mbostock/dashboard)
  * [Authentication simulator](https://observablehq.com/@mbostock/authentication-simulator)
