+++
title = "Free-to-roam visual and audible immersive experience of one of the world’s most important World Heritage sites"
slug = "mxt_vr"
template = "portfolio-entry.html"
[extra]
tags = ["XR", "UI / UX", "Unreal Engine"]
opt_preview_img = ["a303_mockup_narration.png", "inverted", 5, 2]
+++

The largest project I worked on while at [MXT](https://mxt.co.uk/) was a simulation of what the area around of one of the world’s most important World Heritage sites would look like before and after a very important project (which I can't reveal yet). Our job was to show the striking difference between the present and the future to users that may have no experience with VR at all.

Please note that the details I can provided are limited at this point in time.

The simulation uses real-world data to build realistic traffic and noise that would come with it. We decided to use Unreal Engine even though none of us had experience with it.

The UI has been carefully designed to fit two seemingly contradictory gameplay flows: a guided tour and free roaming. Despite the challenge, the UI has always been praised during our user testings.

UI was fully on me, from design to implementation. What would a user with potentially no computer skills see once the headset is on?

## Mock-ups

Much has changed since the initial mock-ups but some cardinal ideas persisted: your left hand would function as a tablet-like interface, while the right as a laser to point and select interactive elements; keep diegetic UI to a minimum; the user should never feel lost or confused on what to do next.

{{ image(src="a303_mockup_lh.png", can_toggle_full_width=true) }}
{{ image(src="a303_mockup_minimap.png", can_toggle_full_width=true) }}
{{ image(src="a303_mockup_narration.png", can_toggle_full_width=true) }}

## Implementation

First time using Unreal Engine — exciting!

Implementation was for the most part what you would expect from a gameplay programmer, except for a few interesting aspects.

UI needs _shapes_, like rectangles with rounded corners. I made a lot of shader-based shapes using a technique called raymarching distance field. This method makes shapes that are much more visually pleasing than sprites, because no matter how close you are, edges are always crisp and you won't see any pixel. It's easier to edit colours and sizes at runtime!

{{ image(src="tablet.png", can_toggle_full_width=true) }}

## An idea I had too late

Whenever possible, I want to avoid explicit tutorials, especially with text. Users never read text. Unfortunately, I didn't find a satisfactory way to be fully clear of them, but the final implementation still has a simple and gradual introduction to the different gameplay features. One aspect that went through many iterations was how to have the user discover the controls on the two hands (raise them to the correct position so that they can be seen) and teach how to use them (move the laser to point to an element and select it).

Too late in development I came up with an idea that I'd love to explore further: how about a *mirror*? The user will immediately understand that the avatar in front of him or her is mimicking his or her movements. What's that shiny thing on the mirrored hand? Better have a look at my own hand, there must be something interesting there! This solution seems very promising — it requires very low user attention and no text.
