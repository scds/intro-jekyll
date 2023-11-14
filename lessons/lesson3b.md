---
layout: default
title: Lesson 3b - Sub-lesson Name
nav_order: 2

# Notice the two lines below. Since this is a sub-lesson of a lesson (Lesson 3a), it's parent is lesson 3 and it's grandparent is Lessons. Make sure to include this if you decide to have sub-lessons. 
parent: Lesson 3 - Lesson Name # Don't forget to change! Should be the title of your parent lesson.
grand_parent: Lessons
---

{: .no_toc}  
# Lesson 3b - Lesson Name 

<details markdown="block" class="toc">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## Located:
- Subdirectory: _layouts

<img width="282" alt="layouts-1" src="https://github.com/SpokenWebAlberta/sandbox/assets/13421476/3d43891f-7ac5-4e3e-800b-ec74f36fa82c">



## What are layouts?
- Page layouts are design templates that control how the page content appears.
- Along with the "default" layout, you can create custom layouts for different types of pages.

## Liquid
- Liquid is a templating language used to combine different components into a single page.
- e.g. The default page includes both 'header' and 'footer'.

**Syntax:** curly brackets + percentage + 'includes' + .html file
- {% includes filename.html  %}

<img width="800" alt="layouts-2" src="https://github.com/SpokenWebAlberta/sandbox/assets/13421476/51de06c7-f987-40f1-911a-fbe9fb361914">

## Markdown
- Layouts are combined with Markdown pages (.md files).
- This is where the page content will appear.

**Syntax:**
- {{content}}

<img width="475" alt="layouts-3" src="https://github.com/SpokenWebAlberta/sandbox/assets/13421476/8d26acc8-e043-4d82-aa25-8368b1154755">
