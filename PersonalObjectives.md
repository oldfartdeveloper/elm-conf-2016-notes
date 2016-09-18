# Personal Objectives

No, this wasn't an "official" conference session, but it dovetails nicely 
with what Evan Czaplicki's aspirations for the Elm community are.

Click **[here](https://github.com/oldfartdeveloper/elm-conf-2016-notes/blob/master/README.md)** for the (more conventional) rest of my notes from 
the conference.

# TL;DR Risk Leaving My Comfort Zone to Participate More

Yeap, i.e. put myself out there more.  I've finally realized that my 
personal goals for my joy in software development are vastly enhanced by 
fully participating in communities.  Otherwise progress is slow and, 
frankly, lonely (and not much fun).
 
The Elm community is one I really enjoy participating in; it was an 
incredible privilege to attend this conference.

So I set the following goals for my participation this time:

# Goals for the Conference

In order of importance.

1. Introduce myself to the **[BDFL](https://en.wikipedia.org/wiki/Benevolent_dictator_for_life)** (Evan) and Richard Feldman
1. Talk (a lot) with the other attendees
1. Write about my experience (and publish it for gawds' sakes)
1. Learn from the sessions
1. Participate w/ the others in the extra-curricular activities

Here's How It Went

## Introduce myself to the BDFL (Evan) and Richard Feldman

This was the most challenging one for me; I had/have all these 
"considerations":

1. Have I done enough with Elm to not sound like an ignoramous?
1. Why do I want to do this; I hate wasting other peoples' time.
1. What communication do I want to have with these two people and why?
1. After the considerations above, do I still want to have this 
communication? Ugh.

Okay, so where do I stand on the above?

1. I've implemented a simple but non-trivial **[animating game engine](https://github.com/oc-elixir-elm/diamondback-railroad/blob/master/README.md)**.  
Hopefully takes me from "newbie" to at least "low intermediate".
1. I want to do this to be part of the Elm community and to contribute to it
. Gotta get started somewhere; this is the time.
1. The communication I want this time w/ Evan is different from the one I 
want w/ 
Richard; see below.
1. Yeah, I think I do want to make this effort.

---

For Evan I've had an itch to do something about making the SVG library more
 user-friendly or perhaps implement a new package over it.  I wanted his 
 take on it, so we had this conversation:

***Question: What is the status and direction of the existing [Graphics 
package](http://package.elm-lang.org/packages/elm-lang/svg/1.1.1/Svg)***

&nbsp;&nbsp;&nbsp;Answer: ultimately going to use HTML 2D/3D? graphics 
engines, but for performance right now should use SVG.

The **[existing SVG package](https://github.com/elm-lang/svg/blob/1.1.1/README.md)** states that it is a stable low-level API that 
won't be changing much.  Hence, obviously my contribution would be a 
higher-level API.  My immediate need is to have an easier to use interface 
to define an *ellipse arc*.  So:

***Question: Does he know of anyone working on such an effort (ellipse 
arc)?***

&nbsp;&nbsp;&nbsp;Answer: no, not yet.

***Question: How comprehensive should the solution be?***

&nbsp;&nbsp;&nbsp;Answer: depends.  Some ideas:

1. Just "fix" what you want for the ellipse.  Call your community package 
**svg ellipse**, **svg ellipse helpers**, or ?.  *Advantages:* quick 
implementation.  Easy to document.  *Disadvantages:* lacks context; under 
what circumstances would a programmer be looking for this?  Proliferates 
another small package into the **[community packages](http://package.elm-lang.org)** which may make it hard to know how to find it.

1. Provide a community "repository" package for all SVG higher-level 
functionality.  Call it **svg helpers** or ? *Advantages:* If you can get 
the community to use your package as the target for their efforts, there could
 be some real 
synergies.  Friendlier SVG APIs would be much easier to find.  
*Disadvantages:* this could be a LOT of work involving organizing and 
coordinating lots of contributions if the community buys into it.  There would 
be constant revision increments.  And what is submitted may stylistically 
differ from other submissions so that it ends up being a "mishmash".  Seems 
like this would only work out if it were one person's vision to bring up the
 level of abstraction across all of SVG together.  If there already exists 
 a similar package in another programming language (like Javascript), then 
 porting that library might be attractive.  Or perhaps the API of the 
 existing graphics package might be an API design baseline; **[Kwarrtz](https://github.com/Kwarrtz)** 
 already has such a **[package](http://package.elm-lang.org/packages/Kwarrtz/render/latest)** started.

1. Would the ellipse functionality be part of a larget package that uses the
 ellipse package?  For example, would this be part of a library that 
 manipulates the **movement of creatures** (rendered largely by ellipse arcs)
 in a 
 game?  Perhaps it 
 should be part
  of that library.  *Advantages:* improved ellipse API now associated with 
  significant game component; easier to locate and, given the context, 
  probably easier to understand and apply.  *Disadvantages:* Now 
  "officially" disassociated with other future SVG API packages.
  
&nbsp;&nbsp;&nbsp;Evan suggested discussng it in the developers' slack channel.

In summary: I don't have to rush it; rather I have the time and can think about
 it and discuss and 
              discover the right direction to go.  *I can be relaxed.*
              
Right now I'm tempted to add the ellipse arc functionality I want into 
**Kwarrtz's** 
package above and then build my **creature** package on top of it.  But I'll
 run it by people in the community; they may have even better ideas that 
 will save me effort and/or improve the result.

---

For Richard, I just wanted to let him know how many "sweet spots" he touches
 in his presentations.  So I did.  He was genuinely appreciative.
 
Since the
  conference, I've bought **[his MEAP book](https://www.manning.com/books/elm-in-action)** and have already made suggestions to the book.
    Btw, he writes as well as he presents.

## Talk (a lot) with the other attendees

This was a constant focus during breaks and lunch; I probably talked w/ at 
least 20 different people.  It became easier as the day went on, I made 
some really interesting friends, and I found out a lot of great stuff!
 
## Write about my experience (and publish it for gawds' sakes)

Yeah, **[published my notes here yesterday](https://github.com/oldfartdeveloper/elm-conf-2016-notes/blob/master/README.md)** and will publish this page shortly.

## Learn from the sessions

I did.  But the surprise for me is that I feel like "scales fell from my 
eyes" on the community discussions and presentations; how important they are
.  I need the community to help me get-in-sync so that they can help me 
select better objectives and be supported in achieving them.  And they need 
me to do the same for them.

## Participate w/ the others in the extra-curricular activities

I'm so glad I went to **[City Museum](http://www.citymuseum.org/visit/)**; certainly one of the most amazing 
places I've ever been.  Loved it.  And we were all ooh-ing and ahh-ing and 
laughing (nervously at times when exploring scary confines like 10 story 
slides).  It encouraged me to take more risks, *live* a little more.
