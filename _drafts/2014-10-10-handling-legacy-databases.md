---
layout: post
title: "Dealing with the technical debt of a legacy databases"
tags: django, python, database, migration, postgresql,mysql
---

###Technical debt

When you are taking over an existing project, or if your project is old enough, uou might encounter the problem of a legacy database, with inconsistent namings, bunch of deprecated colums and generally speaking, of simply running on mysql when you would like to use sll the power of postgresql. 

###Import legacy database

Create a new Django project

    djangoadmin startproject myproject

Open myproject/settings.py and edit DATABASES with your legacy database infos.

Then create a legacy app and use the inspectdb command to automatically generate the corresponding django models. 

    python ./manage.py startapp legacy
    python manage.py inspectdb > legacy/models.py

###model new database

###create import migration

###swap databases

###squash migrations

###cleanup