+++
title = "Azucena: a game built on a custom C++ engine"
slug = "azucena"
template = "portfolio-entry.html"
[extra]
tags = ["graphics", "physics", "C++"]
opt_preview_img = ["capture_02.png", "default", 2, 4]
+++

*Azucena* has been my first complete game! I made this game as a university coursework, and the project included a pitch presentation and a game design document.

I took inspiration mainly from two games: *The Legend of Zelda* and *Hyper Light Drifter*. You play as Azucena, a llama who has to rescue her three babies. Each of them is waiting at the end of a level and the levels can be visited in any order.

{{ image(src="capture_01.png", stretch=true, full_width=true, can_toggle_full_width=true) }}

It runs on an engine built from scratch in C++, with the help of [SFML](https://www.sfml-dev.org/) and [Box2D](https://github.com/erincatto/Box2D). The pieces are the same you would expect to find in any game engine: scenes, entities, components, etc. The game has all the basic technical features necessary to consider a game *a game*, for example: a menu, save and load, a tutorial, an ending, sounds and music, support for different screen resolutions, remappable controls and joystick support.

Before this project, I used to use Unity for very simple tasks, without having a deep understanding of the engine and its potential. But after completing it I saw the light! This small game was a turning point because it made game engine architectures very clear for me.

{{ article_buttons(buttons=["Website & download", "https://marcomoroni.github.io/azucena/", "Source code", "https://github.com/marcomoroni/azucena"]) }}

{{ image(src="capture_04.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="capture_02.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="capture_03.png", stretch=true, can_toggle_full_width=true) }}