# Lists

We use lists all the time. We have lists in our heads like:

* Our favorites movies
* Our favorite foods
* Our closest friends

We also have lists we can use to accomplish a task. For example, a grocery lists helps us make sure we get what we need at the store:

1. Milk
2. Cheese
3. Eggs
4. Chicken
5. Tomatoes
6. Cucumbers

In real life, people use checklists to make sure they do everything right every time. For example, a pilot's checklist before takeoff or before landing.

```
Before-Takeoff Checklist

    Auxiliary fuel pump — Off
    Flight controls — Free and correct
    Instruments and radios — Checked and set
    Landing gear position lights — Checked
    Altimeter — Set
    Directional gyro — Set
    Fuel gauges — Checked
    Trim — Set
    Propeller — Exercise
    Magnetos — Checked
    Engine idle — checked
    Flaps — As required
    Seat belts/shoulder harnesses — Fastened
    Parking brake — Off 

Final items

    Doors and windows — Locked
    Mixture — Full rich unless above 3,000 feet msl
    Lights — Landing, taxi, strobes on
    Camera — Transponder on
    Action — Engine instruments checked

Before-Landing Checklist

    Fuel selector — Fullest tank
    Directional gyro — Aligned with magnetic compass
    Seat belts/shoulder harnesses — secure
    Mixture — Full rich unless airport above 3,000 feet msl
    Cowl flaps — As required 

Final items

    Landing gear — Down
    Propeller — High rpm
    Flaps — As required
```

> Checklists will keep you safe.

In more abstract terms, we can think of lists as a collection of items, that may or may not be ordered, that all relate to each other in some way (the reason for having the list).

In programming, we often have a collection of things we need to work with in some way. Some things we do with collections, aka lists.

## Examples

With a `list of numbers` I can:

* Find the item with the highest/lowest value
* Sum all numbers into a total
* Sort the list from highest to lowest or lowest to highest.

With a list of `things` I can:

> In some video games, you can collect items and use them in the game. Those items are stored in a list.

* Find a thing in a list and use it or operate on it.

With a list of `actions` I can do each action in order:

* Move 10 steps
* Turn 90 degrees
* Glide to nearest edge and bounce

With a list of conditions and actions I can compare against the current state and do the relevant action.

> sometimes called a state engine

* When X is 15, then glide 37 steps 90 degree from current location
:
:

## Say every letter in a word

In many programming language a word, also known as a string, is considered a list of characters. For example:

"Hello, World!" is actually a list that looks like this:

H -> e -> l -> l -> 0 -> , -> W -> o -> r -> l -> d -> !

The computer considers Hello, World! to be a list of characters where each character points to the next one in the sequence.

Try out the Do Now
https://snap.berkeley.edu/snapsource/snap.html#present:Username=whuangpha&ProjectName=Starter%20project%20for%20text%20operators%20practice


## You talking to me?

https://tealsk12.gitbook.io/intro-cs/unit_4/lesson_42/lab_42

>  create a sentence generator using lists
