# Entry 5
##### 3/15/20

### What I am using to learn    
So far I have watched a ton of Blender videos to help me with my 3D models for the web game my partner and I are making. Currently, I am learning as I go instead of watching beginner level videos that teach you the basics. For example, if I am stuck on a specific problem on a model I am trying to create, I would search up the problem and solve it as I go.

### Engineering Design Process
In the Engineering Design Process, my partner and I are up to step five which is creating a prototype of the web game. So far we have most of the models that we will be using in the javascript based game which will be implemented into the game using three.js. There are also some models created using three.js itself and some models created usnig Blender.  

![Example](https://i.gyazo.com/c1cc6b1af7722ab1c40014113cbc8b07.png)   
```import { OrbitControls } from "three/examples/jsm/controls/OrbitControls";

import Game from "@/structures/Game";

import "@/assets/scss/main.scss";

document.querySelector("#btn-start")?.addEventListener("click", async () => {
  document.getElementById("start-wrapper")?.remove();

  const game = await Game.create({
    "metadata": {
      "artist": "Test",
      "beatmapper": "Me",
      "bpm": 146,
      "mp3": "/flag.mp3",
      "title": "Test"
    },
    "notes": [
      // { "column": 1, "start": 6.5 },
      { "column": 1, "start": 0 },
      { "column": 2, "start": 9.8 },
      { "column": 3, "start": 13.1 },
      { "column": 4, "start": 16.4 },
      { "column": 5, "start": 26.3 },
      { "column": 1, "start": 29.5 },
      { "column": 2, "start": 32.8 },
      { "column": 3, "start": 36.1 },
      { "column": 4, "start": 39.4 },
      { "column": 5, "start": 42.7 },
      { "column": 1, "start": 44.1 },
      { "column": 2, "start": 46 },
      { "column": 3, "start": 49.3 },
      { "column": 4, "start": 52.6 }
    ],
    "versioning": {
      "beatmap": "1.0.0",
      "fileFormat": "1.0.0"
    }
  });

  game.start();

  new OrbitControls(game.video.camera, game.video.renderer.domElement);
});
```
[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
