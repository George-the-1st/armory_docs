# User Interface

This page lists all user interface elements added to Blender by Armory and goes into basic detail on them. If you are already comfortable with essentials of Blender, this page serves as a good overview of Armory additions.

## 3D View

At the bottom of 3D viewport is the **Play in Viewport** button. Pressing this button will start Armory if it's not already running, and then proceeds to render the opened scene in the 3D viewport.

<img src="img/start0.jpg" alt="Drawing" style="width: 600px;"/>

When running the player, **Stop** and **Pause** buttons are available. If there is a message received from any of the running scripts (using print() in Python, trace() in Haxe or console.log() in JavaScript), it will be displayed next to those buttons.

<img src="img/start1.jpg" alt="Drawing" style="width: 600px;"/>

---

## Render panel

### Play

<img src="img/render0.png" alt="Drawing" style="width: 260px;"/>

  Here we see the play button that quickly generates a perview for your game at the very top under Armory Play in the Render Properties. Under that we see the Viewport Camera checkbox. Selecting it starts the game from the perspective of the active camera in the scene (current limitations require a camera regardless). Not selecting it starts the game from the perspective of your work camera (your point of view) as it is in your viewport. Below that we see the Runtime dropdown menu that defines the way that your game will be run (e.g. Selecting Browser will generate the game to run in your browser). Right under that we see the navigation dropdown menu. The "walk" method will allow you to use WASD to move around while moving your mouse to look. Viewport Camera must be checked to have access to navigation methods.

  The "advanced" checkbox allows the options below it to become active so you must allow advanced options to have access to those abilities. Doing that gets you access to the Debug Console which allows you to have an active console that generates while playing the game to see important information like framerate and errors. Live Patching allows you to sync the running player data to Blender (EDIT: NEEDS FURTHER EXPLAINATION). Lastly we see Auto Build which rebuilds your scene on operator changes (EDIT: NEEDS FURTHER EXPLAINATION).

### Build

<img src="img/render1.png" alt="Drawing" style="width: 260px;"/>

  Under Armory Build in Render properties we see several features. First off, we see the build button. Unlike the Armory Play menu that generates a light build in order to test gameplay, the Armory Build menu is designed to compile and build your game. The Kode Studio button opens up your project in the Kode Studio IDE (Internal Design Environment) in order to edit the code. Also in this button list is the Clean button which cleans the cached data thus making it so Armory runs the latest code you made.
  
  The Target dropdown menu is the platform you will be compiling your game for. The Advanced checkbox lets you have access to the features below it. The Cache Shaders button simply means that the shaders in your game will be cached and will not be rebuilt. It should be noted that all cached data will be rebuilt regardless of exceptions by the Clean button (NOTE: NEEDS TO BE DOUBLE CHECKED IT TRUE). The Minimized Data checkbox exports the scene data in binary in order to keep the data size small. The Optimize Meshes button exports more efficient geometry indices. It should be noted that this can prolongue build times. Selecting the Sampled Animation checkbox will export object animation as raw matrices. The Deinterleaved Buffers checkbox will use deinterleaved vertex buffers. The GPU Skinning checkbox allows you to limit bounces and samples.
  
  The physics libraries can also be changed and opted to not be included at all Under the Libraries name. Currently physics and Navigation libraries are available to change and the only options available are the use of Bullet Physics and Recast Navigation or the opting out of one or both of these.

### Project

<img src="img/render2.png" alt="Drawing" style="width: 260px;"/>

  In the Armory Project submenu under Render Properties we have the ability to name the project and name the package name for scripts. Under that we see the ability to select the source file appended to khafile.js and the ability to have the file of commands appended to khamake. Below that we see the Publish Project button which generates executable files for you to run based on the target option selected below that.
  
  The Advanced checkbox below that allows access to the advanced features. The Load Active Scene checkbox loads the currently edited scene when the player is launched. Selecting the Export Hidden Renders checkbox exports hidden objects. The Spawn All Layers button spawns objects from all scene layers. This means that objects from all layers will spawn into your built game. The Check for Updates button will take you to the Armory Latest Build page to check for and find updates for Armory (WARNING: CURRENTLY NOT TRUE. CURRENTLY TAKES YOU TO WIKI...SAME WIKI THIS PAGE IS ON).
  
---

## Scene Panel

<img src="img/scene0.png" alt="Drawing" style="width: 260px;"/>

  The Armory Props menu can be found in the Scene properties tab. Selecting the Export checkbox will allow the export of scene data when checked after project has been exported (NOTE: RELATIONSHIP THIS NEEDS TO BE BETTER EXPLAINED). The Export Grease Pencil checkbox will export the grease pencil data. The Invalidate Grease Pencil Cache will delete cached grease pencil data and require reloading most recent data next time in use. The Compress Data checkbox packs data into zip file to decrease file size

---

## World Panel

<img src="img/world0.png" alt="Drawing" style="width: 260px;"/>

<img src="img/world1.png" alt="Drawing" style="width: 260px;"/>

---

## Object Panel

### Props

<img src="img/object0.png" alt="Drawing" style="width: 260px;"/>

### Traits

<img src="img/object1.png" alt="Drawing" style="width: 260px;"/>

---

## Camera Panel

<img src="img/camera0.png" alt="Drawing" style="width: 260px;"/>

---

## Data Panel

<img src="img/data0.png" alt="Drawing" style="width: 260px;"/>

---

## Material Panel

<img src="img/material0.png" alt="Drawing" style="width: 260px;"/>
