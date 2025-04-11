# Entry 5
##### 4/11/25
### Context
<p>Today In Sep 10,I am going showcase What i make from aframe.Aframe I gave myself 4 day to compeleted a project which it is really short to finish.</p> <p>Doing this during these 4 day will make learn about of my learning tool and show how I use aframe.</p>

### Code
<p>This is on 1 day</p>
<p>This is after 4 day</p>

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
      <!-- Set up a dark sky to create an eerie atmosphere -->
      <a-sky color="#0f0f0f"></a-sky>

      <!-- Add lighting for a creepy atmosphere -->
      <a-light type="directional" intensity="0.4" position="5 5 5"></a-light>
      <a-light type="point" color="#ff0000" intensity="0.8" position="0 2 0"
                animation="property: intensity; to: 0; dir: alternate; dur: 300; loop: true"></a-light>

      <!-- Add ground (dark floor) -->
      <a-plane position="0 0 -5" rotation="-90 0 0" width="50" height="50" color="#333333" shadow="true"></a-plane>
      <a-plane position="0 30 -10" rotation="-90 0 90" width="50" height="50" color="#333333" shadow="true"></a-plane>

      <!-- Creepy box and objects -->
      <a-box position="-5 2 -10" width="2" height="4" depth="2" color="#333" shadow="true"></a-box>
      <a-box position="-9 2 -10" width="2" height="4" depth="2" color="#333" shadow="true"></a-box>
      <a-box position="5 2 -10" width="2" height="4" depth="2" color="#333" shadow="true"></a-box>
      <a-box position="10 2 -10" width="2" height="4" depth="2" color="#333" shadow="true"></a-box>
      <a-box position="10 2 1" rotation="-0 20 180" width="20" height="4" depth="2" color="#333" shadow="true"></a-box>
      <a-box position="-10 2 6d" rotation="-0 20 180" width="20" height="4" depth="2" color="#333" shadow="true"></a-box>
      <a-box position="-10 2 -3" rotation="-0 30 180" width="20" height="4" depth="2" color="#333" shadow="true"></a-box>
      <a-box position="-12 2 6" rotation="-0 0 180" width="20" height="4" depth="2" color="#333" ></a-box>
      <!--Eye-->
      <a-sphere position="3 2 -7" radius="1.5" color="#ffff" shadow="true"></a-sphere>
      <a-sphere position="3 2.1 -6.35" radius="1" color="#555" shadow="true"></a-sphere>
      <a-sphere position="3 2.25 -5.8" radius="0.5" color="#ffff" shadow="true"></a-sphere>
      <!-- Haunted tree(No Model)-->
      <a-entity gltf-model="url(spooky_tree.gltf)" position="0 0 -15" scale="1 1 1" rotation="0 0 0"></a-entity>

      <!-- Fog for mystery -->
      <a-entity fog="type: exponential; color: #222222; near: 5; far: 25;"></a-entity>

      <!-- Ambient lighting for spooky effect -->
      <a-light type="ambient" intensity="0.3" position="0 10 0"></a-light>

      <!-- Creepy sound effects(No Sound) -->
      <a-sound src="url(spooky_sound.mp3)" autoplay="true" loop="true" volume="0.7" position="0 3 -4"></a-sound>

      <!-- Interactive box that changes when clicked -->
      <a-box position="0 2 -5" width="3" height="3" depth="3" color="#222" shadow="true"
             event-set__click="scale: 1.5 1.5 1.5; color: #ff0000"></a-box>

      <!-- Add a camera with movement and look controls -->
      <a-camera position="0 1.6 0" wasd-controls="enabled: true" look-controls="enabled: true"></a-camera>

    </a-scene>
  </body>
</html>
```
<p>This what it can do.</p>

### Source

### Takeaway

### Skill
Text

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
