+++
title = "Jurassic World Aftermath"
slug = "jw"
template = "portfolio-entry.html"
[extra]
tags = ["published", "XR", "UI", "Unity", "C#"]
opt_preview_img = ["jw.jpg", "default", 2, 4]
+++

{{ image(src="jw.jpg") }}

The first commercial project I worked on while at [Coatsink](https://coatsink.com/).

_[Jurassic World Aftermath](https://www.oculus.com/jurassic-world-aftermath/)_ is a VR game built in Unity. I touched many parts, such as the UI, the progression system and the minigames scattered around the world.

The project bravely tried to use Unity's — as of time of writing — experimental Data Oriented Technology Stack (DOTS), which introduced me for the first time to data-oriented programming.

DOTS takes C# and attempts to mold it into a data-oriented, garbage-collector-free sub-language, which ideally allows for more performant games. Authoring and runtime would now be split in two different parts, and runtime code would use an entity-component-system architecture instead of the classic `GameObject`s. Whether this will eventually work well for Unity or not going forward I can't say for sure, but it's definitely not there yet. What's sure is that I've learned a lot about memory management and the impact of good (or bad) APIs.

Working for the first time in such a big team made me change some bad habits I realised I had before, so here's some wisdom from a junior programmer: don't over-engineer it; don't commit code thinking you'll have time to go back to it later — make it good the first time; always keep in mind your code is going to be read by someone else — don't wait to add comments; designers (or clients) don't always know what they want — poke them until all is clear; don't skip pre-production.

I was very lucky to work on this as my first somewhat important project, and maybe even more to have had such nice co-workers <3.
