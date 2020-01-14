---
title: "Composer Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
---

For PHP Laravel, most of the commands are run from php and composer.

### Checking Installation

* Be sure your stuff is installed
* See the composer version by typing 'composer' in the terminal.
* Point composer to the php version you installed. See the wiki.

### Creating a site

1. Navigate to your workspace where you want the project to live. Run:
1. composer create-project --prefer-dist laravel/laravel blog
1. Navigate to your new project directory. To run the site, run:
1. php artisan serve

### Adding packages

* Example for adding UI scaffolding with Vue:
* composer laravel/ui --dev
* php artisan ui vue
* npm install (installs the vue and node packages)
* npm run dev (builds the Vue files)
