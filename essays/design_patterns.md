---
layout: essay
type: essay
title: Design Patterns
date: 2023-11-30
published: true
labels:
  - Web
  - Design Patterns
---

Design patterns are software patterns that solve a commonly encountered problem. I won't go into extreme detail about many design patterns and instead I want to discuss when to look to design patterns and why it's good to understand the most common ones.

### Introducing Design Patterns
There are three main design patterns: behavioral, structural, and creational. For example, the strategy pattern is a behavioral pattern that allows for easily swapping out predefined algorithms or behavior interchangeably. For example, when you press Ctrl+S in a fully featured text editor, you might want to select all the text instead of saving. In the text editor's settings, you might swap out Ctrl+S from the action of saving the file for selecting all the text in the file. 

Many design patterns introduce complexity to your software and it's always best to make sure that you carefully choose a good fit for your software design problems.

### When to Use Design Patterns
Because I encountered the use of design patterns most in my game development experience, I will use it as an example. The first time I was introduced to design patterns, I tried to use them everywhere that I thought it was possible and learned that most of the time it overcomplicated the codebase significantly. It was a good learning experience and I would recommend for everyone to apply new concepts as much as possible even if you think it might fail. However, I found that what worked best for me was to draft out a working prototype of something that works, and pay attention to patterns or problems that I run into along the way. Most of the time, the problem will make itself clear as you move forward and that might be a signal that you need a more robust solution.

### My Experience with Design Patterns

While working on a dungeon crawler project of mine, I found that creating an RPG turn based battle with a good amount of complexity needs a robust system for drafting out and adding new abilities and moves. I found through some research that using the composite pattern worked best. Most RPG games have abilities that are composed of effects such as a damage effect, healing effect, or status effect. I used this pattern to easily create and design new abilities for characters to use without having to manually write a separate class for each one which would have been hell.

### Avoid Prematurely Using a Design Pattern
The biggest waste of time I have experienced was trying to implement a design pattern into my dungeon crawler game and realizing I either don't need it, or it doesn't actually solve the problem I needed it to solve. All that pain could have been avoided by using the basics to solve the problem so that I can see extremely clearly exactly what I would need to solve the problem.