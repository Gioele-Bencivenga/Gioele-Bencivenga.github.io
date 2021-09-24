---
title: "Autonomous Intelligent Agents"
excerpt: "AI-driven agents competing for food and evolving in a simulated environment, developed with Haxe and HaxeFlixel"
permalink: /projects/auto_agents/

header: 
  teaser: /assets/images/projects/auto_agents/teaser.png
  overlay_image: /assets/images/projects/auto_agents/teaser-wide.png
  overlay_filter: 0.3 # the lower the more visible the image is
  # caption: "This is a caption: [**This is a Link**](https://unsplash.com)"
  actions:
    - label: "Play on Newgrounds"
      url: "https://www.newgrounds.com/portal/view/754129"
    - label: "Play on Itch"
      url: "https://gioele-bencivenga.itch.io/asteroid-shooter"

# vscode auto format changes the - to + breaking the page, watch out for that
sidebar: 

  - title: "Role/s"
    # image: http://placehold.it/350x250 no image needed here
    # image_alt: "placehold alt text"
    text: "Designer, Developer"

  - title: "Responsibilities"
    text: "Design, Implementation"

  - title: "Collaborators"
    text: "[James Borg](https://scholar.google.co.uk/citations?user=unZHiGIAAAAJ&hl=en) - Project Supervisor"

  - title: "Project Status"
    text: "Finished."
    

gallery:

  - url: /assets/images/projects/auto_agents/screenshot1.png
    image_path: assets/images/projects/space_shooter/screenshot1.png
    alt: "Screenshot of "

  - url: /assets/images/projects/auto_agents/screenshot2.png
    image_path: assets/images/projects/space_shooter/screenshot2.png
    alt: "Screenshot of "

toc: true

categories:
  - Simulations

tags:
  - Haxe
  - HaxeFlixel
  - AI
  - Evolution
  - Genetic Algorithms
  - Sensors
  - Simulation

---

Retro arcade space shooter prototype I made using [Haxe](https://haxe.org/) and [HaxeFlixel](https://haxeflixel.com/) with the [Nape](https://joecreates.github.io/napephys/index.html) physics engine.

I started by recreating the [Asteroids demo project](https://haxeflixel.com/demos/FlxTeroids/) found on the Flixel website, then added stuff I liked and/or wanted to learn to use like physics, particle effects, screen shake, enemies in the form of mines that follow and explode on contact, an open world and camera system.

Development has stalled for now, this was my first Flixel project so the code is messy and I need to find the will to restructure some classes before adding more stuff. I learned a lot from making the game though.

## Gallery

{% include gallery caption="Images of the project" %}

## Source Code

The project is Open Source, the repository [can be found here](https://github.com/Gioele-Bencivenga/MLPAgents).

## Technologies Used

Here are the main technologies I used to make this game:

| Technology                                                        | Usage                                                 |
| ----------------------------------------------------------------- | ----------------------------------------------------- |
| [Haxe](https://haxe.org/) + [HaxeFlixel](https://haxeflixel.com/) | Language and Framework in which I programmed the game |
| [Echo Physics](https://austineast.dev/echo/)                      | Physics library mainly used for raycasting            |
| [Visual Studio Code](https://code.visualstudio.com/)              | IDE used for writing the code                         |