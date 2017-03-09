---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-03-09
labels:
  - Software Engineering
  - Meteor
---

# Solved Problem
A problem that I have had when trying to make a meteor application is that sometimes when I make a change or add a file the change does not appear on the application. Additionally, sometimes the change does appear but something else disappears. 

For example, at one point I added a new template with a helper function. When I checked the running application, my page styling had vanished! I then spent the next 15 minutes or so on a previous branch trying to find where the stylesheet import was in the app in case I had accidentally deleted it at some point. I hadn't!

After finding the import intact, I instead decided to finish writing the helper function instead. Upon doing so, the styling returned to the page. From this I learned rather than getting sidetracked and panicing to focus and try to finish what I am doing.

# Unsolved Problem

A problem that I haven't solved yet has been to get the various components of a import form working. While the form buttons seem to work correctly, the data does not appear in the database when I check. However, I am in no way discouraged by this and I think that if I spend more time on it or do some searching on how to solve the problem, I will figure it out. The same goes for most problems that I have had with web development in the past. 