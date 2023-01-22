+++
title = "A driving simulator for traffic officers training"
slug = "driving_sim"
template = "portfolio-entry.html"
[extra]
tags = ["UX", "UI", "Unity", "C#"]
+++

On one side we have a traffic officer trainee with a VR headset sitting in a car-like rig which can simulate the movements and rumbles of a real one; on the other side an instructor using a connected PC with which they can manipulate the virtual environment to create custom scenarios with car accidents, high traffic, etc.

The design process covered hardware, software and the user experience as a whole. I'll focus on key parts of the mock-ups I created, and then implemented in Unity with UI Toolkit. UI Toolkit is like HTML and CSS adapted for use in a game engine.

Once connected, this is the dashboard the instructor is presented with:

{{ image(src="instructor_dashboard_frame.png", full_width=true, can_toggle_full_width=true) }}

This is the semantic structure:

{{ image(src="semantic_structure.png", can_toggle_full_width=true) }}

A few notes on the design:

* At a glance, your attention is not drawn anywhere (except perhaps the scene view): there are no primary actions and for this reason no buttons or other elements have a prominent style.
* I don't use an accent colour, but contrast instead. I'm not fond of accent colours in unbranded UIs — this makes designs more challenging but arguably more aesthetically pleasing.
* The typeface is Inter, which is pretty standard nowadays.
* All icons are custom made.
* It's minimalist but ergonomic.
* There's much though behind the 'Change map' button: it also serves as way to start, end and reset a 'session'.
* I'm still a programmer! This means I know the tools and the limitations available, and the mock-ups are always assured to be achievable.

Here are some other pieces:

{{ image(src="edit_gantry.png", can_toggle_full_width=true) }}

{{ image(src="second_monitor.png", can_toggle_full_width=true) }}

{{ image(src="details_add_button.png", can_toggle_full_width=true) }}

{{ image(src="details_mini_map.png", can_toggle_full_width=true) }}

{{ image(src="details_road_rendering.png", can_toggle_full_width=true) }}
