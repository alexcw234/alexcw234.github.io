---
layout: project
type: project
image: images/toasteroven.png
title: Manoa Student Kitchen
permalink: projects/manoastudentkitchen
date: 2017
labels:
  - Meteor
  - Semantic UI
  - Javascript
summary: Manoa Student Kitchen is an application that provides students at UH Manoa to share and browse easy-to-make recipes.
---
## Why Manoa Student Kitchen?
College students are often extremely busy, and as such, lack the time to cook elaborate meals. There are also those for whom cooking their own meals is too expensive or difficult.  This is the problem that Manoa Student Kitchen aims to help solve. 

Manoa Student Kitchen is an application that allows students at UH Manoa to share their simple recipes with others that are both affordable and easy to make (requiring no more than a toaster oven). Students who may know a few simple recipes, even if they lack the time to make them themselves, would be able to share them with others who may be looking for something simple and easy to cook up. As keeping costs down is an important part of college life, the app aims to inform students of the cost of each ingredient, as well as of the ideal location to obtain it.

## The Features
As mentioned above students will be able to submit their own recipes to the application. The recipes will then show up when searched for by tag or by recipe name.

![Photo of the homepage](https://github.com/alexcw234/alexcw234.github.io/blob/master/images/home.png?raw=true)

Inspired by Steam tags, the application has a feature allowing users to tag a recipe with a label like "dessert", or "cheap", which helps in the searching process. The most common tags are deemed "popular tags" and appear in a random selection at the bottom of the homepage. In addition, recipes with the most tags appear as "popular recipes" on the homepage.

In addition, users will be able to maintain a profile of their recipes as well as edit their own recipes. Finally, certain users have administrator access, through which they are able to view any recipe, tag, or user on the site as well as delete them upon detected abuse.

For more information about the application and its features, [click here to go to the github.io website](https://manoastudentkitchen.github.io/).

## My Contribution
I worked in a group with 2 other students on this project. Although towards the beginning of the development process my contributions were less apparent, focusing mostly on the homepage and related functions, once the format of the Recipe, Ingredient, and Location collections were decided on and implemented, I took the lead in implementing the application's functionality. Because I have prior experience with web development, particularly in that I know what to look for and how to test when things go wrong, this turned out to be the ideal role for me in the group. My main contribution here was to the Create Recipe page, where I put together a dynamic form that including both dropdown menus loaded from the database, as well as a system to reactively set and store a preview of an image that has been uploaded. A large portion of the helper functions throughout the application ended up being based on the functions on this page and the home page. 

![Add Recipe Page](https://github.com/alexcw234/alexcw234.github.io/blob/master/images/addrecipe.png?raw=true)

It was helpful to be working in a group on a number of levels. For one thing, had I been working alone, the application would probably have ended up with an interface that was quite ugly and spartan (though fully functional). Fortunately, my group members were much more attuned to ui design principles than I am, and so I was able to focus more on the functional aspects of the application.






