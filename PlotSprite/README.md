# <img alt="scientific-snap-icon" src="../images/einstein_snap.png" width="50"/> PlotSprite

One of the foundations of *Snap!*, like *Scratch*, is the *Logo*-like use of "turtle graphics" - simple pen-based drawing.  However, there is no generic means of displaying data graphically, something which is desperately needed when using *Snap!* for scientific or mathematical purposes.

The [PlotSprite.xml](./PlotSprite.xml) Sprite created by Eckart Modrow displays data in the form of simple lists of (x,y) data pairs and can also display functions of the x-axis.  The current model is to load *PlotSprite* into your project and create additional internal (**!**) *PlotSprite* methods for dealing with various plotting tasks.  Client Sprites can then invoke the global methods and *PlotSprite* can respond to global messages (e.g. the classic "green flag" start message).

---

### Example

As an example, let's create a simple set of data: when we define a global "xydata" variable and press the following blocks

![block that creates data](./images/create_data.png)

we get a corresponding list of (x,y) values (here, a simple sine function):

![created sine function data](./images/created_data.png)

After importing PlotSprite.xml into our project, let us create an internal *PlotSprite* reaction to a global "plot data" message, consisting of the response header

![respond to plot data message](./images/when_I_receive_plot_data.png)

the creation of a new plot costume (the width, height, and colour of the frame used for plotting)

![create a plot costume](./images/new_costume.png)

the initialization of the plot (definition of the plot boundaries and setting the line and marker properties)

![plot initialization](./images/plot_properties.png)

and the actual plotting of the global data list

![create plot of data](./images/create_plot.png)

When we put these pieces together

![final plot data block](./images/plot_data_block.png)

and broadcast the message to *PlotSprite* (having already created the data)

![broadcast a plot data message](./images/broadcast_plot_data.png)

we get

![line plot of data](./images/line_plot.png)

Note that we could not have created this block outside of the *PlotSprite*, since we used private blocks (the ones with the "location" and "poster" icons at the start of the block).

Of course, we could have created a "plot" block for *PlotSprite* instead of having it respond to a "plot data" broadcast message.

![a plot block](./images/plot_block.png)

Note that here, the *PlotSprite* uses markers and no lines, whereas before it used no markers and a dashed line.  The other Sprites could then create a plot not by broadcasting a "plot data" message but by directly invoking the "plot" block with it's argument containing the data to be plotted, either by using the "run" block with a passed argument

![run the plot block](./images/run_plot.png)

or by directly asking the *PlotSprite* to run it's "plot" block with the data argument.

![tell the PlotSprite to run the plot block](./images/tell_run_plot.png)

The result is a slightly different plot:

![marker plot of data](./images/marker_plot.png)

This example is available here as [Example.xml](./Example.xml).

