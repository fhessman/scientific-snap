# <img alt="scientific-snap-icon" src="../images/einstein_snap.png"/> StageBrightness

There are many examples of scientific phenomenon which cannot be seen directly, but only via the observation of some indirect measure.  For example, in astrophysics, most stellar phenomena are not directly visible simply because the stars are so far away - one can only observe the amount of light coming from them. *Snap!*'s graphical capabilities makes it simple to create simulations of what is going on but cannot be seen directly, so one merely needs to be able to "observe" what is happening on the *Stage*.  The result is the current average "brightness" or "colour" of the *Stage*, normalized to the brightness or colour of a typical 8-bit pixel.

The *StageBrightnessSprite* reads some sub-image of the *Stage* and converts the pixel values into either a mean gray value (a floating point number between 0.-256.) or the mean RGB values (a list of 3 floating point numbers between 0. and 256.).  Because this conversion is compute-intensive, it is often good to limit the area which is read, so *StageBrightnessSprite* requires a global variable called **"stage_area"** consisting of a list with the values *(xmin,xmax,ymin,ymax)* in units of the *Snap!* *Stage* (which can be read using the mouse x,y reporter blocks in the "Sensing" block menu).

Here is an example of how to use the *StageBrightnessSprite*.  We first fill the *Stage* with a total black background costume so that the reported *Stage* brightness will reflect whatever else we do.
* Select the *Stage* Sprite.
* Select the "Backgrounds" tab.
* Paint a new black costume by selecting the colour black and filling the area with this color.
* Rename the new costume "black" so one can reference it later.
Now we can paste something onto the *Stage* for the *StageBrightnessSprite* to observe.
* Select or create a generic Sprite with the generic arrow costume and position the arrow somewhere on the Stage.
* From the "Pen" block menu, drag a "clear" and a "paste on .." block to the workspace.
* Select the target argument "Stage".
* Press the "clear" block to remove any other graphics from the *Stage*. ![Pen clear block](images/clear_block.png)
* Press the "paste on .." block to paste the generic arrow costume onto the *Stage*. ![Pen paste on block](paste_on_Stage.png)
