# <img alt="scientific-snap icon" src="../images/einstein_snap.png" width="75"/> SciSnap! : the Scientific Snap! Computing Environment

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

SciSnap! is now an official library that can be loaded directly using the "Import" menu.

---

## Documentation

Modrow's extensive introduction to *SciSnap!* is available at http://www.emu-online.de/ProgrammingWithSciSnap.pdf (English) and http://www.emu-online.de/ProgrammierenMitSciSnap.pdf (German).  He gives detailed examples from all of the new *SciSnap!* categories.


---

## The SciSnap! Categories

With *SciSnap!*, it is possible to extend the pallette of categories beyond those in normal *Snap!* ("Motion", "Looks", "Sound", "Pen", "Control", "Sensing", "Operators", and "Variables").
In the standard *SciSnap!* configuration there are additions to the standard catagories as well as fuly new ones:


---

### 0. My own blocks

This is a category area for your own blocks, which makes them easier to find than when they are spread out all over the other categories.

---

### 1. SciSnap! globals

This category is usually only needed to start the SciSnap! environment using the "start SciSnap!" block.

---

### 2. Math tools

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

---

### 3. Data tools

These block are similar to those found in the "Variables" category" but are more powerful: these blocks create and manipulate tables of data.

---

### 4. SQL tools

These block can be used to perform formal database operations, just like in the professional world - as long as you have a connection to a server!

---

### 5. Plotpad for data plots

This is the *SciSnap!* version of the old scientific-snap *PlotSprite*, used to create x-y plots and histograms of data.

---

### 6. ImagePad for image operations

*Imagepad* offers a range of image processing and drawing functions:
- pixel arithmetic;
- grayscale-RGB transformation;
- drawing circles and rectangles;
- reading image values via a mouse or by coordinates;
- support for different image file formats;
- support for simple FITS images (astronomical standard) with metadata.

---

### 7. GraphPad for graph operations

Here, "Graph" means graphs in the sense of mathematical graph theory.
These are blocks that manipulate the connections between objects.
Such connections are used to represent networks and  hierarchies of connections.
The "pad" part means that there are tools for representing such networks graphically as
geometric objects connected by lines.

---

### 8. NNPad for neural networks

The "NNPad" category stands for "Neural-network pad" and provides block by which simple neural networks can be constructed, trained, used, and displayed.
