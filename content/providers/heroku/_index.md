---
title: "Heroku Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
---

{{% children showhidden="true" depth="2" description="true" %}}

### Some Common Heroku Commands

* <https://dashboard.heroku.com/apps>
* git push heroku master
* heroku logs
* heroku apps:rename newname --app oldname

### Connecting the local repository directory to heroku app

1. git remote rm heroku
1. heroku git:remote -a appname

### Node configuration for Heroku

* (This should be under node configuration wiki page) go to your package.json file
* add a start configuration to your scripts section:
* "start": "node server/server.js",
* add a configuration for which node version you are running:  
* "engines": {
    "node": "9.3.0"
  },

* (This should be under node/database configuration wiki page) In your code, you want to have variables for port and uri.
* var uri = process.env.MONGODB_URI || 'mongodb://localhost:27017/databasename';
* var port = process.env.PORT || 3000;

* Navigate to your project directory
* 'heroku create'
* now you want to add the mongodb addon for your project
* 'heroku addons:create mongolab:sandbox'
* Be sure to capture your database environment variables.

### SSL Certificates

heroku certs:auto:enable
heroku certs:auto
