---
title: "NPM.org"
date: 2020-01-13T14:11:32-06:00
draft: false
weight: 50
---

{{% children showhidden="true" depth="2" description="true" %}}

### Logging Into NPM

* Navigate to your workspace directory.
* npm login
* Username: jdoe
* Password:
* Email: (this IS public) jedi.kevo@gmail.com
* Logged in as kshoultz on <https://registry.npmjs.org/>.

### npmjs.com

* <https://www.npmjs.com/docs/orgs/publishing-an-org-scoped-package.html>
* <https://docs.npmjs.com/private-modules/ci-server-config>
* Create a user
* Create an organization.
* Scope your package/project. (@namespace/project)
* Publish your project to npm (it is private by default).

### Updating a package

* npm version patch|minor|major

### NPM LINKING

* Go to the project you want to provide as a link:
* npm link
* go to the directory project where you want to use it.
* npm link gravitywell-library
* Use the following in your node projects to include it.
* require('gravitywell-library');
