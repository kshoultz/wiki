---
title: "Hugo Wiki Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
weight: 50
---

{{% children showhidden="true" depth="2" description="true" %}}

* I have the hugo environment set up on my main machine. I'd like to capture this process in the wiki.
* I have only the github repository on my laptop. I can make content changes from the laptop.
* I only have one Hugo site. I want to revisit the installation and see if I can have the Hugo sites in my main workspace with other framework sites.
* My theme for this wiki is a submodule. I'd like for it to be a copy, so that I can modify the theme.

### Hugo intsallation:

* Why do I want Hugo? 
  * I'd like to have an easy to modify wiki that uses markdown, and keeps from being fancy.
* Downloaded a hugo binary from the github:
  * <https://github.com/gohugoio/hugo/releases/tag/v0.85.0>
* Extracted it to C:/Hugo
* Make sure chocolaty is installed from your node installation.
* Run the isntallation for hugo from an adminstrator started shell:
  * choco install hugo -confirm
* Generate a new hugo site:
  * hugo new site site_name
* Add the theme to the site:
  * git submodule add <https://github.com/matcornic/hugo-theme-learn> themes/learn
* Start the hugo server:
  * hugo server.
