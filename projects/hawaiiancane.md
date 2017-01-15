---
layout: project
type: project
image: images/hawaiiancane.png
title: Kō: An Ethnobotanical Guide to Hawaiian Sugarcane Varieties, Webspace
permalink: projects/hawaiiancane
date: 2016
labels:
  - DNN
  - Javascript
  - jquery
  - Python
  - Selenium
summary: Webspace for Dr. Lincoln's book on Hawaiian Sugarcane varieties.
---

I was hired to build a webspace for Dr. Lincoln's book on Hawaiian Sugarcane varieties. It contains general information about Hawaiian cane as well as an index of over 50 different varieties of sugarcane with images categorized by cane part (stalks, buds, leaves, etc.) It also has a botanical key module with which someone may identify a cane based on answering questions about its characteristics. 

Since Dr. Lincoln wanted a site that he could make basic changes to without any knowledge about programming or web development. To assist in this I used UH Manoa College of Tropical Agriculture and Human Resources (CTAHR)'s DNN content management system as a base for the site. After creating the basic scaffold of built-in modules and static information, I used jquery to implement additional functionality as required. 

One such instance was on the "Cane Varieties" page, where I was requried to display a large number of images and descriptions side by side in a table. I had 2 main types of modules available to do this: 
- Gallery modules: these allow images to be added and modified "easily" (as required) but have poor options for information display
- Tab modules: these are ideal for organizing and displaying the information and images as Dr. Lincoln requested, however required html knowledge to do so.

In order to deal with this dichotomy, I utilized a jquery script to build the table dynamically in the Tab module by fetching the image links from the Gallery module, which was hidden upon page load. This would allow Dr. Lincoln to add images using the gallery module and have them show up on the tab module's table.

The gallery modules required images to be added manually one by one. As there were over 50 sugarcanes, some having up to 50 images, I wrote another script in Python using the web browser automation system Selenium. While I still needed to categorize the images manually, however the actual upload process became much less tedious.

In addition to learning jquery and Selenium, what was most valuable about this project for me was learning how to work around a less-than-ideal developer environment by using the resources that I do have access to in order to leverage user-friendlyness with custumization.





