# <img alt="scientific-snap icon" src="./images/einstein_snap.png" width="75"/> Scientific Snap!

## Motivation

Graphical programming languages like Scratch, GP, and Snap! have enabled school children and amateurs to explore the world of computer programming while having a lot of fun at the same time. Scratch, the father of Snap!, was designed to help children create fun computer graphics and games and so inherited the "turtle"-based graphics from the grandfather of graphic-capable educational languages, Logo. Snap! took Scratch's graphical interface but implemented a deeper and more powerful underlying computing infrastructure and made it possible to work fully within a browser window, relieving educators from the onerous task of installing software.

Although Snap! is now used at the Univ. of Berkeley to teach undergraduate introductory computer science, most users are caught in the Scratch-trap, thinking that it is only good for creating games, multi-media shows, and computer graphics.  The ease at which complex problems can be solved using a graphical language should be put to use for other educational purposes, e.g. enabling amateur programmers - especially in schools - to learn how scientific problems can be solved.  While the advanced amateur may want to learn how to program in other, more complex and undoubtably more powerful languages like C++ or python, your average middle-school or high school student doesn't have the time or inclination to climb that steep learning curve.

With Snap!, school classes can be enabled to produce their own scientific simulations or process sensor data using standard scientific techniques without the additional baggage of having to learn a complex computer language with a non-intuitive user interface. All Snap! needs, in addition to the standard set of computing tools, are a few more means of easily accessing, processing, and displaying data and additional tools that make Snap! scientific simulations simpler to programme and more powerful in their effect.

The purpose of this git project is to give a home for the collection of such resources as well as to collect examples of how such projects can be done.

E. Modrow and F.V. Hessman (2020-SEP-03)

---

## Installation

You can retrieve the whole package using the usual git methods, but then you'll be downloading all of the example documents and their images as well.  If you are only interested in the blocks and/or Sprites, make your way to where the XML files are listed.  DO NOT try to download using the shown link: it points to a further HTML file, not to the XML file itself.  Press the link and you'll see the beginnings of the XML.  Press the "Raw" button so that only the XML is displayed in your window and save this text as your <tt>\*.xml</tt> file.

---

## Programming Standards

The whole point of using Snap! is that it is powerful (in its own way), easy to learn and easy to programme. Small scripts are easy to read, since the flow of control is shown visually using
- the separation into different scripts (sets of connected blocks)
- the vertical and lateral structure of the connected blocks
- the colours of the blocks and
- the separation into different scripts and Sprites.

However, a complicated and large Snap! script can still be quite a bit to digest.  Both because you will want to be able to understand what the programmes do after a week and because you will want to share them with your friends, colleagues, and/or teacher, you can do several things to make your programmes as understandable as possible - techniques common to all programming languages but with particular quirks in Snap!:
- Keep your scripts small enough to be easily read in one or two glances. If your script is too long, it will be hard to read, hard to debug, and hence hard to maintain.  Long scripts can usually be separated into several smaller scripts working together.
- Avoid repeating sequences of blocks - this is usually a sign that there's an underlying generic function best kept in a separate script.
- Programme using an "object-oriented" point-of-view: keep all of the functionality that doesn't have to be exposed to the whole Snap! universe within a Sprite.  In Snap!, this means remembering that global blocks (those without the "location" icon in front of the block name, like "go to x y") have to be executable by all Sprites and private blocks (those with the "location" icon before the name) can ONLY be executed by that Sprite.  If a Sprite wants to have another Sprite's block executed, it can do so using the various "tell", "run", and "ask" blocks.
- Add comments to blocks and scripts telling the reader what is supposed to be going on.
- When new blocks are created for a Sprite, they appear in the block menu, not on the script working space (and private blocks only appear there if you're looking at the right Sprite's space). It helps to keep an overview of what blocks are associated with a Sprite if you drag the new blocks onto the script working space; this makes it easier to find, edit, and test them.
- Think about what kind of inter-Sprite-communication is best for your project: broadcasts, global blocks, or private blocks called via the "tell", "run", and "ask" mechanism.  Broadcasts are simple and easy to programme, but are sent to everybody.  Using global blocks is really easy, but some functionality is not available.  The "tell", "run", and "ask" mechanisms are the most straight-forward means of letting Sprites talk with each other, but Snap! separates the requested block from the input to that block, making the request rather large and cumbersome-looking.
- Think about what variables need to be global (immediately accessible by all Sprites and scripts), private (simply accessible to a Sprite but less simply by another), or local (a script variable only visible within the script itself).
 
