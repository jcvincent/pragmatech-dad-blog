---
title: My Blog Pipelines
date: 2025-09-28
draft: false
tags:
- pragmatechdad
- posts
---

Reference from networkchuck

Running in Windows 11

[Install Hugo on Windows](https://gohugo.io/installation/windows/)

Use Winget
[Winget](https://learn.microsoft.com/en-us/windows/package-manager/) is Microsoft’s official free and open-source package manager for Windows. To install the extended edition of Hugo:

```
winget install Hugo.Hugo.Extended
```

To uninstall the extended edition of Hugo:

```
winget uninstall --name "Hugo (Extended)"
```


Hugo

hugo new site pragmatechdad
Congratulations! Your new Hugo site was created in C:\SandBox\pragmatechdad.

Just a few more steps...

1. Change the current directory to C:\SandBox\pragmatechdad.
2. Create or install a theme:
   - Create a new theme with the command "hugo new theme <THEMENAME>"
   - Or, install a theme from https://themes.gohugo.io/
3. Edit hugo.toml, setting the "theme" property to the theme name.
4. Create new content with the command "hugo new content <SECTIONNAME>\<FILENAME>.<FORMAT>".
5. Start the embedded web server with the command "hugo server --buildDrafts".

See documentation at https://gohugo.io/.




git config --global user.name "jcvincent" 
git config --global user.email "everydaybetter@outlook.ph"

git submodule add -f https://github.com/nanxiaobei/hugo-paper.git themes/hugo-paper
