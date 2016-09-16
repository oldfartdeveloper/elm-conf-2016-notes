# Rolling Random Romans -- Joel Quenneville - Thoughtbot

## His Purpose

Illustrate via example some of the pitfalls of having numerous sources of 
randomness and how to avoid them.

## What I Got Out of It

I learend that functions returning random values are, by definition, not 
pure functions and that his raises holy hell w/ testing.  By associating 
seed values to the API, you can now get consistent results.  He also showed 
ways to hide the seed value.
 
# My Notes

Time-travel Republican Rome.

Me - ancient software engineer

Goddess Juno has a problem for you to solve

Your mission - automate her task

1.  Build a dashboard for all of Rome's children
1.  Automatically name the kids
1.  Algorithm for naming.

## Mens' names

Publius - personal name
Cornelius - Clan name
Scipio - Nickname.  Can be inherited.
Africanus - Honorific title

Last two are optional.

## Women's names

Cornelia - last name of husband
Africana - inherited honorific
xxx - xxx

Shows how he models and implements it.

Pure functions always return the same value.  This is a problem for random

Random is inherently not pure

By adding a seed, can be pure.

Called Pseudo-random

Not for secure functions; random not secure.

Suggestion: work from the bottom up


