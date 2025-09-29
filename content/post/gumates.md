---
title: "Gumates"
description: "Gumates is a casual physics-based co-op game where you and your friend stretch, stick, and stumble your way through challenges. Use your gummy arms to grab, pull, and hold onto objects."
draft: false
type: "post"
tags: ["Unreal","Personal"]
categories: ["2_personalProjects"]
cover: 'medias/gumates_splash.png'
weight: 2
---

{{< figure 
src="medias/gumates_poster.png" 
alt="Gumates"
width=100%
>}}

##### **Genre:** Platformer
#####  **Engine:** Unreal Engine
#####  **Role:** Lead Programmer & Project Manager
##### **Team size:** 5
#####  **Development time:** 4 months
#####  **Link:** *https://zyhu.itch.io/gumates*

---

# About the game

## Game Trailer

<div class="video-container">
  <iframe
    src="https://www.youtube.com/embed/1KNCi4pM8IM"
    allowfullscreen
  ></iframe>
</div>

Gumates is a 2 player couch co-op game where you and your friend play as two gummy bears stuck together.
You'll have to move around together, pull one another and coordinate you movements to get across the various levels.



# My Role: Lead Programmer & Project Manager
## Proejct manager

As project manager I was responsible of maintaining a clear roadmap for the entire developement cycle. Assigning tasks based on priorities and dependencies and making sure to have realistic and feasable deadlines based on everyone's performance and availability.


## Lead Programmer

I also coordinated other programmers to follow coherent standards and assigned tasks based on weekly goals and skill levels as well as implementing most gameplay features such as grabbable objects, physics behaviours and more.

{{< sidebyside
  src1="medias/gumates_clip1.gif"
  alt1="Gumates Working together"
  caption1="Players working together"
  src2="medias/gumates_clip2.gif"
  alt2="Carousel"
  caption2="Gummies carousel"
>}}

# Physics
One of the main challenges in this project was the physical nature of the game. We wanted the physics interactions to drive the gameplay while still maintaining satisfying controls for platforming and hand movements.

This required most animations to blend between ragdoll behaviors and handcrafted animations, while ensuring these forces wouldn’t interfere with the physics simulation or collisions.

{{< sidebyside
  src1="medias/gumates_clip3.gif"
  alt1="Pulling"
  caption1="Players physics animations"
  src2="medias/gumates_clip4.gif"
  alt2="Platforming"
  caption2="Forces in action"
>}}

We ended up working with two separate physics layers: one dedicated solely to animation interactions, which didn’t apply forces to move objects, and another for actual physics-based movements. This approach allowed us to maintain precise control over collisions and interactions while giving player models the ability to stretch and bend, adding visual flair.

# Extra footage

{{< sidebyside
  src1="medias/gumates_clip5.gif"
  alt1="Early mechanics prototypes"
  caption1="Early mechanics prototypes"
  src2="medias/gumates_clip6.gif"
  alt2="Tutorial level greybox"
  caption2="Tutorial level greybox"
>}}
