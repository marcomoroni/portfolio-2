+++
title = "Some physics-based animations with particles and rigid bodies"
slug = "pba"
template = "portfolio-entry.html"
[extra]
tags = ["physics", "C++"]
opt_preview_img = ["point.gif", "inverted", 3, 3]
+++

This is a set of physics-based animations I made at university using C++.

{{ article_buttons(buttons=["Source code", "https://github.com/marcomoroni/set09119"]) }}

## Flag

These particles are connected by springs and I applied an isotropic wind to the the triangulated cloth (not to each individual particles).

{{ image(src="flag.gif", stretch=true, can_toggle_full_width=true) }}

## Point gravity

Here you can see a group of particles that are affected by two points of gravity. The gravity, just as you would expect, is stronger the closer to these points and null after a certain set distance.

{{ image(src="point.gif", stretch=true, can_toggle_full_width=true) }}

## Newton's gravity between any two bodies

While the previous simulationunses an approximate gravitational formula, this one uses Newton's law of gravity: every two particles with mass are affected by each other. To be able to see such interactions I decided to make them stick together once they get very close.

The lighter particle has a higher mass.

{{ image(src="newton.gif", stretch=true, can_toggle_full_width=true) }}

## *Super Mario Galaxy*'s gravity

In *Super Mario Galaxy* the player is able to walk in planetoids of any shape and size. This is possible because bodies are affected by the gravity of only one planetoid at once and the gravity direction is the inverse of the normal of (usually) the closest surface.

I've managed to apply this principle to particles in box-shaped planetoids. The gravity direction is the normalised vector from the particle to a point *U*, where *U* is the point on (or in) the planetoid closest to the particle.

{{ image(src="smg.gif", stretch=true, can_toggle_full_width=true) }}

## RigidBody (OBB)

This is a rigidbody with the shape of a box (OBB) colliding with a plane.

{{ image(src="cube.gif", stretch=true, can_toggle_full_width=true) }}

## Collisions between OBBs

This last simulation has two OBBs colliding with each other.

{{ image(src="domino.gif", stretch=true, can_toggle_full_width=true) }}
