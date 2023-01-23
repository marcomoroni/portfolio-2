+++
title = "A short investigation on Animal Crossing: New Horizons UI"
slug = "acnh"
template = "portfolio-entry.html"
[extra]
tags = ["UI", "Unity", "Shaders"]
opt_preview_img = ["wobble.gif", "default", 3, 3]
+++

This is a small UI exploration of _Animal Crossing: New Horizons_, more specifically of this bubbly effect and stripe pattern:

{{ image(src="ac.gif") }}

{{ image(src="stripes.jpg") }}

I created the following two shaders.

First, the bubbly effect applied to a sprite, which I achieved by displacing the UVs by a modified sine function:

{{ image(src="wobble.gif") }}

Second, I made the animated stripe effect applied to a circle, where both the stripes and the shape are procedural:

{{ image(src="circle.gif") }}

The circle shape is based on a distance function, but instead of using a floor function to pick the pixels to render, I divided each pixel by the partial derivative of itself. It sounds complex, but it's simply a method to make anti-aliased edges. The pattern is created with a modified and tinted sine wave, and it uses the anti-aliasing method of the circle.