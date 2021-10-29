+++
title = "A generator of cities following the style of Minna O."
slug = "cities"
template = "portfolio-entry.html"
[extra]
tags = ["procedural generation", "Unity", "C#"]
opt_preview_img = ["ortho-02.png", "inverted", 4, 2]
+++

This was the Honours Project for my degree in Games Development at Edinburgh Napier University. I studied and classified the different procedural content generation (PCG) techniques and used them to create cities similar to the ones drawn by [Minna O.](https://nokkasili.tumblr.com/):

{{ image(src="minna02.jpg", stretch=true) }}
{{ image(src="minna03.jpg", stretch=true) }}
{{ image(src="minna04.jpg", stretch=true) }}
{{ image(src="minna05.jpg", stretch=true) }}

The following are screenshots of the generated artefacts (made in Unity — they are 3D and interactive). I was extremely lucky to have Minna helping me throughout the project — she made all the assets I needed!

{{ image(src="perspective-01.png", stretch=true, full_width=true) }}
{{ image(src="perspective-03.png", stretch=true, full_width=true) }}

And a 2D one (with an orthographic projection):

{{ image(src="ortho-01.png", stretch=true, full_width=true) }}

Needless to say, the final result is way more limited than initially imagined, but I'm extremely happy with what I've learnt. Procedural art is really fascinating!

{{ article_button(text="Try the generator", href="https://marcomoroni.itch.io/architect") }}

If you'd like to learn more about how I did it, keep reading!

## Classification

PCG techniques can be divided in two categories:

* additive techniques, where the artefacts are created: goblins and treasures are placed in a map, the loot of a chest is created, etc.;
* substractive techniques, where the artefacts are filtered: the generator (or sometimes a human) needs to evaluate what has been produced and pick the correct or best ones.

For this project I ended up using only additive techniques. Here's a short summary of the most used additive PCG algorithms:

* Tiles: As the name suggests, when you have a bunch of equally sized tiles you can place them by following certain rules.
* Grammars: These techniques usually consist on a set of rewriting rules. For example, if I have a rule such as *A &#8594; AB* (*A* will transform into *AB*), I can iteratively expand a string *A* in *AAB*, *ABABB*, *ABBABBB*, etc. This is called an L-system, and it was initially developed to describe how plants look. Fractals are also a type of grammar.
* Distribution: Let's say you need to populate a map with trees, and you want them to be at a certain distance from each other, or you need to cluster them more tightly in certain areas. You can use distribution techniques, which give you more control over randomness.
* Parametric: Not really an algorithm by itself, it usually refers to generators that can be controlled through parameters.
* Interpretative: noise (usually Perlin noise) can be interpreted as a height map, which can then be used to create a terrain mesh.
* Simulations: Involve usually advanced algorithms like neural networks and evolutionary ones, which are out of the scope of this project.

## Techniques used

For every category I identified its strengths and weaknesses, and then picked the ones that better suited what I wanted to achieve.
...

## Other things I've learnt but didn't use

...

## Academic poster

{{ image(src="poster_front.png") }}
{{ image(src="poster_back.png") }}