---
title: "PostgreSQL Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
---

{{% children showhidden="true" depth="2" description="true" %}}

### Running Your Scripts

* Make sure you are in your workspace directory.
* Run script command:
  * psql -a -f gravitywell-library/src/data/postgres/master.sql -d [dbname]
  * psql -a -f performance/scripts/sql/master.sql -d performance
* Push or pull postgres database to heroku:
  * heroku pg:push databaseName heroku-database-name --app heroku-app-name
  * heroku pg:pull heroku-database-name databaseName --app heroku-app-name
