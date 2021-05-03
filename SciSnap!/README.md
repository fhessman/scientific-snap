# <img alt="scientific-snap icon" src="./images/einstein_snap.png" width="75"/> SciSnap! : the Scientific Snap! Computing Environment

## INTRODUCTION

Most of the initial **scientific Snap!** examples presented here use vanilla *Snap!* plus a few helpful *Sprites* like the *PlotSprite*.
Of course, there are an amazing number of things one can do with vanilla *Snap!*, but by-and-large *Snap!* only provides the primitives needed to do generic computing tasks.
This is fine if the main goal of using *Snap!* is to learn how to programme, but if the goal is to solve more complex scientific or mathematical problems, one spends a lot of time "getting up to speed".
Other programmig languages used for maths or science are therefore extended by providing libraries for generic but more complex mathematical, statistical, or numeric problems.
A good example is the "python" language (a modern text-based, interpreted language): while "python" has a full set of primitives like variabels, lists and dictionaries and generic computer science libraries for things like threading, multiprocessing, and access to the internet, it is the "numpy" ("numeric python") and "scipy" ("scientific python") libraries that provide the higher level functions needed to actually use the language in maths and science.

To some extent, the official "Libraries" available to all *Snap!* programmers try to cover some of the additional specialied functionality needed by some - e.g. for maps, the use of sound, animation, etc. - but they cover just a small fraction of what is needed in general for truly mathematical and scientific programmers (e.g. try to find the constant "pi"!).

In order to provide *Snap!* with a similar mathematical and scientific infrastructure as enjoyed by other programming languages, Eckart Modrow - a prominant *Snap!* developer - decided to create a computing environment compatible with vanilla *Snap!* but outfitted with additional functionality and libraries for using *Snap!* at a much higher level.
The goals were
* to be 100% compatible with vanilla *Snap!* (no specialized versions of *Snap!* - just additions);
* to cover the normal range of functions needed for high school and undergraduate mathematics and science;
* to provide libraries that cover a wide range of normal mathematical and scientific needs, e.g. mathematical and scientific plotting, the use of vectors and matrices, data tables with metadata, the use of SQL databases;
* to provide additional specialized libraries for topics of particular interest, e.g. neural networks;
* to minimize the use of complicated "tell", "call", and "run" commands between *Sprites*; and
* to make the environment so configurable that it is more easily used within a high school or undergraduate teaching environment.
The result was named "SciSnap!", or "Scientific Snap!".

Given *Snap!*'s present internal structure, these goals could only be met by breaking the creation of a new project into two stages:
1. a configuration stage, where the basic libraries needed for a particular project are collected (other ones can be added later - see below); this configuration is saved as a normal *Snap!* project and can be passed on, e.g. by a teacher to her students.
2. the initial configuration is then loaded again, whereby the user interface is modified/re-organized slightly, e.g. by removing/renaming/re-organizing the block palletes to make it easier to find the blocks used later and removing the normal need to slowly collect a range of libraries.

## INSTALLATION

There is no real installation needed, other than the use of the *SciSnap!* configuration Sprite.
1. Load the latest version of *Snap!* into your browser.
2. Download the *SciSnap!* configuration *Sprite* (e.g. from here).
3. Click on the *Sprite* or invoke the "green flag" broadcast.
...

## CONFIGURATION OF A SciSnap! PROJECT

...


## SAVING YOUR SciSnap! PROJECT

...


