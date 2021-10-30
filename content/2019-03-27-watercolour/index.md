+++
title = "Procedurally generated watercolour textures"
slug = "watercolour"
template = "portfolio-entry.html"
[extra]
tags = ["procedural generation"]
opt_preview_img = ["textures.gif", "default", 3, 3]
+++

{{ image(src="textures.gif", stretch=true) }}

While working on my Honours Project I discovered the wonders of procedural generation, and here I had another go at it with procedural watercolour textures. I found a couple of ways to do it: one is from [Tyler Hobbs](https://tylerxhobbs.com/essays/2017/a-generative-approach-to-simulating-watercolor-paints), in which a shape is deformed multiple times, and the other is from [this Reddit post](https://www.reddit.com/r/proceduralgeneration/comments/6mta0f/watercolor_simple_noise_algorithm/). I tried the latter: the algorithm recursively expands a small image (here 3 &#215; 3 pixels) by adding a new pixel between the existing ones, and their colour is chosen through a linear interpolation between the neighbouring ones.

The implementation is in [Processing](https://processing.org/) (Java — *ew*).
