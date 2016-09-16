# Q/A Session w/ panel

# Selling Elm to Customer?

* Admit what the risk.
    * Not the developer group size.
    * People will lose interest.
* Communicate the benefit (stability, changeability).
    * Elm has some dominating advantages.
         * Compile/no runtime error
         * Claim 2-week learning curve for Elm (don't quite believe it myself, but maybe)
* People want to hear different things.
    * "Do you like to work in Javascript?" Developers: no
    * "Zero runtime exceptions" - Managers. yeah!
* Consultants frequently trusted by client to make programming language choice.
    * Easy to choose Elm in that case.
    * Python paradox.
        * Developers like Python -- motivated.
    * NoRedInk finds hiring front end developers (Elm) much easier than before.  Almost impossible to hire non-Elm
      developers.
* If stakeholder not receptive, suggest waiting a year.  Remember you're not giving up.
    * Takes courage; things will seem really slow.
    
# Working w/ Designers

Remember that Elm is awesome for designers.

When designers give you CSS and HTML and ask you to make it work.

R Feldman: "designers are smart people and can learn Elm."  Argues that Elm is easier to understand than CSS.

But what about taking away all "their tools"?  There is a tool: HtmlToElm to convert html to elm.

Designers collaborate on corner states (like "loading...").  visual vs code but both are necessary.

# Binary Trees

If through ports, use a set

# What should not be a component?

Only something that is completely separated from the rest of the application should be considered to be a component.

Object hierarchies can be thought of functions.  When things get crazy, make helper functions.

A component can be thought of as a module w/ an associated data structure (what I thought anyways).

Feldman thinks data modeling is harder than isolation.

# Participate

If you don't, then people don't know you.  In such cases, is irresponsible to take your word for what you assert you can
do..

# Haskell barriers to maintenace of Elm-lang.org

Evan: jsut change teh pieces that are not haskell sensitive.

Watch people and the problems they run into.

If you stumble on something, you should take the stumbling to the community.

# Effect Managers

A piece that isolates your Elm stuff from interacting w/ the server.  Effect managers manage that.

Perhaps one kind of effect manager for each server type.

# Showing Appreciation?

Be nice when flagging issues; realize that the team is trying really hard.

