# Nightingale.space - Elm and Crowd-Sourced Music Making - Murphy Randle

Organizer of js.alt meetup

## His Purpose

Elm implementation of simple app to collect music "sheets" as note codes and
 collect them from Twiter contributors.
  
## What I Got Out of It

Clever.  Learned about Elm packages that do regular expressions.  
Implementation was very efficient. Need to learn what `<|>` symbol means.
 
# My Notes

## Scenario

Desire to fit music into 140 bytes on Twitter.


### Plan

* A-G for note
* letter to indicate whether sharp or flat
* Letters to indicate note duration
* Letter to indicate which octave.

### Implementation

1.  Pull song from host.  (Use Elixir)
1.  Shows Elixir code running on server to show the channel
1.  Consuming a Phoenix channel
    * Uses fbonettic/elm-phoenix-socket
1.  Breaks the channel communication into a Note record
1.  Showed TDD
1.  Parser library bogdamp/elm-combine
    * Uses regexes to parse the string
    * Using `<|>` which I haven'g seen before.
1.  Uses a port to send it to the JS-based music generator.
    * shows how Maybe is used to handle "accidental" vagarity.
1.  Shows how Elm highlights each note when it is played.
