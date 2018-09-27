# Jordans-restful-crud
Jordans RESTful CRUD

## Objectives

1. Build RESTful actions for index, show, new, create, edit, update, delete 
2. Use form_for for all forms
3. Correctly redirect when needed
4. Interlink between pages using link_to



## Instructions

You have been given the task to build a Rails app called **Jordans Fly**, the app will need to have two separate models:
**Jordans Fly** is an app that shows all of shoes an owner's shoe collection via an app


The models that you need loo
* owner

* shoes

Also dont forget to include an owner controller and shoes controllers 
and also dont forget to include views - show, edit, new


The data relationship will look something like this:

* A shoe belongs_to an owner

* An owner has_many shoes

(This is a one to many relationship)



Your database should look like the following:

```db
table "owners"
  string   "name"

table "shoes"
  string   "name"
  string   "name"
  string   "size"
  string   "color"
  string   "owner_id"
```

Make sure the app has the following components:


index, show, new, create, edit, update
2. Use form_for for all forms
3. Correctly redirect when needed
4. Interlink between pages using link_to


* You can use the `resource`, `model`, `migration`, and `controller` generators, but do not use the `scaffold` generator
*Top Tip: Remember to use the --no-test-framework flag when generating models and controllers to avoid generating unnecessary testing frameworks!*
