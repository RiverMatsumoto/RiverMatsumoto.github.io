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


These standards don't just apply to code. When a pattern arises in a project, like the file structure and where you store your images, you should probably keep it the way it is. For example, in Unity, a common organizational pattern is to keep non-code assets in a resources folder for easy access in your project. This is because Unity has a utility class Resources that allows you to load any asset from anywhere if it's in a folder called Resources. These are simply organizational patterns, but I want to talk a bit more about linters.

### Nitpicky linters distract me

After downloading and using the linter my computer science gave me, I went mad using the linter. When I am programming, I don't want warnings to distract me from aspects of the code that are actually functioning. This linter was warning me about spelling, the amount of new line spaces between code, highlight all of my code red, and more. This is just distracting me while I am solving a problem. The solution is to just turn off the linter until you want to refactor your code to clean it up. Even then, I do disagree with a few of the style suggestions.

I want to work on the problem, then refactor when the time is right. When I have orange or red underlines on all of my code before it is even finished, it just doesn't feel good. Even if I can ignore it, when I need to intake that signal, process it, and finally ignore the warning, it adds up over time.

##### 4 spaces vs 2 spaces indenting

This one is a nitpick, but the reason I stick to 4 indent with my code is that when you have too much nesting, it gets obvious that something is probably wrong and you should probably refactor something out into its own function. When you have 2 space indenting, you can basically fit nearly 10 indentations in which it's difficult to analyze the scoping of everything and I personally have a hard time reading it. Also I am quite biased because I started learning programming with C#, python, and C/C++ which all pretty universally use 4 space indenting. I am okay with every other code style difference in Javascript.



