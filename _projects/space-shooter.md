---
title: "Arcade Space Shooter"
excerpt: "A top down, retro looking, space shooter developed with Haxe and HaxeFlixel"
permalink: /projects/space_shooter/

header: 
  teaser: /assets/images/projects/space_shooter/teaser.png
  overlay_image: /assets/images/projects/space_shooter/teaser-wide.png
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
    text: "[Niccolo' Toscani](https://www.instagram.com/niccolo_toscani/?r=nametag) - Background Music Composer"

  - title: "Project Status"
    text: "Unfinished, development stalled"
    

gallery:

  - url: /assets/images/projects/space_shooter/screenshot1.png
    image_path: assets/images/projects/space_shooter/screenshot1.png
    alt: "Screenshot of spaceship shooting"

  - url: /assets/images/projects/space_shooter/screenshot2.png
    image_path: assets/images/projects/space_shooter/screenshot2.png
    alt: "Screenshot of spaceship shooting"

toc: true

categories:
  - Games

tags:
  - Haxe
  - HaxeFlixel
  - Arcade
  - Retro
  - Space
  - Shooter
  - Development

---

Retro arcade space shooter prototype I made using [Haxe](https://haxe.org/) and [HaxeFlixel](https://haxeflixel.com/) with the [Nape](https://joecreates.github.io/napephys/index.html) physics engine.

I started by recreating the [Asteroids demo project](https://haxeflixel.com/demos/FlxTeroids/) found on the Flixel website, then added stuff I liked and/or wanted to learn to use like physics, particle effects, screen shake, enemies in the form of mines that follow and explode on contact, an open world and camera system.

Development has stalled for now, this was my first Flixel project so the code is messy and I need to find the will to restructure some classes before adding more stuff. I learned a lot from making the game though.

## Gallery

{% include gallery caption="Some screenshots from the game" %}

## Source Code

The project is Open Source, the repository [can be found here](https://github.com/Gioele-Bencivenga/FlixelGame).

## Technologies Used

Here are the main technologies I used to make this game:

| Technology                                                        | Usage                                                          |
| ----------------------------------------------------------------- | -------------------------------------------------------------- |
| [Haxe](https://haxe.org/) + [HaxeFlixel](https://haxeflixel.com/) | Language and Framework in which I programmed the game          |
| [Visual Studio Code](https://code.visualstudio.com/)              | IDE used for writing the code                                  |
| [Piskel](https://www.piskelapp.com/)                              | PixelArt drawing tool used for minor edits on the image assets |
| [Audacity](https://www.audacityteam.org/)                         | Audio software used for minor edits on the audio assets        |

## Credits

### Images

- Asteroid images by Cayden Franklin, [source here](https://opengameart.org/content/pixel-art-2d-asteroid-pack)
- Ship image by scofanogd, [source here](https://opengameart.org/content/spaceship-9)
- Laser and particles by Master484, [source here](https://opengameart.org/content/bullet-collection-1-m484)

### Sounds

- Sound effects by [Juhani Junkala](https://www.youtube.com/watch?v=dbACpSy9FWY), [source here](https://opengameart.org/content/512-sound-effects-8-bit-style)

### Music

- Background music by [Niccolo' Toscani](https://www.instagram.com/niccolo_toscani?r=nametag)
