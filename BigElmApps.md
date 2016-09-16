# Beyond Hello World and Todo Lists - Ossi Hanhinen - @ohanhi

He is a front end expert at **Futurice** and has been using elm for more 
than a year.

Interesting to me: he also builds rubber-powered free-flight airplanes.

## His Purpose

Talk about the lessons he's learned as he's developed a project over a long 
period.  #1 rule: focus on solving the problem at hand; don't get distracted.

## What I Got Out of It

He confirmed what I've felt as I've developed my game engine.

* Don't be too quick to refactor into what we in Rails call "partials".  
It's more work; wait to see if the additional effort would be justified.

Some useful tips for coding I haven't encountered yet:

* Interaction outside of Elm will force handling of exceptional events.  
Separate out the exceptional events as early as possible so that the 
remainder of your app doesn't have to carry then around.
* You can put logging into case and piping statements to get good logging 
coverage of a particular area.
* Don't convert Javascript; use ports instead.  Saves time and effort and if
 you do your port implementation correctly, you will have isolated out the 
 potential for runtime errors from the external Javascript.
 
# My Notes

## Overview of projects

* Lessons learned
     * Project structure
     * Refactoring
     * Message passing
     * Code reuse
* Protips
* True Stories

### True story #1

For forms engine, wanted to write "partials" as separate modules.  More work
. So don't refactor right away; wait to see if it's useful

### Words

Triplet (init, update, view)

* init
* update
* view

Helper function, returns whatever type
"routing" "pages' in SPA with URLs

Protip # - elm-format rocks!

### Projects

"Everything is NOT a component"

#### Newspaper editing

Can choose articles and article "blocks".  Single-signon authentication used internally

#### D25

Social media app.

## True story "Real data can break your app"

Defined a context pattern

```elm
type alias Context =
  { hostname : String
  , user: User
--  , ...
  }
  
-- Page.elm
init: Contentx -> (Model, Cmd Msg)
```

Startup error caused by database int ID whose values could exceed range of Elm Int.  Changed Int to Blob type.

### Authentication

* Externalize if possible
* Your goals:
     * anonymous use
     * same app logged in/out?
     * routes differ?
     
```elm
type RemoteData e a
    = Not Asked
    | Loading
    | Success a
    | Failure e`
```
Above will help you to show the status to the user more reliably.

#### Login

```
If logged in
  got to /app/*
else
  go to /*
```

Objective: when you get to AppRouter, you no longer have a "maybe" situation due to whether he's logged in or not.

Protips:

* Put log into case statement
* Put log into piping sequences.

Variation:

```elm
task
  |> Task.map (log "great success")
  |> Task.mapError (log "here's where it fails")
```

### Project sTructure

Started w/

```
  Model
    Article.elm
    ...
    
  Update
    Article.elm
    ...
    
  Views
    ...
```

Later
```
  Article.elm
  View
    Main.elm
    Header
      ...
      ...
```

Toned down a lot of what they are testing.  Now tests functionality; end-ot-end testing is what they have discovered
they really want.

### Project Structure (later)

initial

```
/src
  Home.elm
  Feed.elm
  Router.elm
```

Later organized per use

```
/src
  Routers
     Applelm
     Toplevel.elm
  Types
     ...
  Pages
     ...
  Helpers
     ...
  Components
     ...
```

Protip: Ports are your friends.  If you want functionality in Javascript, go ahead and use it w/ a port.  If you want
to convert later, then you can.

### Summary

* reuse 
* ROI - learn what you really need to do and also what you DON'T have to do.
* structuring - don't worry about at first; as time passes you will discover what needs restructuring.

"Solve the problem at hand".  In Elm more than other languages, you don't need to worry about "fussiness" as much.  Just
code and you will discover what you need to change, and it won't be that difficult to change it then.
