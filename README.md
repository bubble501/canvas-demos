Canvas Demos
============
The purpose of this project is to create the same application using different HTML5 Canvas
frameworks. The Maze demo is based on, and uses assets and code from Blockly's Maze:
    https://blockly-demo.appspot.com/static/apps/maze/index.html

*You can compare 'demo.js' and 'pegman.js' for each of the projects to see the differences for yourself.*

Impelementation exists for the following frameworks:
* PhaserJS (game engine, uses Pixi for rendering) - http://phaser.io
* KineticJS (for interactive web graphics) - http://kineticjs.com

(incomplete; not suitable or hard to use for this demo)
* PixiJS (rendering engine; 2D WebGL+Canvas) - http://www.pixijs.com
* PandaJS (game engine) - http://www.pandajs.net

(not yet implemented)
* EaselJS
* FabricJS

### Other evaluations and comparisons:
* The following StackOverflow link has an evaluation of FabricJS and KineticJS:
  http://stackoverflow.com/questions/8938969/current-state-of-javascript-canvas-libraries
* Another comparison between EaselJS, FabricJS, PaperJS, PixiJS:
  https://groups.google.com/forum/#!topic/flashcodersny/rU0-3zD7QIo
* http://www.softr.li/blog/2012/06/20/which-html5-canvas-javascript-library-should-i-use

The application uses the following features:
* Images & Sprites
* Animation & Transitions/Tweens

The application does not USE any of:
* Drag-n-drop
* Collision detection
* Mouse & Keyboard events
* Physics

PhaserJS - game engine
======================
Phaser JS is a game engine build on top of Pixi JS.
* Tutorials - impressive collection of tutorials
  - http://examples.phaser.io - great set of examples / tutorials
  - http://www.photonstorm.com/phaser/tutorial-making-your-first-phaser-game
  - http://gamemechanicexplorer.com
  - http://discoverphaser.com (book)
* Documentation - rich set of guides
  - http://phaser.io/getting-started-js.php
  - http://docs.phaser.io/

### Pros
* Great documentation; lots of well organized examples.
* Phaser.js IS a game development framework and as such, it makes it very easy to work with
  Sprites, Animations, Transitions.
* Very simple to start with and allows you to create a full game within ~100 lines of code.
* Has several physics engines.


Kinetic JS - for interactive web graphics
=========================================
* Tutorials - a handful of basic tutorials exist. However, I find Google & StackOverflow
  to be a lot more useful.
* Documentation - documentation for the API exists. However, the documentation is missing
  basic examples.
* User base & StackOverflow - it seems that there is a large user base and a lot of questions
  are covered and answered in StackOverflow.

### Pros
* Easy and simple to use.
* Has a number of basic shapes; supports 
* The "Tween" API is very nice and easy to use, and includes a number of Easings.

### Cons
* It would be useful to have a generic image/assets loader, even though it is easy to copy the
  image loader from the examples/tutorials.
* The Sprite animation API is somewhat limited and does not have options not to loop
  animations; there are also no events when the animation ends, so you have to manually manage 
  transitions, based on the current frameIndex.
* Not able to flip sprite animations.
* It is NOT a game engine and as such not suitable for complex games.
  Can be used to implement simple board games or similar.


Panda JS - game engine
======================
Panda JS is another game engine build on top of Pixi JS.
* Tutorials - very limited
  - http://www.emanueleferonato.com/2014/03/05/look-at-panda-js-html5-game-engine-capabilities-with-a-working-game-prototype/
* Small snippet of code showing differences between Phaser and Panda JS
  - http://www.pandajs.net/snippets/9719395.html

### Pros
* Encourages good object-oriented design and implementation

### Cons
* Documentation is not very detailed; doesn't have a lot of examples nor tutorials.
* Hard to figure out; doesn't provide a minified js file, which makes it hard to 'install' and use.
* Seems to be designed for standalone HTML5 games.


Pixi JS - rendering engine
==========================
It seems that Pixi is designed as a fast and efficient rendering engine. It can be used for serious
game development but it is NOT a game engine. Pixi is encouraging developers to
extend existing basic classes, such as Sprite and TilingSprite, as a way to add new functionality.
Other frameworks are designed to use their shapes and constructs to assemble and compose a scene.

It is not suitable to use Pixi JS for this demo, beucase Pixi is pretty low level for the purpose of
the maze app. However, a number of game engines are built on top of Pixi which are used to implement
this demo project.

Tutorials:
- Building a Parallax Scroller with Pixi.js: Part 1
    http://www.yeahbutisitflash.com/?p=5226

### Pros
* Provides an asset loader; encourages use of TexturePacker (http://www.codeandweb.com/texturepacker).
* It has a nice support for Spine (http://esotericsoftware.com/spine-in-depth).

### Cons
* Unless using Spine, it does not provide an easy to use animations support. People usually extend
  Sprite or MovieClip to implement their own animation functionality.

#### Useful Comments / Links
* Tweening - http://www.html5gamedevs.com/topic/938-tweening/
* See QA - http://www.html5gamedevs.com/topic/2393-creating-an-object-with-multiple-animations-in-pixijs/



Additional Resources
====================
* http://www.html5gamedevs.com
* http://cdnjs.com
* http://physicsjs.challengepost.com

