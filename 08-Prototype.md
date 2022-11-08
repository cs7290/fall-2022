
# 08-Prototype

Review projects from last week

## For next week...

* Continue working on one of the class projects (stinky or bioscience map -- see below).
* Pick one of the three project options below and start working on it.

## stinky -- CS 7290 version

This is a class project -- we'll work on this as a team for the rest of the semester no matter what, and we'll consolidate individual contributions into a single website.

* Deliverable: publicly accessible site at https://cs7290.github.io/stinky
* Stakeholder: CLF or someone (like my neighbor) who smells stinky stuff, would like to report it and know about it
* Goal: Raise awareness and increase participation in Portland area smell issues. This would real-time (or almost real time) app would leverage [Smell My City](https://smellmycity.org/) and previous work of DS5110 students. Previous projects had a lot of trouble getting data from Portland (a 311-based app), so the convenience of Smell My City seems worth our effort. Their API should be fairly simple to harvest in a manner that allows the app to be updated. Their github site will be helpful figuring out real-time access, or we can contact them directly.

## bioscience map of Maine

This is a class project -- we'll work on this as a team for the rest of the semester no matter what, and we'll consolidate individual contributions into a single website.

* Deliverable: publicly accessible site at https://cs7290.github.io/bioscience
* Stakeholder: [Dr. Aileen Huang-Saad](https://roux.northeastern.edu/people/aileen-huang-saad/)
* Goal: Dr. Huang-Saad will join us 14 Nov at 6:15pm to talk about vision, goals and discuss prototypes
* Feedback so far...
  * Hover over each dot and display the name and city and a blurb of what company does
  * We'll agree upon a format for the Excel file so that the data can be updated by a non-technical user
    * We'll get an updated excel file shortly after she visits class next week
    * We can propose/discuss the format for that file next week
  * Add columns to the excel file that allows you tag things and add things...
    * For example, want to be able to add things like company description, research they do, etc.
  * Add a column such as "specialty" then highlight things like "ag biotech", "molecular biology"
  * Identify a career/education path through the elements -- we'll need to figure out how to do this!
    * For example, if you want to work at JAX and you're in HS, what do you need to do?
    * One path might be, e.g., go to one of the CTEs and study X, go to one of the colleges and study Y

## Option #1: choropleth of Maine for DS5010

This is an optional individual project -- you can work independently or in teams of 2

* Deliverable: publicly accessible site at https://cs7290.github.io/broadband
* Stakeholders: DS students in DS5010 (Fall 2022)

## Option #2: data-science use case 

This is an optional individual project -- you can work independently or in teams of 2

* Deliverable: jupyter notebook, related observable notebook (possibly public)
* Implementation should use one of:
  * pure JavaScript (along the lines of the clustering demo we saw in class)
  * [observable-jupyter](https://github.com/thomasballinger/observable-jupyter)
  * [observable-jupyter-widget](https://github.com/thomasballinger/observable-jupyter-widget)
* Example
  * plotly.com builds these kinds of applications with Dash and they have a gallery with all kinds of stuff
  * for example: [image segmentation demo](https://gallery.plotly.host/dash-image-segmentation)
  * we would build our own UI elements with D3, for example...
  * look at `viewof stroke` in [Introduction to views](https://observablehq.com/@observablehq/views)
  * in an observable-jupyter implementation, unlike Dash, our only back end would be the Python kernel 
  * our example would include instructions so that anyone in DS 5110 with no knowledge of JavaScript could use it
  * we would use publicly accessible images, for example:
  * [sklearn.datasets.sample_images](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_sample_images.html)

## Option #3: data-science use case 

This is an optional individual project -- you can work independently or in teams of 2

* BYOD -- bring your own deliverable
* BYOS -- bring your own stakeholder
* BYOS -- bring your own story
* BYOD -- bring your own data

The only real requirement is that you build on things you've learned in the course.
