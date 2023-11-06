+++
title = "I'd like to go home"
slug = "idliketogohome"
template = "portfolio-entry.html"
[extra]
tags = ["Game Jam", "Unity", "C#"]
opt_preview_img = ["h1.png", "default", 2, 4]
+++

{{ image(src="h1.png", stretch=true, full_width=true, can_toggle_full_width=true) }}

{{ image(src="h2.png", stretch=true, full_width=true, can_toggle_full_width=true) }}

{{ image(src="h3.png", stretch=true, full_width=true, can_toggle_full_width=true) }}

I made *I'd like to go home* during the [Global Game Jam](https://globalgamejam.org/) 2019, where you have create a game in 48 hours.

{{ article_buttons(buttons=["Play it", "https://marcomoroni.itch.io/id-like-to-go-home", "Playthrough (3:01)", "https://youtu.be/kFk0DDlWAJY", "Source code", "https://github.com/marcomoroni/ggj-2019"]) }}

This year I decided to go all solo: I drew the assets and I used Unity to build it. It's made with 2D sprites in a 3D side-scrolling scene.

It's a short story about a rabbit that lost his way home. My attention was all on the immersion of the player and the art-style was inspired by [Jon Klassen](http://jonklassen.tumblr.com/) — for the characters and the story — and [Gal Shir](https://galshir.com/) — for the colours and the vegetation.

Some technical insights:
* The background seems to be of one solid dark purple: the 3D plane on the ground has a monochrome unlit shader so that you cannot see where the floor ends.
* The camera is controlled by Unity's Cinemachine and it has a noise and vignette post-processing effect.
* The sprites are generally made in two steps: first, basic shape with a solid colour; second, a dithered layer to add a secondary colour.
* There is what seems to be a 3D model of a home: at the time of writing I don't know how to 3D model, so I simply assembled it with some sprites (*hehe*).