---
title: "StoryMaps"
categories:
  - Blog
tags:
  - Post Formats
  - notice
---

In the love Data Week, I took the lecture of "Introduction to Story Maps (ArcGIS Online) ". This lecture introduces the basic functions of the GIS platform ArcGIS Online. This platform is a user-friendly platform that enables users to create their own multi-layered maps to visualize spatial data. In the lecture, we went through two major parts. The first part introduces us how to create multi-layered maps with different types of spatial data. The second part talks about making a arcGIS story map, which is to show different stories inside a map and embed it into a webpage.

## Different forms of maps

There are two ways to display a map: **Raster and Vector**.
Maps displayed by raster is like pixeled pictures, and the **resolution decrease as the viewer zooms in**. Maps displayed by vector **does not lose resolution when zoomed in**. Below is a slide from the lecture to show the difference between raster and vector.

<img src="/assets/images/mapforms.jpg" style="zoom:25%;" />

## Multi-layered Maps 

In the lecture, the instructor showed us how to visualize statistical results in different map layers from spatial data. We are provided with a data package that contains the graduation and dropout rate in NYC public school ditricts. 

First, we import the compressed files containing different spatial data files into the platform. And the platform will automatically read the data and generate each map based on different files.

For example, the first map below is a layer showing public school districts in NYC. The second layer contains the marks of each unsolved homicide within this range. 

![School District Map]("/assets/images/school_districts.jpg")

![Unsolved Homicides Map]("/assets/images/unsolved_homicides.jpg")

After that, we can ask it to generate maps that express public school density **in shades of color blocks**, which can make the images more concise and intuitive.

![Combined Map Maps]("/assets/images/district_homimcide_color.jpg")

Then we can **put the two layers together into one map**, which will generate the following one. From this map, we can see the relationship between distribution of unsolved homicides and density of public schools.

![Combined Map Maps]("/assets/images/combined.jpg")

Also, we can look into specific data sets using "**filter**" function. This function enables people to better understand **how one layer would affect the performance of different data groups in another layer**. Here I use the example of separating the victim group by sex. In the map, we can see that red dots represent males, blue dots represent females and green represent unknown. And the background color blocks indicats the density of public school districts within that region. And we can get a rough conclusion that unsolved homicides with male victims are more likely to appear in regions with less public schools. 

![Combined Map Maps]("/assets/images/sex.jpg")

## Story Maps 

In the second part of the lecture, we are introduced to a function called story maps. This function enables users to **embed maps created in the first part into webpages**. 

![Combined Map Maps]("/assets/images/embed_maps.jpg")

The story Maps function supports multimedia, which means you can directly import images and videos either from your local files or online sources. **The images can also be embedded into the map** to give a clear view of different "stories" happening in different region on the map. In the example, I used a *New York Times* article as the text source and put relavant images on the map to give the audience a more concrete coherent and visualized reading experience.

![Combined Map Maps]("/assets/images/blk.jpg")

View the full StoryMap [here](https://storymaps.arcgis.com/stories/1278d6ead2e4460e96b59b8e11603c14).


























