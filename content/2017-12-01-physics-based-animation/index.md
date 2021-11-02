+++
title = "Some physics-based animations with particles and rigid bodies"
slug = "pba"
template = "portfolio-entry.html"
[extra]
tags = ["physics", "C++"]
opt_preview_img = ["point.gif", "inverted", 3, 3]
+++

This is a set of physics-based animations I made at university in C++.

{{ article_buttons(buttons=["Source code", "https://github.com/marcomoroni/set09119"]) }}

## Flag

The particles are connected by springs and there's an isotropic wind applied to the the triangulated cloth (not to each individual particle).

{{ image(src="flag.gif", stretch=true, can_toggle_full_width=true) }}

## Point gravity

A group of particles affected by two points of gravity.

{{ image(src="point.gif", stretch=true, can_toggle_full_width=true) }}

## Newton's gravity between any two bodies

While the previous simulation uses an approximate gravitational formula, this one uses Newton's law of gravity: every two particles with mass are affected by each other. To be able to see such interactions I made them stick together once they get very close.

The lighter particle has a higher mass.

{{ image(src="newton.gif", stretch=true, can_toggle_full_width=true) }}

## *Super Mario Galaxy*'s gravity

In *Super Mario Galaxy* the player is able to walk in planetoids of any shape and size. This is possible because bodies are affected by the gravity of only one planetoid at once and the gravity direction is the inverse of the normal of (usually) the closest surface.

I applied this principle to particles in box-shaped planetoids. The gravity direction is the normalised vector from the particle to a point *U*, where *U* is the point on — or in — the planetoid closest to the particle.

{{ image(src="smg.gif", stretch=true, can_toggle_full_width=true) }}

## RigidBody (OBB)

A rigidbody with the shape of a box (OBB) colliding with a plane.

{{ image(src="cube.gif", stretch=true, can_toggle_full_width=true) }}

## Collisions between OBBs

Two OBBs colliding with each other.

{{ image(src="domino.gif", stretch=true, can_toggle_full_width=true) }}
