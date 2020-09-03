![scientific-snap-icon](../images/einstein_snap.png)
scientific-snap
===============

Plotting
--------

One of the foundations of Snap!, like Scratch, is the Logo-like use of "turtle graphics" - simple pen-based drawing.  However, there is no generic means of displaying data graphically, something which is desperately needed when using Snap! for scientific or mathematical purposes.

PlotSprite displays data in the form of simple lists of (x,y) data pairs.  The current model is to load PlotSprite into your project and create additional internal and global PlotSprite methods for dealing with various plotting tasks.  Client Sprites can then invoke the global methods and PlotSprite can respond to global messages (e.g. the classic "green flag" start message).

As an example, let's create a simple set of data:

<img scr="./images/create_data.png" height="50" alt="scientific-snap icon">

