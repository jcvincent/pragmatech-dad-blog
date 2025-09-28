---
title: My First Blog Post
date: 2025-09-28
draft: false
tags:
  - pragmatechdad
  - posts
---

Inspired by networkchuck.

{{< youtube dnE7c0ELEH8 >}}

I did my blog site by running in Windows 11 using Obsidian, Hugo, Github and Hostinger.

Install Go Lang

[Install Hugo on Windows](https://gohugo.io/installation/windows/)
See documentation at https://gohugo.io/.

Use Winget
[Winget](https://learn.microsoft.com/en-us/windows/package-manager/) is Microsoft’s official free and open-source package manager for Windows. To install the extended edition of Hugo:

```
winget install Hugo.Hugo.Extended
```

To uninstall the extended edition of Hugo:

```
winget uninstall --name "Hugo (Extended)"
```


Create a new site

```
## Verify Hugo works
hugo version

## Create a new site 

hugo new site websitename
cd websitename
```


Download a Hugo Theme

Select your theme here https://themes.gohugo.io/.

Initialize your local git repo

```
## Initialize a git repository (Make sure you are in your Hugo website directory)

git init

## Set global username and email parameters for git

git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"


## Install a theme (we are installing the Terminal theme here). Once downloaded it should be in your Hugo themes folder
## Find a theme ---> https://themes.gohugo.io/

git submodule add -f https://github.com/nanxiaobei/hugo-paper.git themes/hugo-paper

```


Setup GitHub
- Git yourself an account
- Then create a repo

Authenticate yourself


``` 
## Generate an SSH key (Mac/Linux/Windows)

ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```


Push to GitHub

```
# Step 8: Push the public folder to the hostinger branch using subtree split and force push
echo "Deploying to GitHub Hostinger..."
git subtree split --prefix public -b hostinger-deploy
git push origin hostinger-deploy:hostinger --force
git branch -D hostinger-deploy

```

