---
layout: essay
type: essay
title: UI Frameworks
date: 2023-10-5
published: true
labels:
  - CSS
  - Bootstrap
  - UI/UX
  - Frameworks
---

## Why UI Frameworks?

UI frameworks like Bootstrap Tailwind, Svelte, and many more all are meant to streamline the process of adding styling and common UI elements. These kinds of frameworks are not absolutely necessary to make good looking websites, but they save time from implementing common problems that are not trivial. Sure, you could go and customize your own classes in CSS and JS, but it will take time, especially for implementing layouts and common functionality.

Take for example the dropdown class in Bootstrap taken from their documentation:

```html
<div class="dropdown">
  <button class="btn btn-secondary dropdown-toggle" type="button" data-bs-toggle="dropdown" aria-expanded="false">
    Dropdown button
  </button>
  <ul class="dropdown-menu">
    <li><a class="dropdown-item" href="#">Action</a></li>
    <li><a class="dropdown-item" href="#">Another action</a></li>
    <li><a class="dropdown-item" href="#">Something else here</a></li>
  </ul>
</div>
```

Implementing dropdowns in raw JS and CSS are not trivial. These frameworks are not really that hard to learn and allow you to style faster than just using CSS. Server side rendering is another plus. When needing to whip up a quick prototype of what a website would look like, you better believe that a UI framework will be on your side.

### Experience with Bootstrap 5, Positives & Negatives

I will attribute most of my issues to using Bootstrap as being inexperienced, but here are some of my thoughts on using it:

##### Layouts are easier to modify than details

I found when recreating websites for practice that you can't create *everything* with Bootstrap. There are limitations. Based on what I have seen, layouts are easier to describe than minute details in UI frameworks. The sizing of images for example need to be done with CSS if you want a specific image size you need to use CSS as Bootstrap only provides a basic sizing API such as: `w-100` or `min-vh-100` which are pretty common to use. Occasionally, I spend too much time trying to look for functionality in Bootstrap that might not exist.

##### The sacrifice in learning a framework is very small relative to the benefit

One of my worries as a developer is relying too much on a framework or not learning fundamentals. These tools are supposed to make things easier, not harder, and by relying on high level abstractions done for me gives me the worry that if I was stripped from it, then I would become useless.

I think that UI Frameworks are different compared to abstractions in programming languages because from a fundamental level, we use HTML and CSS as a way to visually describe the page. The UI framework just needs to make it easier to describe the page to become a valuable tool in my opinion. HTML and CSS are quite unique compared to more lower level UI implementations like in C/C++ or python because a lot of UI written with programming languages usually more focused on the functionality. Overall, UI frameworks are a great tool to have in your pocket for productivity, but as always, you shouldn't rely on that tool solely on its own to provide you with what you want.