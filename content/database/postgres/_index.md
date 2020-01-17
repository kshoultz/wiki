---
title: "PostgreSQL Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
---

{{% children showhidden="true" depth="2" description="true" %}}

### Installation and Configuration

* The latest version as of this documentaion is PostgreSQL 12.1
* If you have a previous version of PostgreSQL, you'll want to run the uninstaller executable first.
* Download and install the latest version of PostgreSQL.
* Be sure to take note of your database credentials.
* Be sure the installation bin is on your PATH system variable.
* Check the installation at the command line by running psql --version

### Running Your Scripts

* Make sure you are in your workspace directory.
* Run script command:
  * psql -a -f gravitywell-library/src/data/postgres/master.sql -d [dbname]
  * psql -a -f performance/scripts/sql/master.sql -d performance
* Push or pull postgres database to heroku:
  * heroku pg:push databaseName heroku-database-name --app heroku-app-name
  * heroku pg:pull heroku-database-name databaseName --app heroku-app-name

### General Notes

* I've installed a PostgreSQL extension to Visual Studio Code.
* It seems to work pretty well for peeking into data.
* I'd like to bind the keyboard shortcuts to some that I'm familiar with (cTRL+ENTER to run scripts).
* I have a local database set up and databases connected to a few of my Heroku sites.
* The main stand alone tool for PostgreSQL is pgAdmin.
