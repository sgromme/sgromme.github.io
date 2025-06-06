---
title: Setting Up Chirpy
author: scott_gromme
date: 2025-03-27 09:10:00 +0800
categories: [Blogging, Chirpy]
tags: [writing, Jekyll, Chirpy]
render_with_liquid: false
---



This is a brief introduction to setting up a Github page.  Trying to get the setup time to 1 hour.  More to follow.




## Prerequisites
Note: This is for Windows , WSL and Docker but should work for any operating system. (As a alternative you can you Github code spaces see this link)

[Github Codespaces](https://sgromme.github.io/posts/setting-up-chirpy-codespaces)


1. Git account. 
2. WSL-2 
3. Docker Desktop. 
4. Install Ubuntu (use the latest version) in WSL. (with git configured see Appendix A)

Check that Docker runs in your Ubuntu install.

```console
docker run hello-world
```


Steps to follow on wiki:
Do the "Getting Started", "Customize the Favicon" and "Writing a New Post".
### Note: Under the "Getting Started" link , do only "Option 1:". You will be using Dev Containers in Visual Studio Code, make sure to install the DevContainer Extension in Visual Studio Code.

[Home · cotes2020/jekyll-theme-chirpy Wiki · GitHub](https://github.com/cotes2020/jekyll-theme-chirpy/wiki)


## Directory tree structure of pages added and modified.
![Desktop View](assets/img/posts/Screenshot-2025-03-31-082148.png){: width="972" height="589" }
_The _drafts directory and example posts is optional_

## Pages to modify and Add

![Desktop View](assets/img/posts/Pasted-image-20250327084506.png){: width="972" height="589" }
_The _config.yml file edits in green_

### Page to modify

![Desktop View](assets/img/posts/Pasted-image-20250327084629.png){: width="972" height="589" }
_The _tabs/about.md file edits in green_


### Pages to modify and add

![Desktop View](assets/img/posts/Pasted-image-20250331073240.png){: width="972" height="589" }
_The files to be modified or added_

## Lessons Learned while using jekyll-theme-chirpy

1. Test all page (especially _config.yml ) updates on your local web server before pushing to Github. Also make sure to test on Edge and Chrome.
2. Your Github page should always be open and on the "Actions" tab on your remote repository to see if any errors have occurred after pushing changes to Github. You should also be on the Github web page to test updates and to verifiy everthing displays correctly. If a error occurs, just expand the error and see if you can troubleshoot it.
3. Posts pages need to be exact - for example - only one empty line should be after a #(or multiple # header line), if a extra space is added and the post\text might not display correctly or at all (occurs in Chrome browser).
4. Use the _drafts directory to keep example posts and posts that are not complete.  You can then drop them in the _posts directory and test them on the local server before pushing then to Github.
5. Install and use Copilot to help with using chirpy.
6. Store your images under ./assets/img/posts.


## Appendix

### Appendix A: Git Configuration

Add git variables with the following commands (usually only on Wsl-2).  If you are unsure run these commands to see if they already exist.

```console
git -v
git config --global user.name
git config --global user.email
```

```console
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Appendix B: Directory Structure

Command to print the directory structure.

```console
tree
```

### Appendix C: Starting the Jekyll Server in reload

Command to start the web server: 

```console
bundle exec jekyll serve --livereload
```
