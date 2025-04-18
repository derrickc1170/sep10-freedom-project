# Entry 5
##### 4/11/25
Context
Today is September 10, and I want to showcase what I built using A-Frame. I gave myself just 4 days to complete this VR project, which was a tight deadline, but it was a great way to challenge myself and explore A-Frame more deeply.

Working on this over the 4 days helped me learn a lot about the tools I'm using and really pushed me to understand how A-Frame works.

### Code
#### Day 1

<!-- (Nothing yet – just getting started!) -->
#### Day 4 – Final Version

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Horror Place in VR</title>
    <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
    <style>
      body { margin: 0; overflow: hidden; }
      #scene { height: 100vh; }
    </style>
  </head>
  <body>
    <a-scene>
      <!-- Sky and lighting -->
      <a-sky color="#0f0f0f"></a-sky>
      <a-light type="directional" intensity="0.4" position="5 5 5"></a-light>
      <a-light type="point" color="#ff0000" intensity="0.8" position="0 2 0"
                animation="property: intensity; to: 0; dir: alternate; dur: 300; loop: true"></a-light>

      <!-- Ground -->
      <a-plane position="0 0 -5" rotation="-90 0 0" width="50" height="50" color="#333333"></a-plane>
      <a-plane position="0 30 -10" rotation="-90 0 90" width="50" height="50" color="#333333"></a-plane>

      <!-- Creepy boxes -->
      <a-box position="-5 2 -10" width="2" height="4" depth="2" color="#333"></a-box>
      <a-box position="-9 2 -10" width="2" height="4" depth="2" color="#333"></a-box>
      <a-box position="5 2 -10" width="2" height="4" depth="2" color="#333"></a-box>
      <a-box position="10 2 -10" width="2" height="4" depth="2" color="#333"></a-box>
      <a-box position="10 2 1" rotation="-0 20 180" width="20" height="4" depth="2" color="#333"></a-box>
      <a-box position="-10 2 6" rotation="-0 20 180" width="20" height="4" depth="2" color="#333"></a-box>
      <a-box position="-10 2 -3" rotation="-0 30 180" width="20" height="4" depth="2" color="#333"></a-box>
      <a-box position="-12 2 6" rotation="-0 0 180" width="20" height="4" depth="2" color="#333"></a-box>

      <!-- Eye -->
      <a-sphere position="3 2 -7" radius="1.5" color="#ffff"></a-sphere>
      <a-sphere position="3 2.1 -6.35" radius="1" color="#555"></a-sphere>
      <a-sphere position="3 2.25 -5.8" radius="0.5" color="#ffff"></a-sphere>

      <!-- Haunted tree (Model not loading yet) -->
      <a-entity gltf-model="url(spooky_tree.gltf)" position="0 0 -15" scale="1 1 1"></a-entity>

      <!-- Fog for mystery -->
      <a-entity fog="type: exponential; color: #222222; near: 5; far: 25;"></a-entity>

      <!-- Ambient lighting -->
      <a-light type="ambient" intensity="0.3" position="0 10 0"></a-light>

      <!-- Sound (not working yet) -->
      <a-sound src="url(spooky_sound.mp3)" autoplay="true" loop="true" volume="0.7" position="0 3 -4"></a-sound>

      <!-- Interactive box -->
      <a-box position="0 2 -5" width="3" height="3" depth="3" color="#222"
             event-set__click="scale: 1.5 1.5 1.5; color: #ff0000"></a-box>

      <!-- Camera -->
      <a-camera position="0 1.6 0" wasd-controls look-controls></a-camera>
    </a-scene>
  </body>
</html>
```

#### What It Can Do
<p>This VR scene creates a spooky horror environment with creepy lights, fog, and an eerie vibe. I also added interactive elements like a box that changes when clicked, and attempted to load a haunted tree model and some sound.</p>

Some problems I ran into:

* `The GLTF model didn’t load correctly. It showed up as a block instead of the full 3D model.`

* `The spooky sound effect didn't play (probably due to file path or browser permissions).`

### Source
Aframe:[here](https://aframe.io/docs/1.7.0/introduction/)
Lighting:[here](https://aframe.io/docs/1.7.0/components/light.html#main)
Fog:[here](https://aframe.io/docs/1.7.0/components/fog.html#main)
Camera:[here](https://aframe.io/docs/1.7.0/components/camera.html#main)
Background:[here](https://aframe.io/docs/1.7.0/primitives/a-sky.html#main)
### Skill:
#### Googling
* Googling was one of the most helpful things I did while working with A-Frame. Whenever I got stuck or didn’t know how to do something, I searched it on Google. Simple searches like “how to add light in A-Frame” or “how add sound in A-frame” gave me answers fast. I found useful tutorials, documentation, and examples that helped me understand what to do. Google helped me fix bugs, learn new things, and make my scene look better. It was like having a guide right there whenever I needed help

#### Creativity
* Creativity was a big part of working with A-Frame. I had to imagine what I wanted my 3D scene to look like and figure out how to make it happen. I thought about things like what kind of mood I wanted—spooky, fun, calm—and chose colors, lighting, and objects that matched that feeling. I also came up with ideas for how to make the scene more interesting, like adding fog, sound, or animations. Creativity helped me take a basic scene and turn it into something unique and fun to explore.

### Takeaway
* <p>Even with just 4 days, I created a full VR scene with interactive elements. I learned how to use A-Frame’s core features, especially lighting and camera controls. While some features didn’t work as expected, I still learned a lot about 3D asset management and troubleshooting. Next time, I’ll give myself more time for testing models and adding polish.</p>

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
