# Lightning Talks

## Matthew Griffith - Animation in Elm

### His Purpose

Show the "spring" metaphor for CSS animation and how it's better.

### What I Got Out of It

I learned that the "spring" metaphor is, indeed, superior to what I used in 
my game engine because it taks the time duration component out.  This is 
important when you receive competing outside events to your animation; the 
automated result with "spring" is more likely to do what you want in such 
situations.
 
## My Notes


* Shows gear mechanism.
* Elm-style animation library version 3 released this morning.


Purposes

...make it easier

ok, I got this thing
it needs to fade in and change position
I need to know when its done

Shows really nice interface; neee to look at this.

What if the animation is already doing something?

* smoothly interrupt it
* queue up after it

How do we get from A to B?

* duration + easing
* springs (default)

Why Springs?

* easy to model clean interruptions
* easier to adjust as an animation designer

Why do Springs seem more difficult?

* very hard to model correctly in css animations
* you have to build an intuition about them

Building an intuition for springs

* stiffness
     * how fast does it move?
* damping
     * how fast does it settle?
     
duration is a secondary property of the spring.

This is important for interruptions.

### Examples

* Stagger Movement
* Slight delay on following the mouse
* CSS Filters
* Polygon Transitions (through SVG)
* Shadows

---

## Functional Data Structures - Tessa Kelly - NoRedInk @t_kelly9

**[slides](http://bit.ly/2cxDOLw)**

### Her Purpose

Explain the pros and cons of different strategies for implementing binary 
trees in Elm.

### What I Got Out of It

When implementing a complex data structure and its API, try out different 
Elm collection packages and see which one works better.  I was surprised to 
learn that simple linked lists were the most appropriate.
 
## My Notes (note: partial and not very coherent)

Binary Tree API

* Array
* Dict
* Tree | & ||

Array Based

Stragety:

* Use Array as our base
* Derive child indices
* Hope for a complete binary tree

Summary: interesting presentation of 4 ways to attack the implementation design.

---

## ABadi Kurniawan - Building a RealTime app w/ Elm and Horizon

https://horizon.io

### His Purpose

For some applications, an Elm client doesn't need a classic web application.
  Hs shows how to get everything he needs from Firebase through a product 
  called Horizon.

### What I Got Out of It

Interesting, but I believe the number of applications that will be able to 
survive w/ so little server business rule knowledge is seriously limited.

## My Notes

Shows how to use Horizon/Elm to keep all development in the client.

I think it is an API to go back to Firebase.

Shows simple chat application implementation.

Presenter built an **Elm Horizon** as an Elm API to Horizon.


https://abadi199.github.com/elm-conf - slides


