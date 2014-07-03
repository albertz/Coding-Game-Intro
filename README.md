
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
That's what most games use, and that's also what we mostly use here.
Python is of course also a very good starting language.
But this tutorial here is not about a programming language comparison.
You will find many such comparisons via Google.
And many people also have different opinions about it.


# Some simple game ideas

* 2D side-based action jump-n-run / shooter game.
Remember [Commander Keen](http://en.wikipedia.org/wiki/Commander_Keen)?

* 2D top-down action / shooter / puzzle game. Like [my Robot](http://www.az2000.de/projects/robot2/), [original Robot](http://www.game-of-robot.de/robot2.htm), [Zelda](http://en.wikipedia.org/wiki/The_Legend_of_Zelda), [GTA 2](http://en.wikipedia.org/wiki/Grand_Theft_Auto_2).

* Some sort of [Snake](http://en.wikipedia.org/wiki/Snake_(video_game)).

* Some other simple puzzle game. Like [2048](http://gabrielecirulli.github.io/2048/), [Minesweeper](http://en.wikipedia.org/wiki/Minesweeper_(video_game)), etc.

* Some other arcade game.


# Useful libraries

C++ comes with its own standard template library (STL). And you can use all of the C library.
However, that only covers some standard structures (string, list, map, set, ...), file IO, and some more.
Then, your OS usually comes with its own libraries, for doing anything more complex, like writing GUIs, graphics, sounds, etc.
The OS libraries are usually OS dependent and Windows, Linux and MacOSX differ a lot from each other.
If you want your game to be runable many different systems, there are many cross-platform libraries which you can use.
Just avoid using anything from the OS libraries directly and use some cross-platform library instead to do graphics, sounds, networking, etc.

Here are some useful ones:

* [SDL](https://www.libsdl.org/). Very simple, has a lot of functionality, and supports many many platforms.
* [GLFW](http://www.glfw.org/). Mostly for OpenGL.


# Existing bigger sized games

* [OpenLieroX](http://openlierox.net), my own game. 2D side-based shooter.
[Read here for more.](http://www.openlierox.net/wiki/index.php/Learning_to_code)
And then, [this](http://www.openlierox.net/wiki/index.php/Contribute_to_the_source_code) is probably a good guideline.
[Here is the source code on GitHub.](https://github.com/albertz/openlierox)

* [SafeTheRock](https://sourceforge.net/projects/savetherock/).
[Source code on GitHub](https://github.com/albertz/SaveTheRock).
