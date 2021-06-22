User Story 1
As a time-pressed user
So that I can quickly go to web sites I regularly visit
I would like to see a list of bookmarks

sequenceDiagram
	User->>+Browser: clicks `todolist`
  Browser->>+Controller: GET /todolist
  Controller->>+Model: Todolist.items
  Model->>-Controller: Array of item objects
  Controller->>+View: render :todos with @items
  View->>-Controller: HTML
  Controller->>-Browser: 200 OK, body HTML
  Browser->>-User: see to list

Bookmark Manager

This code is intended as a supplementary guide for [bookmark manager](https://github.com/makersacademy/course/tree/master/bookmark_manager). The commits on master branch roughly correspond with the walkthroughs provided in the challenge.

## User Stories

```
As a time-pressed user
So that I can quickly go to web sites I regularly visit
I would like to see a list of bookmarks
```

## Domain Model

## Domain Model

![Bookmark Manager domain model](./public/images/bookmark_manager_1.png)


## How to use

### To set up the project

Clone this repository and then run:

```
bundle
```

### To run the Bookmark Manager app:

```
rackup -p 3000
```

### To run tests:

```
rspec
```

### To run linting:

```
rubocop
```
# Bookmark_Manager
