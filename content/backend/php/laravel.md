---
title: "Laravel Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
---

### Downloading An Existing Laravel Site

1. git clone <https://github.com/theirdomain/theirproject> yourdirectory
1. php artisan key:generate (.env does not get committed to git).
1. composer install
1. npm install

### Creating a New Site

1. Navigate to your workspace where you want the project to live. Run:
1. composer create-project --prefer-dist laravel/laravel blog
1. Navigate to your new project directory. To run the site, run:
1. php artisan serve

### Create the Vue Scaffolding

* composer laravel/ui --dev
* php artisan ui vue
* npm install (installs the vue and node packages)
* npm run dev (builds the Vue files)
* These files are deployed to the public directory
* You will need to tie the vue framework to the blade and implementation. See the Vue wiki.
* php artisan serve
