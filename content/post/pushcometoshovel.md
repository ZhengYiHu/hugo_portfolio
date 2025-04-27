---
title: "Push Comes to Shovel"
description: "Push Comes to Shovel is a story driven puzzle game where you’re tasked with recovering three lost organs for a peculiar doctor."
draft: false
type: "post"
tags: ["Unreal","Personal"]
categories: ["2_personalProjects"]
cover: 'medias/pcts_thumbnail.jpg'
weight: 3
---
{{< figure 
src="medias/pcts_banner.jpg" 
alt="Main Hub"
width=100%
>}}
##### **Genre:** Story driven - Puzzle
#####  **Engine:** Unreal Engine
#####  **Role:** Lead programmer
##### **Team size:** 18
#####  **Development time:** 4 months
---
# About the game

You play as **Leo**, a young archeologist armed with a shovel.
You can form dirt piles and dig up underground tunnels. Your quest is to help a mysterious doctor recovering some lost organs alongside your loyal bunny companion **Scoop**

{{< sidebyside
  src1="medias/pcts_piling.gif"
  alt1="Piling"
  caption1="Piling up dirt piles"
  src2="medias/pcts_tunneling.gif"
  alt2="Tunneling"
  caption2="Tunneling across surfaces"
>}}

# My Role: Lead Programmer

As the **Lead Programmer**, I was responsible for overseeing the programming team by assigning tasks based on each member’s strengths and ensuring clear communication between departments. I worked closely with designers, artists, and writers to align technical requirements with the creative vision of the project.

On the development side, I built and maintained key systems that formed the backbone of the game, including the **dialogue system**, **quest system**, and **save/load** functionality. To streamline development, I also created user-friendly interfaces and tools that allowed non-programmers to easily implement content without needing to touch code.


## Quest System

I developed a fully **data-driven** quest system, where all quest logic is based on the game's save data. Whenever the player’s progress changes, quests automatically update to reflect the new state.

Each quest can define a variety of conditions, such as previously completed quests, inventory contents, or world states (like interacting with specific objects).

This system accommodates the design of non-linear quests and branching dialogues, allowing for complex player choices and dynamic storylines. Designers can create as many quests as they want, with as much depth and variation as needed, simply by editing a data file. No changes to the game's blueprints are required.


{{< figure 
src="medias/quest_system.png" 
alt="Quest"
width=100%
>}}

## Dialogue System

Given the non-linear nature of the game, the dialogue system needed to dynamically display different dialogue options based on the current game state. To keep the branching dialogue and associated logic well-organized, I implemented a text-based dialogue editor.

I integrated <a href="https://github.com/sinbad/SUDS" target="_blank">Steve’s Unreal Dialogue System (SUDS)</a>  to assist with parsing and encoding dialogue data efficiently. The system is now capable of handling complex events, such as giving items or triggering animations at specific points during conversations.

This ensures that dialogues evolve in response to player actions, supporting a rich, interactive narrative experience.

<div style="display: flex; justify-content: space-between; gap: 20px;">
    <figure style="text-align: center;">
        <img src="medias/harry_dialogue.png" alt="harry dialogue" style="height: 300px; object-fit: cover;">
        <figcaption>Harry Dialogue</figcaption>
    </figure>
    <figure style="text-align: center;">
        <img src="medias/pcts_magic_trick.gif" alt="magic trick" style="height: 300px; object-fit: cover;">
        <figcaption>Magic Trick</figcaption>
    </figure>
</div>

## In Game Debugger

As the game gives players more freedom, it becomes essential to test a wide range of possible situations, including the most unlikely ones. To support this, I developed a custom debugger panel that not only provides a detailed view of the game's current state, but also allows designers and QA to manipulate game elements in real-time.

This panel enables testers to quickly adjust variables, trigger events, and observe how the world updates instantly, ensuring that all scenarios are covered during testing.

{{< figure 
src="medias/pcts_debugger.gif" 
alt="Debugger"
width=100%
>}}