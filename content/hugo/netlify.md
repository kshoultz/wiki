---
title: "Netlify Host Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
---

* Your netlify account can connect to a github repository.
* My hugo repository is automatically recognized and Netlify does everything for me.
* As a note, one problem I ran into was a deleted submodule file. I just restored the .gitmodules file and everything worked fine.
* I also added a .gitignore file to ignore the public directory that gets generated. No need to commit those files because Netlify will build and generate those files.
* I'll want to register a custom domain to this wiki.
