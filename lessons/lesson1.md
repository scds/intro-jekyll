---
layout: default
title: Lesson 1 - Getting Started
nav_order: 1
parent: Lessons
---
<!-- 
This page is an example lesson template.
Add, edit, or remove any content below for the workshop in question. -->

<!-- Putting a {: .no_toc} above a header removes it from the table of contents -->

{: .no_toc}  
# Lesson 1 - Getting Started

A small description about the lesson.

<!-- This is your table of contents. You don't need to touch it, it automatically creates it when you add or remove headers. If you do not want a header to be included, put {: .no_toc } above the header line, as you can see above with Lesson 1 - Lesson Name. Make sure that there's also an empty line above {: .no_toc }... Markdown is picky about this :( -->
<details markdown="block" class="toc">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

<!-- Here are your learning objectives. Just like in the introduction, but more specific for this lesson. -->
## Create a New Repository in GitHub
1. Sign into GitHub
2. At the top-right, click the "+" Sign.
3. Select "New Repository."
4. Under Owner, select your username.
5. Under Repository name, type "my-website".
- You will be redirected to a Quicksetup page. For now, you don't need to touch the settings. We'll return to this page in a moment...

See: [GitHub's Guide to Creating a Repo](https://docs.github.com/en/get-started/quickstart/create-a-repo) for more detailed info.

## Install Jekyll and Create Jekyll Site

*Note: To install and run Jekyll, you will need to use your computer's *Command Line* interface.

1. Open Terminal (On a mac, type Cmd + spacebar) and search "Terminal."
2. In terminall, install the necessary software: Homebrew, chruby, and Ruby (See [Jekyll Installation](https://jekyllrb.com/docs/installation/) for instructions.
3. Install Jekyll
```
gem install jekyll
```
4. Install Jekyll bundler
```
gem install jekyll bundler
```
5. Create your new Jekyll site
*Note: you can choose any name! Here, I've chosen "my-website."
```
jekyll new my-website
```
6. Change into your new directory
```
cd my-website
```
7. Build the website
```
bundle exec jekyll serve
```

See: [Jekyll's Quickstart Guide](https://jekyllrb.com/docs/) for more detailed instructions.

## Modify Gemfile

1. In the main folder, open the file "Gemfile."
2. Uncomment the line below, and replace GITHUB-PAGES-VERSION with the latest supported version of the github-pages gem. You can find this version here: "[Dependency versions](https://pages.github.com/versions/)."
  - e.g. At the time of creating this module, the dependency for GitHub Pages is "228." 

```
 gem "github-pages", "~> 228", group: :jekyll_plugins
```

3. Add the following gem

```
gem "webrick"
```


## Modify YML file

The YML file configures the main settings for your website.
*Note: Make sure you have the correct URL. Capitalization and backslash placement matters!

1. In the main folder, open the file "_config.yml".
2. Fill in the following fields:
- URL (main url) e.g. “https://cmiya.github.io”
- BaseURL (subpath) e.g. “/my-website”
- title
- email
- description
- Github_username

<!-- Summarize your learning objectives here. It acts as a reminder to the learner about what they just learned, as well as a checklist for you to make sure you covered everything you wished to cover. -->

## Test file (locally)
1. In Terminal, type:
  
```
bundle exec jekyll serve
```
   
1. In your browser (Chrome), visit the URL:
  
```
http://localhost:4000/
```

If successful, you should see a preview of your page.

## Key Points / Summary

- Local (i.e. your computer) vs. Remote (e.g. GitHub)
- Gemfile
- YML file

<!-- You can add your additional resources for a specific lesson here, however there is also an additional resources page alongside the conclusion at the end of the workshop website.
## Additional Resources (optional)


- Here, you can list some additional resources the student can access to learn more about this lesson.

 -->
