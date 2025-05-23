
# Description

This is somewhat a coding tutorial / introduction.
The best way to learn to code is of course just to actually code.
The most fun way to start coding is by writing small little games.

This repository contains various resources for doing exactly that.
(It's mostly a work-in-progress at the moment. Just look around what's already there. It might already be helpful.)

Coding games actually covers a lot of topics, like AI, cross-platform, low-level, graphics, audio, networking, and more.
[Read here why game development is a great learning playground.](http://www.openlierox.net/wiki/index.php/Why_game_development_is_a_great_learning_playground)

With some little coding knowledge, it also makes sense to take existing Open Source games as a base.
You can either join their team, or just take the code and extend it for yourself.
In any case, the project team people will most likely be very happy to introduce you to their code and help you to extend it by some fun idea of you.


# Programming language

The programming language doesn't really matter that much.
Don't be scared about C++. It isn't really that complicated.
Or maybe Rust, or Nim, or some of the other newer native languages.
Python is of course also a very good starting language.
But this tutorial here is not about a programming language comparison.
You will find many such comparisons via Google.
And many people also have different opinions about it.


# Some simple game ideas

* 2D side-based action jump-n-run / shooter game.
Remember [Commander Keen](http://en.wikipedia.org/wiki/Commander_Keen)?
* 2D top-down action / shooter / puzzle game.
Like [my Robot](http://www.az2000.de/projects/robot2/),
[original Robot](http://www.game-of-robot.de/robot2.htm),
[Zelda](http://en.wikipedia.org/wiki/The_Legend_of_Zelda),
[GTA 2](http://en.wikipedia.org/wiki/Grand_Theft_Auto_2).
* Some sort of [Snake](http://en.wikipedia.org/wiki/Snake_(video_game)).
* Some other simple puzzle / arcade game.
Like [2048](http://gabrielecirulli.github.io/2048/),
[Minesweeper](http://en.wikipedia.org/wiki/Minesweeper_(video_game)),
[Frozen Bubble](http://www.frozen-bubble.org/),
[Tetris](http://en.wikipedia.org/wiki/Tetris)
etc.
* Some card game.
* Some turn-based game.


# Useful libraries

C++ comes with its own standard template library (STL). And you can use all of the C library.
However, that only covers some standard structures (string, list, map, set, ...), file IO, and some more.
Then, your OS usually comes with its own libraries, for doing anything more complex, like writing GUIs, graphics, sounds, etc.
The OS libraries are usually OS dependent and Windows, Linux and MacOSX differ a lot from each other.
If you want your game to be runable on many different systems, there are many cross-platform libraries which you can use.
Just avoid using anything from the OS libraries directly and use some cross-platform library instead to do graphics, sounds, networking, etc.

Here are some useful ones, for C++.

* [Raylib](https://www.raylib.com/). Very simple, more recent.
* [SDL](https://www.libsdl.org/).
Very simple, has a lot of functionality, and supports many many platforms.
Somewhat low-level, 2D graphics, OpenGL, sound, input event, GamePad support, etc.
This is the most famous and often used game library.
* [Allegro](https://www.allegro.cc/).
Somewhat like SDL, but a bit less features and a bit less often used.
It's slightly more high level than SDL.
* [GLFW](http://www.glfw.org/), [GLEW](http://glew.sourceforge.net/). Mostly for OpenGL.
* [PhoenixCore](https://github.com/jonparrott/PhoenixCore). 2D OpenGL based drawing library.
* [NanoVG](https://github.com/memononen/nanovg). OpenGL based 2D vector drawing library.
* [skia - 2D Graphics Library](https://code.google.com/p/skia/). [Read also here.](http://www.phoronix.com/scan.php?page=news_item&px=OTM0Mw)
* [Troll2D](https://code.google.com/p/troll2d/) (2008). Simple 2D game engine.
* [SFML](http://sfml-dev.org/). Multimedia library, system, window, 2D graphics, audio, network. [SFGUI](http://sfgui.sfml-dev.de/) or [TGUI](https://tgui.eu/) for GUI.
* [Fast Light Toolkit (FLTK)](http://www.fltk.org/). Comes with many GUI widgets.
* [librocket](http://librocket.com/)
* [Picasso graphic](https://code.google.com/p/picasso-graphic/) (2013)
* [Polycode](http://polycode.org/). OpenGL, with Lua scripting.
* [Angel2D](http://angel2d.com/). Big and powerful. Maybe overkill.
* [Torque2D](http://www.garagegames.com/products/torque-2d). Big and powerful. Maybe overkill.
* [Godot Engine](http://www.godotengine.org/). Maybe overkill.
* Unity or Unreal are the big commercial ones. Maybe overkill. Also not fully open source licences.
* [Ogre](http://www.ogre3d.org/). 3D graphics rendering engine. Probably overkill for the beginning.
* [Proton SDK](http://www.rtsoft.com/wiki/doku.php?id=proton). Might be overkill.
* [Rainbow](https://bitbucket.org/tido/rainbow). Might be overkill.
* [ClanLib SDK](http://www.clanlib.org/). OpenGL, GUI framework, network engine, physics, etc. Might be overkill.
* [openFrameworks](https://openframeworks.cc/)
* [bgfx](https://github.com/bkaradzic/bgfx). Cross-platform rendering library (3D graphics).
* [Slang Shader Language](https://shader-slang.org/)
* [Lua](http://lua.org). Most famous embedded scripting language, very often used in games. Also very fast.
* [Box2D](http://box2d.org/). 2D physics engine.
* [OpenAL](http://en.wikipedia.org/wiki/OpenAL). For 3D sound.
* [Gameplay3D](http://www.gameplay3d.org/), full framework.
* [Qt](http://qt-project.org/).
This is more for standard GUI application development, not so much for games.
You probably don't need/want that for a game.
However, in the application development world, this is probably the most important library.
* [EntityX](https://github.com/alecthomas/entityx).
Fast, type-safe C++ Entity Component System.
Article '[Evolve Your Hierarchy](http://cowboyprogramming.com/2007/01/05/evolve-your-heirachy/)' covering the theory of Entity Component Systems (ECS).
* [Protogame asset management](http://protogame.org/docs/asset_management.html).
Protogame itself is Mongo-based.
But it has some nice concepts.
* Some GUI frameworks:
[CEGUI](http://cegui.org.uk/) (OpenGL, MIT license),
[MyGUI](http://mygui.info/) (MIT license),
[OtterUI](https://github.com/Twolewis/OtterUI),
[Agar](http://libagar.org/),
[OUI](https://bitbucket.org/duangle/oui-blendish/src),
[Turbo Badger](https://github.com/fruxo/turbobadger),
[blog post summary](http://www.fysx.org/2010/09/13/quest-for-a-gui/),
[IMGUI](http://sol.gfxile.net/imgui/),
[GLIMGUI](https://bitbucket.org/MartinFelis/glimgui),
[GWEN](https://github.com/garrynewman/GWEN),
[Guichan](https://gitorious.org/guichan)

Other relevant non-C++ frameworks:

* [LÖVE](http://love2d.org/).
For Lua.
[Examples](http://www.love2d.org/wiki/Category:Games),
[more examples](https://github.com/miko/Love2d-samples),
[tutorials](http://www.love2d.org/wiki/Category:Tutorials).
Löve itself might be a good base for a C++ framework, too.
There are even [many extension libraries](http://www.love2d.org/wiki/Category:Libraries).
[Here are some supporting dev software.](http://www.love2d.org/wiki/Category:Software)
* [Planimeter's Grid Engine](https://www.planimeter.org/grid-sdk/).
For Lua.
Based on Quakeworld architecture and comes with fully client-side predicted multiplayer
([ref](https://news.ycombinator.com/item?id=28083193)).
* [Pyxel](https://github.com/kitao/pyxel) for Python
* [Pygame](https://www.pygame.org/) for Python.
  Also see [pygame-web](https://pygame-web.github.io/), [pyscroll](https://github.com/bitcraft/pyscroll).
* [Arcade](https://api.arcade.academy/) for Python
* [FNA](https://fna-xna.github.io/). Reimplementation of Microsoft XNA Game Studio 4.0 Refresh


# Existing Open Source games as a good project base

* [OpenLieroX](http://openlierox.net), my own game. 2D side-based shooter.
[Read here for more.](http://www.openlierox.net/wiki/index.php/Learning_to_code)
And then, [this](http://www.openlierox.net/wiki/index.php/Contribute_to_the_source_code) is probably a good guideline.
[Here is the source code on GitHub.](https://github.com/albertz/openlierox)
* [Commander Genius](http://clonekeenplus.sourceforge.net/). Commander Keen compatible clone, i.e. 2D side-based jump-n-run.
* [SafeTheRock](https://sourceforge.net/projects/savetherock/).
[Source code on GitHub](https://github.com/albertz/SaveTheRock).
* [Teeworlds](https://www.teeworlds.com/). 2D side-based shooter, similar to OpenLieroX but aiming is with mouse.
* [Secret Maryo](http://secretmaryo.org/) and [SuperTux](http://supertux.lethargik.org/). 2D jump-n-runs. Mario.
* [Mari0](http://stabyourself.net/mari0/). 2D jump-n-run. Mario + Portal.
* [ASCIIpOrtal](https://github.com/cymonsgames/ASCIIpOrtal). 2D side-based jump-n-run puzzle game. Portal.
* [Enigma](http://www.nongnu.org/enigma/). Puzzle game.
* [Craft](https://github.com/fogleman/Craft). Minecraft clone. Simple and small C code base.
* [zSILENCER](http://zsilencer.com/)
* [OpenClonk](http://www.openclonk.org/)
* [Mr. Rescue](http://tangramgames.dk/games/mrrescue/)
* [The Battle for Wesnoth](http://www.wesnoth.org/). 2D turn-based strategy game. Long development history. Quite complex now.
* [Xonotic](http://xonotic.org/) (earlier Nexuiz). 3D FPS. Big project, so you should bring at least medium experience already, but still, developing a new game mode or so might not be too hard.
* [Destination Sol](https://sourceforge.net/projects/destinationsol/)
* [space-shooter.c](https://github.com/tsherif/space-shooter.c). simple and pure C. also see [its architecture](https://github.com/tsherif/space-shooter.c/blob/master/ARCHITECTURE.md)
* [pacman.c](https://github.com/floooh/pacman.c)

See also these lists:

* [Wikipedia](http://en.wikipedia.org/wiki/List_of_open-source_video_games)
* [LGDB](http://www.lgdb.org/games?sort_by=created&taxonomy_vocabulary_3_tid=All&taxonomy_vocabulary_5_tid=All&taxonomy_vocabulary_7_tid=All&taxonomy_vocabulary_6_tid=All&taxonomy_vocabulary_14_tid=All&taxonomy_vocabulary_9_tid=All&taxonomy_vocabulary_34_tid=All&taxonomy_vocabulary_16_tid=87&taxonomy_vocabulary_12_tid=39)
* [Free Gamer](http://freegamer.blogspot.de/)
* [Libre game wiki](https://libregamewiki.org/List_of_games)
* [freegamedev](http://freegamedev.net/wiki/Complete_open_source_games)


# Assets / artwork / graphics / sounds for your game

You can create your own graphics and sounds.
Some useful tools:

* [sfxr](http://www.drpetter.se/project_sfxr.html) for creating sounds.
[bfxr (Web version)](http://www.bfxr.net/).
* [SunVox](http://www.warmplace.ru/soft/sunvox/) for sound
* [LMMS](http://lmms.sourceforge.net/) for creating music.
* [SoundHelix](http://www.soundhelix.com/) for algorithmic random music.
* [Gimp](http://www.gimp.org/) for graphics. Might be too powerful, though, because most likely, you just want to create pixel graphics.
* [GrafX2](http://pulkomandy.tk/projects/GrafX2) ([old homepage](https://code.google.com/p/grafx2/)), bitmap paint program
* [Pixel](http://www.kanzelsberger.com/pixel/) image editor
* [MyPaint](http://mypaint.intilinux.com/) graphics application
* [Pinta](http://pinta-project.com/), drawing/editing program modeled after [Paint.NET](http://getpaint.net/).
* [Aseprite](http://www.aseprite.org/) ([GitHub](https://github.com/aseprite/aseprite)),
animated sprite editor & pixel art tool.
Seems to have become comercial now.
* [Tiled map editor](http://www.mapeditor.org/)
* [Tile studio](http://tilestudio.sourceforge.net/)
* [Toast Editor](http://toastedware.com/?page_id=190), web-based level editor
* [Overview for Pixel Art Programs](http://forums.gnomoria.com/index.php?topic=4508.0)
* [2D game art for programmers blog](http://2dgameartforprogrammers.blogspot.de/)
 
There are some useful existing resources you can use:

* [OpenGameArt.org](http://opengameart.org/).
[And this.](http://lpc.opengameart.org/)
[See also.](https://news.ycombinator.com/item?id=7890901)
[Nice one](http://opengameart.org/content/castle-tiles-for-rpgs),
[some more](http://forums.themanaworld.org/viewtopic.php?f=8&t=14884&sid=4695e444f4bc4cb59fccc765dc79f68f&start=75).
* [Freesound.org](http://www.freesound.org/)
* [Glitch the game](http://www.glitchthegame.com/public-domain-game-art/)
* [Oddball's small offerings](http://forums.tigsource.com/index.php?topic=8834.05). Font, characters, tiles, items.


# Other tutorials

* [Coding for absolute dummies (in German) (by me)](http://www.az2000.de/docs/coding_for_dummies/), tries to explain the very basics of programming, the idea of an algorithm and such
* [Trivial C++ console catch-me game (in German) (by me)](http://www.az2000.de/projects/cpp_tut/). You develop a very simple catch-me-if-you-can C++ console sort-of game step by step.
* [40 game development tutorial overview](http://gamedevelopment.tutsplus.com/articles/40-fantastic-game-development-tutorials-from-across-the-web--gamedev-3384)
* [Game Programming in C and C++](http://www.cprogramming.com/game-programming.html)
* [SDL / Game Programming tutorial](http://lazyfoo.net/tutorials/SDL/index.php)
* [OpenGL Programming Wikibooks](http://en.wikibooks.org/wiki/OpenGL_Programming)
* [OpenGL / Game programming tutorials](http://nehe.gamedev.net/)
* [OpenGL tutorial](http://www3.ntu.edu.sg/home/ehchua/programming/opengl/CG_Introduction.html)
* [Aron's SDL tutorials](http://aaroncox.net/tutorials/arcade/index.html)
* [GameDevGeek](http://gamedevgeek.com/tutorials/)
* [Game from scratch in C++ and SFML](http://www.gamefromscratch.com/page/Game-From-Scratch-CPP-Edition.aspx)
* [What every programmer needs to know about networking](http://gafferongames.com/networking-for-game-programmers/what-every-programmer-needs-to-know-about-game-networking/), [The Quake3 network model](http://fabiensanglard.net/quake3/network.php), [The Unreal networking architecture](http://udn.epicgames.com/Three/NetworkingOverview.html)
* [Handmade Hero](https://handmadehero.org/). Screen recordings of the full development of a game, over 600 days.


# Forums / Other references

* [my wiki on coding in general](https://github.com/albertz/wiki/blob/master/coding.md)
* [TIGForums](http://forums.tigsource.com/)
* [gamedev.net](http://www.gamedev.net/page/index.html)
* [Game Programming Wiki](http://www.gpwiki.org/)


# Game coding competitions

There are a few game coding competitions, where you have to code a full small game in a very short time, like 24 hours, or 72 hours, or maybe a week.

* [Ludum Dare](http://www.ludumdare.com/compo). This is probably the most famous competition. The creator of Minecraft, alias Notch, as often take part here.
* [more on Wikipedia](http://en.wikipedia.org/wiki/Game_jam)
* [How to get the most out of a Game Jam](http://gamedevelopment.tutsplus.com/articles/how-to-get-the-most-out-of-a-game-jam--gamedev-437)

Some developers, such as Notch, sometimes make their coding screencast publicly available. This is often very entertaining and rewarding to watch. You will most probably learn a lot. And you will see how other developers are developing a small game in a short time.

* Notch (Minecraft dev):
[Twitch](http://www.twitch.tv/notch),
[YouTube](https://www.youtube.com/results?search_query=notch+coding),
[Twitter](https://twitter.com/notch)

Many developers write some post mortem about their development during such competition.
This is interesting because it shows you what tools to use to develop a fun game in a short time period.

* [Ludum Dare 27, 10corp](http://www.ludumdare.com/compo/2013/08/26/postmortem-10corp/).
C++11, SFML, [custom framework SSV](https://github.com/SuperV1234?tab=repositories).
* [Ludum Dare 29, N.A.M.E.](http://www.ludumdare.com/compo/2014/05/18/n-a-m-e-a-very-late-post-mortem/).
C++11, SFML. [Code on GitHub](https://github.com/ace13/LD29).
* [Ludum Dare 28, BlockDodger](http://jibransyed.wordpress.com/2013/12/16/blockdodger-my-second-ludum-dare-post-mortem/).
C++, SDL, OpenGL, GLEW, GLM, FreeImage.
* [Ludum Dare 28, incomplete source on GitHub](https://github.com/hovatterz/Ludum-Dare-28).
C++, Lua, EntityX.

