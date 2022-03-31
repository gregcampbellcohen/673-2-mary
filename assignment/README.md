# Assignment 02: Adding user interaction to our maps

## Table of contents

<!-- TOC -->

- [Assignment 02: Adding user interaction to our maps](#assignment-02-adding-user-interaction-to-our-maps)
    - [Table of contents](#table-of-contents)
    - [Part I: Complete an interactive map from the lesson (4 pts)](#part-i-complete-an-interactive-map-from-the-lesson-4-pts)
    - [Part II: Interactive map of labor/household statistics (6 pts)](#part-ii-interactive-map-of-laborhousehold-statistics-6-pts)
        - [Reflection from reading](#reflection-from-reading)
        - [Deliverable](#deliverable)
        - [Tip](#tip)
    - [Challenge: Use an original data source (**+2 pts**)](#challenge-use-an-original-data-source-2-pts)

<!-- /TOC -->

## Part I: Complete an interactive map from the lesson (4 pts)

Run through the lesson and create the interactive map of Kentucky housing ownership patterns. While you can cut-and-paste code to (mostly) complete this part of the assignment, you should strive to understand how functions work, when they are called, and why we are passing data as arguments between functions.

**Task:** Rewrite the legend code so that the `addLegend()` function only adds the HTML legend to the map and a new function named `updateLegend()` updates the title and class range values when the user selects a new data attribute. 


## Part II: Interactive map of labor/household statistics (6 pts)

Look through the datasets provided within the [data](data/) directory. The data describe statistics about labor and households, drawn from [American Fact Finder](https://factfinder.census.gov) and joined with county geometries from the [US Cartographic Boundary Shapefiles](https://www.census.gov/geo/maps-data/data/cbf/cbf_counties.html). See the [meta.md](data/meta.md) file for a description of the attribute field names.


### Reflection from reading

From our [short reading](https://shapeofdesignbook.com/chapters/02-craft-and-beauty/) reflect upon the advice the professor gave Chimero: that his portfolio, "Needs more love." Then read the task and requirements below. After you select a dataset to map, consider the following questions:

1. In what ways do you believe in the map you're about to create? What gives you the inspiration to labor over your map?
2. How do you care about an intended audience for this map? Imagine if this project was for a client, e.g., a non-profit doing advocacy around labor and social issues. Now, you have two audiences.

Use your answers to these questions to guide you through the process detailed here:

### Deliverable

Create an interactive map meeting the following requirements:

- [ ] the map uses a choropleth thematic type to represent quantitative data
- [ ] the map provides the user with a UI widget (either a dropdown menu or radio buttons) for updating the map and legend with a new data attribute
- [ ] the map has a clear and descriptive title/subtitle that should establish 1.) **what** is being mapped, 2.) **where** the phenomena is geographically, and 3.) **when** the mapped phenomena occurred
- [ ] the map has a legend, including:
    - [ ] a descriptive legend title (i.e., not "legend")
    - [ ] an indication of what numeric class ranges each color represents
- [ ] the page includes supplementary information about the map, including a description, links to data sources, the map author (and links to the author's GitHub profile or portfolio)
- [ ] the map and page are uniquely styled with novel typography and colors, i.e., if you use the lesson template, it should be altered
- [ ] the page loads smoothly and the code contains no errors
- [ ] the code is well-written with appropriate comments
- [ ] the repository includes timely commits of progress with descriptive commit messages

Save the _index.html_ file for the map within the _assignment/_ directory and commit your work as you go. When you are finish, submit a link to the repository in Canvas.

### Tip

You can reuse the document you created from the lesson, which will have most of the components you will need to finish this part of the assignment. You will, of course, need to change variable names and decide whether (and how) an attribute needs to be normalized. Feel free to restructure the HTML as you see fit and customize the CSS. Or, use an entirely different Bootstrap template, CSS boilerplate, or framework. Whichever path you take, reflect on *why* you make the design choices you do.

## Challenge: Use an original data source (**+2 pts**)

Aim high, extend **Part II**, and build a new map using an original data source (and geography other than KY counties). Since you only have a week, the trick here is to get the dataset and format it correctly as soon as possible.

You'll likely want to use the _ky_counties_housing.json_ file (or the optional data files in the _lab-02/data_ directory) as a model for building your data file. It should be a GeoJSON file that includes the geometries of your mapped area and the quantitative data value as attributes within the properties of the file.

Choose data with attributes that are qualitatively different (such as owned with a mortgage vs. owned free and clear). Avoid data that are temporal time stamps (we'll be exploring this kind of data in the next Module and using a UI slider to sequence through those values to update the map). Consider novel additions like modifying the script so that one set of class breaks is applied across all three datasets and updating the tooltip to include the raw number count.

The map must meet the requirements set for the map in **Part II** and have at least four attributes that can be selected for mapping. Save the _index.html_ file for the map within the _assignment/_ directory and commit your work as you go. 