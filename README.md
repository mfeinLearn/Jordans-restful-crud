# Jordans-restful-crud
Jordans RESTful CRUD

## Objectives

1. Build RESTful actions for index, show, new, create, edit, update
2. Use form_for for all forms (no need to share forms or partials)
3. Correctly redirect when needed
4. Interlink between pages using link_to



```db
table "artists"
  string   "name"
  text     "bio"

table "genres"
  string   "name"

table "songs"
  string   "name"
  integer  "artist_id"
  integer  "genre_id"
```
