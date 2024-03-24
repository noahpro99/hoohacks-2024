## Inspiration

All four of us are STEM majors, and all four of us did NOT have very memorable, interesting, or fun experiences learning history in school. But we believe that history as a subject is not boring at all. We wanted to enhance the experience of learning history in a way that is both immersive and interactive.

## What it does

3Dera takes any **well-documented historical event**, and it generates a 3D scene that you can **enter in VR**. These scenes are **NOT PRE-MADE**, and are created when prompted. While in the scene, 3Dera plays an audio recording of a description of the historical event, so that you can learn about the history while being immersed in the scene.

## How we built it

There are 3 components behind 3Dera's logic:

1. Object selection from **Objaverse (obj library)**, and placement into a blender scene using x, y, z coordinates and relative size scaling. (Selection is based on the context of the historical event, which is recognized using GPT-4).

2. Skybox (360 view) of the historical event and ground textures are generated by using the **HuggingFace API**. Generated based on the context of the event as well.

3. We use the **Wikipedia API** to collect the information about the historical event, then GPT-4 to summarize and process it into an audio file, which will play when the scene is launched.

## Challenges we ran into

Objects can come in many sizes, orientations, placements, so standardizing and configuring all of these to match the scene of a historical event was very difficult. Especially because Objaverse library is NOT standardized by default, and contains objects from many different sources and authors.

## Accomplishments that we're proud of

This was a very ambitious project, and we believe that it's a very cool way of learning history: by putting yourself directly INTO the history.

## What we learned

Blender, blender scripting, 3D stuff in general, etc.

## What's next for 3Dera

Expand and standardize object library, thus expanding the amount of historical events we can generate scenes for. Better graphics, more accurate/contextual object placements.

Demo: https://youtu.be/L3gGZ3T9t98