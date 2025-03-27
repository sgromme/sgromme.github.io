---
title: Setting Up Chirpy
author: W. Scott Gromme
date: 2025-03-27 09:10:00 +0800
categories: [Blogging, Chirpy]
tags: [writing, Jekyll, Chirpy]
render_with_liquid: false
---



This is a brief introduction to setting up a Github page.  Trying to get the setup time to 1 hour.  More to follow.




Prerequisites:
Note: This is for Windows , WSL and Docker only.
Git account. 
WSL-2
Docker Desktop. 
Install Ubuntu (use the latest version) in WSL. (with git configured see Appendix A)
Check Docker run in your Ubuntu install  "docker run hello-world"


Steps follow on wiki:
Do the "Getting Started", "Customize the Favicon" and "Writing a New Post".
[Home · cotes2020/jekyll-theme-chirpy Wiki · GitHub](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)



Here  are the files you will want to add or modify(M is modified and U is new file)


![[Pasted image 20250326170004.png]]


What to modify in _config.yml and _tabs/about.md_ files 
```
├── _config.yml
├── _tabs
│   ├── about.md
```

### Page to modify

![Desktop View](assets/img/posts/Pasted-image-20250327084506.png){: width="972" height="589" }
_The _config.yml file edits in green_

### Page to modify

![Desktop View](assets/img/posts/Pasted-image-20250327084629.png){: width="972" height="589" }
_The _tabs/about.md file edits in green_

Run the tree command to get a overview of the 


vscode ➜ /workspaces/sgromme.github.io (main) $ tree

```
├── assets
│   └── lib
├──_config.yml
├── _data
│   ├── contact.yml
│   └── share.yml
├── Gemfile
├── Gemfile.lock
├── index.html
├── LICENSE
├── _plugins
│   └── posts-lastmod-hook.rb
├── _posts
│   └── 2023-08-28-my-first-post.md
├── README.md
├── _site
│   ├── 404.html
│   ├── about
│   │   └── index.html
│   ├── app.min.js
│   ├── archives
│   │   └── index.html
│   ├── assets
│   │   ├── css
│   │   │   ├── jekyll-theme-chirpy.css
│   │   │   └── jekyll-theme-chirpy.css.map
│   │   ├── img
│   │   │   └── favicons
│   │   │       ├── android-chrome-192x192.png
│   │   │       ├── android-chrome-512x512.png
│   │   │       ├── apple-touch-icon.png
│   │   │       ├── browserconfig.xml
│   │   │       ├── favicon-16x16.png
│   │   │       ├── favicon-32x32.png
│   │   │       ├── favicon.ico
│   │   │       ├── mstile-150x150.png
│   │   │       └── site.webmanifest
│   │   ├── index.html
│   │   └── js
│   │       ├── data
│   │       │   ├── mathjax.js
│   │       │   ├── search.json
│   │       │   └── swconf.js
│   │       └── dist
│   │           ├── categories.min.js
│   │           ├── commons.min.js
│   │           ├── home.min.js
│   │           ├── misc.min.js
│   │           ├── page.min.js
│   │           ├── post.min.js
│   │           └── theme.min.js
│   ├── categories
│   │   ├── blogging
│   │   │   └── index.html
│   │   └── index.html
│   ├── feed.xml
│   ├── index.html
│   ├── norobots
│   │   └── index.html
│   ├── posts
│   │   ├── index.html
│   │   └── my-first-post
│   │       └── index.html
│   ├── redirects.json
│   ├── robots.txt
│   ├── sitemap.xml
│   ├── sw.min.js
│   └── tags
│       ├── index.html
│       ├── supply-planning
│       │   └── index.html
│       └── writing
│           └── index.html
├── _tabs
│   ├── about.md
│   ├── archives.md
│   ├── categories.md
│   └── tags.md
└── tools
    ├── run.sh
    └── test.sh
```


Appendix A:
Add git variables with the following commands.


```
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```
