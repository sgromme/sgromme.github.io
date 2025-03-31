---
title: Setting Up Chirpy
author: scott_gromme
date: 2025-03-27 09:10:00 +0800
categories: [Blogging, Chirpy]
tags: [writing, Jekyll, Chirpy]
render_with_liquid: false
---



This is a brief introduction to setting up a Github page.  Trying to get the setup time to 1 hour.  More to follow.




Prerequisites:
Note: This is for Windows , WSL and Docker only. (As a alternative you can you Github code spaces)

1. Git account. 
2. WSL-2 
3. Docker Desktop. 
4. .Install Ubuntu (use the latest version) in WSL. (with git configured see Appendix A)

Check that Docker runs in your Ubuntu install.
```
docker run hello-world
```


Steps to follow on wiki:
Do the "Getting Started", "Customize the Favicon" and "Writing a New Post".

[Home · cotes2020/jekyll-theme-chirpy Wiki · GitHub](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)


### Directory tree structure of pages added and modified.
```
├── _data
│   ├── authors.yml
├── _config.yml
├── _tabs
│   ├── about.md
├── _drafts
│   ├── 2019-08-08-text-and-typography.md
│   ├── 2019-08-08-write-a-new-post.md
│   ├── 2019-08-09-getting-started.md
│   └── 2019-08-11-customize-the-favicon.md
├── _site
│   ├── assets
│   │   ├── img
│   │   │   ├── favicons
│   │   │   │   ├── android-chrome-192x192.png
│   │   │   │   ├── android-chrome-512x512.png
│   │   │   │   ├── apple-touch-icon.png
│   │   │   │   ├── browserconfig.xml
│   │   │   │   ├── favicon-16x16.png
│   │   │   │   ├── favicon-32x32.png
│   │   │   │   ├── favicon.ico
│   │   │   │   ├── mstile-150x150.png
├── _posts
│   ├── 2023-08-28-my-first-post.md
│   └── 2025-03-27-setting-up-chirpy.md

```

### Page to modify

![Desktop View](assets/img/posts/Pasted-image-20250327084506.png){: width="972" height="589" }
_The _config.yml file edits in green_

### Page to modify

![Desktop View](assets/img/posts/Pasted-image-20250327084629.png){: width="972" height="589" }
_The _tabs/about.md file edits in green_


### Pages to modify and add

![Desktop View](assets/img/posts/Pasted-image-20250331073240.png){: width="972" height="589" }
_The files to be modified or added_



Appendix A:
Add git variables with the following commands.


```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Appendix C:
Command to print the directory structure.
```
tree
```


Appendix B:
Command to start the web server: 
```
bundle exec jekyll serve --livereload

```
