# Minecraft: Cosmic Age!

<img src=./graphics/logo/logo_3x2.png style="max-width: 50%;">

## Description
  Explore the universe by building self sustainable automation lines on planets inorder to keep you allive. 
  
  This mod aims to add tons of unique planets for the player to explore whilst also giving some automation / factory building vibes.
  On every planet you will have to automate the things that keep you allive whilst also constructing a new / better space ship to leave the planet and travel even deeper into space.
  
## For developers

---

This datapack contains a copy of my datapack-common code library which can be found [here](https://github.com/TheBlackSwitch/datapack-common-code)

---

### More about beet/bolt:
This project uses beet to build all datapack code.
Beet is the loader, it loads a plugin called bolt which allows for bolt files to combine python and mcfunction.
Beet also loads a plugin called mecha which is a language server for bolt. It basically checks the code for any errors when building the project.

The code is found in ``src/assets`` (for the resourcepack) and ``src/data`` (for the datapack). These folders act as a normal data/resource pack aswell as a bolt project. Most of the bolt code will be written in ``src/data/modules``.

The ``build`` folder contains the generated datapack and resourcepack, this is the file that would actually be downloaded. This gets regenerated everytime the project is built and thus making changes here is not such a good idea.

To make change to the build files, you'll have to setup a local python virtual environment with these packages installed:
    - beet
    - bolt
    - aegis (for linting, completions and syntax highlighting | optional)
    - pillow
Then you can link your minecraft instance with beet so it autmatically puts the resource-and-datapack into your world folder using ``beet link`` To build the project, you can do ``beet build`` everytime or do ``beet watch``to make it auto build on changes. More on how to setup beet can be found [here](https://mcbeet.dev/)

