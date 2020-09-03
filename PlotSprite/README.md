<img alt="scientific-snap-icon" src="../images/einstein_snap.png" width="50"/>

Plotting
--------

One of the foundations of Snap!, like Scratch, is the Logo-like use of "turtle graphics" - simple pen-based drawing.  However, there is no generic means of displaying data graphically, something which is desperately needed when using Snap! for scientific or mathematical purposes.

PlotSprite, created by Eckart Modrow, displays data in the form of simple lists of (x,y) data pairs and can also display functions of the x-axis.  The current model is to load PlotSprite into your project and create additional internal and global PlotSprite methods for dealing with various plotting tasks.  Client Sprites can then invoke the global methods and PlotSprite can respond to global messages (e.g. the classic "green flag" start message).

As an example, let's create a simple set of data: when we define a global "xydata" variable and press the following blocks

![block that creates data](./images/create_data.png)

we get a corresponding list of (x,y) values (here, a simple sine function):

![created sine function data](./images/created_data.png)

After importing PlotSprite.xml into our project, let us create an internal PlotSprite reaction to a global "plot data" message, consisting of the response header

![respond to plot data message](./images/when_I_receive_plot_data.png)

the creation of a new plot costume (the width, height, and colour of the frame used for plotting)

![create a plot costume](./images/new_costume.png)

the initialization of the plot (definition of the plot boundaries and setting the line and marker properties)

![plot initialization](./images/plot_properties.png)

and the actual plotting of the global data list

![create plot of data](./images/create_plot.png)

When we put these pieces together

![final plot data block](./images/plot_data_block.png)

and broadcast the message to PlotSprite (having already created the data)

![broadcast a plot data message](./images/broadcast_plot_data.png)

we get

![plot of data](./images/plot.png)


Of course, we could have create a "plot data" block instead of responding to a "plot data" broadcast message.

