+++
title = "Impossible shapes made using OpenGL inspired by Monument Valley"
slug = "mv"
template = "portfolio-entry.html"
[extra]
tags = ["graphics", "C++"]
opt_preview_img = ["screen07.png", "inverted", 5, 1]
+++

{{ image(src="animated.gif", stretch=true, full_width=true, can_toggle_full_width=true) }}

This is a coursework I've made for a Computer Graphics module. I used [OpenGL](https://www.opengl.org/) to recreate a scene that looked like a level from the game *[Monument Valley](https://www.monumentvalleygame.com/)*:

{{ image(src="mv_screen.jpg", tall=true) }}

You've probably noticed the impossible geometries: I made them by using a camera with an orthographical projection, therefore you can't perceive depth.

I used three directional lights facing the three visible surfaces. In this way I have a higher control of the colours I want my scene to have.

The Phong shader had to be used without the reflection component because reflection is affected by the distance from the camera. Using it would break the illusion of impossible geometries.

To create the water waves that you can see on the left cube I multiplied two identical normal maps moving in different directions.

Finally, I worked with frames to allow multiple ones to work at the same time: I can have multiple post-processing effects, such as vignette and inverse colours.

{{ article_buttons(buttons=["Source code", "https://github.com/MarcoMoroni/CG_cw2", "Report", "https://github.com/MarcoMoroni/CG_cw2/blob/master/Report/report.pdf"]) }}

{{ image(src="screen04.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="screen06.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="screen05.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="screen02.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="screen07.png", stretch=true, can_toggle_full_width=true) }}
