---
title: "Autonomous Intelligent Agents"
excerpt: "AI-driven agents competing for food and evolving in a simulated environment, developed with Haxe and HaxeFlixel"
permalink: /projects/auto_agents/

header: 
  teaser: /assets/images/projects/auto_agents/teaser.png
  overlay_image: /assets/images/projects/auto_agents/teaser.png
  overlay_filter: 0.3 # the lower the more visible the image is
  # caption: "This is a caption: [**This is a Link**](https://unsplash.com)"
  actions:
    - label: "Play on Newgrounds"
      url: "https://www.newgrounds.com/portal/view/..."
    - label: "Play on Itch"
      url: "https://gioele-bencivenga.itch.io/auto-agents"

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

  - url: /assets/images/projects/auto_agents/environment.png
    image_path: assets/images/projects/auto_agents/environment.png
    alt: "Image displaying the enclosed environment where the simulation takes place. "

  - url: /assets/images/projects/auto_agents/foodnpoison.png
    image_path: assets/images/projects/auto_agents/foodnpoison.png
    alt: "Image showing the representation of food (in magenta) and poison (in green). Their hitboxes are a circle even though they are displayed as a colored square."
  
  - url: /assets/images/projects/auto_agents/mlp_structure.png
    image_path: assets/images/projects/auto_agents/mlp_structure.png
    alt: "Image showing the structure of the multilayer perceptron. Size of the input and hidden layer was varied during experiments."
  
  - url: /assets/images/projects/auto_agents/mlp_test.png
    image_path: assets/images/projects/auto_agents/mlp_test.png
    alt: "Screenshot of the program used to test the functioning of the multilayer perceptron."
  
  - url: /assets/images/projects/auto_agents/sensors.png
    image_path: assets/images/projects/auto_agents/sensors.png
    alt: "Image showing the sensors that the agents used to sense the environment. Number and length of sensors was varied during experiments."

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

## Project Description

Dissertation (final year project) made while at Keele University.
The agents have a set of rays shooting from in front of them to sense the environment and a multilayer perceptron as a brain to decide what to do.
They can bite food, each other, or poison and have a limited amount of energy.
At set intervals the best individuals in the population reproduce and the worst are removed from the simulation, over time agents will be fitter and fitter, surviving more time.

## Gallery

{% include gallery caption="Project-related images" %}

## Source Code

The project is Open Source, the repository [can be found here](https://github.com/Gioele-Bencivenga/MLPAgents).

## Technologies Used

Here are the main technologies I used to make this game:

| Technology                                                        | Usage                                                 |
| ----------------------------------------------------------------- | ----------------------------------------------------- |
| [Haxe](https://haxe.org/) + [HaxeFlixel](https://haxeflixel.com/) | Language and Framework in which I programmed the game |
| [Echo Physics](https://austineast.dev/echo/)                      | Physics library mainly used for raycasting            |
| [Visual Studio Code](https://code.visualstudio.com/)              | IDE used for writing the code                         |