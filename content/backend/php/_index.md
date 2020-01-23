---
title: "PHP Notes"
date: 2020-01-13T14:11:32-06:00
draft: false
---

{{% children showhidden="true" depth="2" description="true" %}}

### Setup and Configuration

* Download and install the latest version of PHP.
* I want my root directory to be clean, so I install to "C:\Program Files\php-7.3.11".
* Checking version: php -v
* Be sure php is in the Path variable.
* When I moved my php directory on my laptop, for some reason the php.ini got lost.
* I tried a lot of things, but what ultimately worked was to re-run the composer setup executable. It asked if I wanted to create a php.ini file, which is what I was trying to figure out.

### Visual Studio Code Extensions

* Laravel Blade Spacer
* Laravel Blade Snippets
* Laravel goto view
* PHP DocBlocker
* PHP Getters & Setters
* PHP import checker
* PHP Intelephense
* PHP Namespace Resolver

### Creating a new php application

* TODO: Add instructions.

### Running a server

* TODO: Add instructions.

### Using the PDO

* <https://phpdelusions.net/pdo>
* <https://www.php.net/manual/en/pdo.prepared-statements.php>
* <https://www.php.net/manual/en/pdo.transactions.php> (Important Note: The cursor remains open until the end of transaction, and since PostgreSQL works in auto-commit mode by default, the cursor is closed immediately after the procedure call, so it is not available to the caller. To work with cursors the caller have to start a transaction.)
* <https://www.php.net/manual/en/book.pdo.php>
* <http://www.nusphere.com/kb/phpmanual/ref.pdo.htm>
