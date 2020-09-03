<img alt="scientific-snap-icon" src="../images/einstein_snap.png" width="50"/>

Plotting
--------

One of the foundations of Snap!, like Scratch, is the Logo-like use of "turtle graphics" - simple pen-based drawing.  However, there is no generic means of displaying data graphically, something which is desperately needed when using Snap! for scientific or mathematical purposes.

PlotSprite, created by Eckart Modrow, displays data in the form of simple lists of (x,y) data pairs and can also display functions of the x-axis.  The current model is to load PlotSprite into your project and create additional internal and global PlotSprite methods for dealing with various plotting tasks.  Client Sprites can then invoke the global methods and PlotSprite can respond to global messages (e.g. the classic "green flag" start message).

As an example, let's create a simple set of data: when we press the following blocks

![block that creates data](./images/create_data.png)

we get a corresponding list of (x,y) values (here, a simple sine function):

![created sine function data](./images/created_data.png)

After importing PlotSprite.xml into our project, we create an internal reaction to a global "green flag" starting message, consisting of the initialization of a plot (definition of the plot boundaries and setting the line and marker properties)

![plot initialization](./images/plot_initialization.png)

and 




