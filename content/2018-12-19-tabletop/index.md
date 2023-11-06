+++
title = "A tabletop engine with fancy tools for developers"
slug = "tabletop"
template = "portfolio-entry.html"
[extra]
tags = ["Unity", "C#"]
opt_preview_img = ["engine01.gif", "default", 5, 1]
+++

This is a tabletop engine made with Unity: a player can drag-and-drop cards across different *decks* (a *deck* is considered a collection of cards that can be laid down in different ways). A developer should be able to easily set up a scene for any board game (not really *any* but you get the point). To help out developers I built some tools to arrange the scene using the powerful feature of the Unity Editor.

{{ article_buttons(buttons=["Source code", "https://github.com/marcomoroni/set10110"]) }}

This project made me realize how much I enjoy tools development. Tools are extremely important especially for big games, and with them I can even do some UX design that I like so much!

The engine based around two concepts: *cards* and *decks*. Decks hold parameters on how to lay down the cards it owns and cards can be dragged and dropped between decks.

I built a handy Editor Window to manage the cards that will be added to the scene; it was soon clear that it was a necessary tool to have, otherwise every card asset would have been needed to be changed individually. It consists on a database where cards can be added, deleted or duplicated.

{{ image(src="engine01.gif", stretch=true, can_toggle_full_width=true) }}

{{ image(src="gizmos.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="database.png", stretch=true, can_toggle_full_width=true) }}

{{ image(src="inspector.png", stretch=true, can_toggle_full_width=true) }}
