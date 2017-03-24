---
layout: essay
type: essay
title: Re-approaching Meteor
date: 2017-03-23
labels:
  - Meteor

---

## I think this has become a pattern...
I spent the past few weeks learning the basics of the Meteor web framework. Similar to how I had an initial attempt at learning Javascript several months before learning Javascript for real, this was not my first attempt at learning Meteor. And, like my initial impression of Javascript, my first impression of Meteor was not the best.

Due to a misunderstanding in which I was advised to use a local-storage database when I actually needed something server-side (after which I spent the next week or so getting frustrated over the concept of data "magically" floating across multiple devices' local storage), I developed misgivings towards unfamiliar databases. So when the tutorial I looked at for Meteor told me to insert some sample data by typing into the browser command line, it raised red flags for me, being too much like what I had been vexing over before. Further, it just seemed "too" easy. Apparently, I could type in data and it would just be stored in the database. No setup! (at least, in that tutorial) But, coming from learning about SQL and relational databases, the lack of setup (at least, in that tutorial) was precicely why I didn't feel comfortable. It all just seemed too, and I don't really have a word for this but, "floaty".

## A New Attempt
Approaching Meteor again, I went in with more knowledge of how web applications worked, and was able to become more comfortable with the framework. For one, it helped me to initially ignore the first tutorial and explore the contents of the various files in the sample application template. I managed to find the stuff.js file that had the schema for the database, which cleared up the misgivings I had previously had for Meteor, seeing how it could be tied to the input fields.

Overall I like the simplicity of Meteor in that it is easy to accomplish both front-end and back-end tasks without having to switch between setups or make http requests. I do expect there to be some ways in which simplicity could be detrimental however, but I have not run into anything like that yet with the simple assignments that I have learned from. I look forward to working on a larger project using Meteor, especially after descovering the "searchable tags" input field offered by Semantic UI, and imagining how I could use that in an application.

![alt tag](https://github.com/alexcw234/final-project-mockup/blob/master/doc/EditProfile2.png?raw=true)
(Specifically in searching for the instruments, and genres for musicians...although the listing would need to be thorough as to not leave anything out)

A challenge that I have faced so far is that sometimes there will be an error in the application, but no indication of where the error comes from. A lot of the times this is due to forgetting to import something, but other times it is caused by mislabeling a link. Most of the time, however, the console does print something to do with the error that has occurred, which is helpful coming from AngularJS where the console output is rarely useful.



