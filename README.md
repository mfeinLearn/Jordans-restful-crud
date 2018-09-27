# Jordans restful CRUD lab

## Objectives

1. Build RESTful actions for index, show, new, create, edit, update, delete 
2. Use form_for for all forms
3. Correctly redirect when needed
4. Interlink between pages using link_to

## Overview

You have been given the task to build a Rails app called **Jordans Fly**, this app is to help shoe collector keep track of their shoes. **Jordans Fly** is an app that shows all of shoes an owner's shoe collection via an app

## Instructions

You'll need to create all of the migrations, models, routes, controllers, and views for this lab.


1. Create migrations and models for:
* owner
* shoes

- This is a one to many relationship
* A shoe belongs_to an owner
* An owner has_many shoes

```db
table "owners"
  string   "name"

table "shoes"
  string   "name"
  string   "brand"
  string   "size"
  string   "owner_id"
```

2. Create a `Owner#index` page that displays a i)list of  all owner's name ii)a count of how many shoes they owe iii)have the name of the owner as a link to their show page.

3. Create a `Owner#show` page that displays i)the owner's name, ii)display all of the brand of the shoes that the owner owns.

4. Create a `Shoe#index` page i)display all of the brand of the shoes that is in a database.

5. Create a `Shoe#show` page that lists the name,brand, size, of the shoe.

* You can use the `resource`, `model`, `migration`, and `controller` generators, but do not use the `scaffold` generator
*Top Tip: Remember to use the --no-test-framework flag when generating models and controllers to avoid generating unnecessary testing frameworks!*

***NOTE***: As with much of our Rails curriculum, remember to always use the `--no-test-framework` flag when you generate models, controllers, etc. That way, the Rails generators will not create additional tests on top of the test suite that already comes with the lesson. E.g., `rails g model User username:string email:string --no-test-framework`.

