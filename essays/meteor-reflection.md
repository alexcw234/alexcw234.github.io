---
layout: essay
type: essay
title: Re-approaching Meteor
date: 2017-03-23
labels:
  - Meteor

---

## I think this has become a pattern...
I spent the past month going from learning the basics of the Meteor web framework to building an application, called [manoastudentkitchen](https://manoastudentkitchen.github.io/) that is built from it. With all things however, comes a first impression. Similar to how I had an initial attempt at learning Javascript several months before learning Javascript for real, this was not my first attempt at learning Meteor. And, like my initial impression of Javascript, my first impression of Meteor was not the best.

Due to a misunderstanding in which I was advised to use a local-storage database when I actually needed something server-side (after which I spent the next week or so getting frustrated over the concept of data "magically" floating across multiple devices' local storage), I developed misgivings towards unfamiliar databases. So when the tutorial I looked at for Meteor told me to insert some sample data by typing into the browser command line, it raised red flags for me, being too much like what I had been vexing over before. Further, it just seemed "too" easy. Apparently, I could type in data and it would just be stored in the database. No setup! (at least, in that tutorial) But, coming from learning about SQL and relational databases, the lack of setup (at least, in that tutorial) was precicely why I didn't feel comfortable. It all just seemed too, and I don't really have a word for this but, "floaty".

## A New Attempt
Approaching Meteor again, I went in with more knowledge of how web applications worked, and was able to become more comfortable with the framework. For one, it helped me to initially ignore the first tutorial and explore the contents of the various files in the sample application template. I discovered how Meteor stores data in collections, and how those collections were structured, which cleared up the misgivings I had previously had for Meteor.

Overall I like the simplicity of Meteor in that it is easy to accomplish both front-end and back-end tasks without having to switch between setups or make http requests. In that way, it has an advantage over the other framework I know, AngularJS (having its own backend helps too!). I also liked the template system and routing, which I found intuitive enough. The best part about Meteor to me, however, is, thanks to Mini Mongo, how the data updates immediately on the webpage when it changes in the database.

<img src="https://github.com/alexcw234/alexcw234.github.io/blob/master/images/home.png?raw=true" width=50%>

On the other hand, after using Meteor to build a larger web application, there were some aspects that I struggled with. For example, I found myself writing a lot of redundant code in the template helpers and events, which seemed themselves to be tied to the individual page. I suspect, however, that there is a way to simplify Meteor code that I haven't been able to learn yet, but once I do would prove extremely helpful, like when I learned how to use providers in AngularJS. These things, of course, are learned with experience, and by studying the examples from others. One thing I did like about meteor was the amount of helpful documentation that was found online. In particular, the collection-finding functions were described in enough detail that I never found myself having trouble querying the database.

Overall, my "second" first steps into Meteor have given me invaluable practice in learning a new web framework. While I am not sure if I will use meteor in future projects, I will certainly be able to use the principles of Software Engineering that I learned from building a Meteor application going forward.
