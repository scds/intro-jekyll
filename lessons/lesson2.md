---
layout: default
title: Lesson 2 - Commit your Work
nav_order: 2
parent: Lessons
---

{: .no_toc}  
# Lesson 2 - Upload Website Repository to GitHub

Files can be stored **locally** (on the computer you are working on) or **remotely** (hosted elsewhere, like on GitHub).

*Sending* file changes to the remote version of your project (i.e. on GitHub) is called a "**push**." If you make changes to your remote version and want to update the local version on your computer, you can *recieve* file changes using a  "**pull**."

Let's see how that works... 

<details markdown="block" class="toc">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

## Commit your work

1. In Terminal, stage the changes you made (i.e. prepare to send) by typing:
```
git add .
```
2. *Commit* your changes and add a description (optional)
```
git commit -m 'Initial GitHub pages site with Jekyll'
```

## Add your GitHub repo as your remote repository

```
git remote add origin https://github.com/USER/REPOSITORY.git
```

## "Push" files to your remote repo

```
git push -u origin main
```

## Key Points / Summary

- Local vs. Remote
- Push vs. Pull
