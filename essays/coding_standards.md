---
layout: essay
type: essay
title: Coding Standards and Strict Linters
date: 2023-9-14
published: true
labels:
  - Software Development
  - Code Style
---

It's obvious that we should have standards for our code. It helps people who will possibly look at your code in the future. You are the one who will look at your own code the most often and sometimes it hurts when looking at what you wrote in the past. One of the worst things you can do in a project is have inconsistent standards. This is important for a few very important reasons

1. Less overhead to comprehend your code
2. Your code is honest

There is nothing worse than inconsistency in software. Standards encourage efficiency. If your project says that underscores should be used for member instance variables, it better stay that way. Even if you personally don't like the style, it's better to either stay consistent, or go through the trouble of changing the standard for the entire project.

I experienced this when working on my dungeon crawler project. I was using Jetbrains Rider which encourages certain naming conventions by default. Even though I disliked the PascalCase naming convention for public properties, I made sure to stay consistent throughout the entire project as to not anger my future self.


These standards don't just apply to code. When a pattern arises in a project, like the file structure and where you store your images, you should probably keep it the way it is. For example, in Unity, a common organizational pattern is to keep non-code assets in a resources folder for easy access in your project. This is because Unity has a utility class Resources that allows you to load any asset from anywhere if it's in a folder called Resources.
