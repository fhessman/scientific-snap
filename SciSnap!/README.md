# <img alt="scientific-snap icon" src="./images/einstein_snap.png" width="75"/> SciSnap! : the Scientific Snap! Computing Environment

## Introduction

Most of the initial **scientific Snap!** examples presented here use normal *Snap!* plus a few helpful *Sprites* like the *PlotSprite*.
Of course, there are an amazing number of things one can do with normal *Snap!*, but - by and large - *Snap!* only provides the primitives needed to do generic computing tasks.
This is fine if the main goal of using *Snap!* is to learn how to programme, but if the goal is to solve more complex scientific or mathematical problems, one spends a lot of time "getting up to speed".
Other programming languages used for maths or science are therefore extended by providing libraries for general purpose but more complex mathematical, statistical, or numeric problems.
A good example is the "python" language (a modern text-based, interpreted language): while "python" has a full set of primitives like variables, lists and dictionaries, and generic computer science libraries for things like threading, multiprocessing, and access to the internet, it is the "numpy" ("numeric python") and "scipy" ("scientific python") libraries that provide the higher level functions needed to actually use the language in maths and science.

To some extent, the official "Libraries" available to all *Snap!* programmers try to cover some of the additional specialied functionality needed by some - e.g. for maps, the use of sound, animation, etc. - but they cover just a small fraction of what is needed in general for truly mathematical and scientific programmers (e.g. try to find the constant "pi"!).

In order to provide *Snap!* with a mathematical and scientific infrastructure similar to that enjoyed by users of other programming languages, Eckart Modrow - a prominant *Snap!* developer - decided to create a computing environment compatible with normal *Snap!* but outfitted with additional functionality and libraries for using *Snap!* at a much higher level.
The goals were
- to be 100% compatible with normal *Snap!* (no specialized versions of *Snap!* - just additions);
- to cover the normal range of functions needed for high school and undergraduate mathematics and science;
- to provide libraries that cover a wide range of normal mathematical and scientific needs, e.g. mathematical and scientific plotting, the use of vectors and matrices, data tables with metadata, the use of SQL databases;
- to provide additional specialized libraries for topics of particular interest, e.g. neural networks;
- to minimize the use of complicated "tell", "call", and "run" commands between *Sprites*; and
- to make the environment so configurable that it is more easily used within a high school or undergraduate teaching environment.
The result was named "SciSnap!", or "Scientific Snap!".

Given *Snap!*'s present internal structure, these goals could only be met by breaking the creation of a new project into two stages:
1. a configuration stage, where the basic libraries needed for a particular project are collected (other ones can be added later - see below); this configuration is saved as a normal *Snap!* project and can be passed on, e.g. by a teacher to her students.
2. the initial configuration is then loaded again, whereby the user interface is modified/re-organized slightly, e.g. by removing/renaming/re-organizing the block palletes to make it easier to find the blocks used later and removing the normal need to slowly collect a range of libraries.

## Installation

There is no real installation needed, other than the use of the *SciSnap!* configuration Sprite.
1. Load the latest version of *Snap!* into your browser.
2. Download the *SciSnap!* configuration *Sprite* (e.g. from here).
3. Click on the *Sprite* or invoke the "green flag" broadcast.
...


## The SciSnap! Categories

With *SciSnap!*, it is possible to extend the pallette of categories beyond those in normal *Snap!* ("Motion", "Looks", "Sound", "Pen", "Control", "Sensing", "Operators", and "Variables").
In the standard *SciSnap!* configuration there are additions to the standard catagories as well as fuly new ones:


### Looks

Here are the blocks for manipulating categories:
- setting up *SciSnap!*;
- adding new categories;
- hiding (old) categories;
- importing libraries to categories.

The most important new block here is the ![Switch to SciSnap!](./images/Switch_to_SciSnap.png) block needed to re-configure normal *Snap!* into *SciSnap!*.


### Math

This category contains a wide range of standard mathematical functions and objects, from relatively simple things found in high school mathematics to more advanced things found in undergraduate topics: e.g.
- sets;
- complex numbers;
- vectors, matrices, and tensors;
- series;
- integration and derivation;
- polynomials;
- solutions to standard equations;
- root finding;
- statistical distribution functions.

### Plotpad

This is the *SciSnap!* version of the scientific-snap *PlotSprite*.

### Imagepad

*Imagepad* offers a range of image processing and drawing functions:
- pixel arithmetic;
- grayscale-RGB transformation;
- drawing circles and rectangles;
- reading image values via a mouse or by coordinates;
- support for different image file formats;
- support for simple FITS images (astronomical standard) with metadata.


### Sql

This category replaces Modrow's specialized SQL-version of *Snap!* and offers a full set of SQL functionality for accessing local or network databases.


### Control

Some *Sprite* manipulation blocks.


### Sensing

The ![datetime](../images/datetime.png) function that returns the current datetime in ISO format: a string containing both the date and time in the format YYYY-MM-DDThh:mm:ss


### Operators

A variety of new operator functions and constants are contained here:
- important numerical constants like "pi" and "e";
- mathematical functions like factoral, binomial coefficients, and a random number generator (0 to 1);
- a handy function for rounding decimal numbers;
- string manipulations;
- writing text to files;
- convertion of datetimes to fractional hours, minutes, or seconds of the given day.


### Data

Here are a large number of blocks that enabe the creation and manipulation of tabular data, with or without metadata (column/row labels).
Included are such advanced things as 
- grouping data;
- statistics;
- sorting;
- convolution.
- regression;


### Graphpad

Here, "Graph" means graphs in the sense of mathematical graph theory.
These are blocks that manipulate the connections between objects.
Such connections are used to represent networks and  hierarchies of connections.
The "pad" part means that there are tools for representing such networks graphically as
geometric objects connected by lines.


### Nnpad

The "Nnpad" category stands for "Neural-network pad" and provides block by which simple neural networks can be constructed, trained, used, and displayed.


### Myblocks

This empty category with the traditional gray color is for your own blocks, so that it is easier to find them without having to pour through dozens of standard blocks.

