---
layout: post
title:  "Multiple \"GitHub Pages\" sites with a single domain"
date:   2016-08-17 12:23:03 +0200
categories:
  - Ninja's tips
  - GitHub
---
Today I set to a task of publishing the first barebones version of this diary – and since I'd already had one purely static website deployed to my [GitHub Pages](https://pages.github.com/) space, I pondered on how to push a new Jekyll powered site alongside it. *"Alongside it" as in "under a different path on the same domain" (such as, in my case, [http://uruba.ninja](http://uruba.ninja) -> [http://uruba.ninja/blog](http://uruba.ninja/blog)).*

If you're facing the same decision, be advised that there are basically two options as to how to achieve this:

- **Publish the website in a folder in the main repository**
- **Create a new repository with a `gh-pages` branch**

While the former *"folder"* option offers a way to have everything neatly in one place, it may result in a slightly cluttered directory structure (not to mention that it may introduce strenuous difficulties, should you want to utilize the GitHub's integrated Jekyll site generator and still want to keep the sites independent of each other). So, you can just create a folder `site2` in your repo, push the content in, and your `username.github.io/site2` site is good to go.

The latter *"repository"* option is a concise way to keep everything clean and separated, as the name of the repository becomes automatically your path relative to your main GitHub site. So, if you create a new repository named `site2` and push your new site's content onto its `gh-pages` branch, you will get your new site at `username.github.io/site2` also.  
Though you have to keep in mind that the name you choose for this repository will be unavailable for any your other projects.

**_So, in the end it really boils down to your personal preference – you end up with the same result either way._**
