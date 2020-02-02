---
layout: project
type: project
image: images/surfGamePic.PNG
title: Surfer
permalink: projects/surfer
# All dates must be YYYY-MM-DD format!
date: 2019-3-12
labels:
  - Java
  - EZ
summary: A 2-d game I made for ICS111
---

<img class="ui image" src="{{ site.baseurl }}/images/surfGamePic.PNG">

I made this surfing game in ICS 111 as a way to show my understanding of simple object orientation in Java. We had recently been taught about object orientated programming in Java and needed to demonstrate our understanding by making a game that utilized multiple classes, arrays, and loops. We were tasked with properly implementing these cohesively in a game where you control a character that must collet resources, while avoiding obstacles.

Creating the class for the character was easy enough, for I have made simple games before where you move a character two dimensionally using the keyboard. Defining classes for the resources and obstacles were also easy, for their functions were few and simple. What was challenging at the time was implementing the classes and working with each class instance's variables. The idea of objest orientation is somewhat layered making confusing, which is what I sturggled with. For example, the obstacles were storms and traveled from the right of the screen to the left, so they must be reset when reaching the left side. Here's the code for that.

```
for(int i = 0; i < numberOfStorms; i++) {
  if (Stormholder[i].picture.getXCenter()<= 0) {
    Stormholder[i].teleport();
    }
  }
```

A simple loop and function call, but what took me a while to wrap my head around was the depth of the if statements parameters. When trying to make sense of what is really being done, it's hard to do so at a glance, but by going through and tracing the instances and functions, it becomes easy to understand.

This program didn't only help solidify my understanding of simple object orientation in Java, but it more importantly taught me about the value and how to properly trace code. Though it is one of the first things taught, it is often overlooked for being simple, yet it is one of the most valuable tools in programming, as I learned with this experience.
