<h1 align="center">
   <br>
   <br>
   <img width="320" src="./media/logos/houdini-cctools_logo.svg" alt="Houdini Character Creator Tools (CCTools)">
   <br>
   <br>
</h1>

# Character Creator Tools for SideFX Houdini

**Note:** This project is in an early, unstable work-in-progress stage with a
lot of experimental testing. **It is NOT production-ready and there is currently
no documentation or support.**

## Project Overview

The aim of this project is to provide a collection of tools contained within a
[Houdini Digital Asset](https://www.sidefx.com/docs/houdini/assets/intro) to
facilitate animation via APEX rigging (including ragdoll effects) for any model
created with Reallusion's Character Creator.

### [Join our Discord server](https://discord.gg/VjxAau35tp)

## Requirements

1. A CC3 or CC3+ character model created using Character Creator exported in FBX
   format.
2. SideFX Houdini v20.5 or above.

## Houdini HDA Information

This repo contains the Limited Commercial Use Houdini Digital Asset (HDA).

Beginning with the first v1.0 production-ready release, this project will also
be published on [Orbolt](https://www.orbolt.com/) for free in order to provide
an unrestricted HDA.

## Setup Instructions

1. Clone or download this repo.

2. Install the HDA `/otls/cctools.0.0.1.hdalc` by following the
   official docs on how to [install and manage Houdini digital assets](https://www.sidefx.com/docs/houdini/assets/install.html).

3. Open `cctools_demos.hiplc` to see a few different demos. _Note:_ demos are
   works-in-progress and may not work.

### Required Character Creator Export Settings

- **Target Tool Preset:** Maya
- **FBX Options:** Mesh
- Leave the prefix/suffix fields blank.
- Uncheck **Embed Textures**.
- **Default Pose:** A-Pose (CC3+ Bind Pose)
- Uncheck **Use Subdivided Mesh**.

_Note:_ Characters exported with subdivisions are not supported.

You can also use the [free 3D character base models provided by Reallusion](https://www.reallusion.com/character-creator/free-3d-character-base.html).
These base meshes are already correctly set up and compatible.

_Due to Reallusion licensing restrictions, models cannot be distributed in this
repository._

## License

This project is released into the public domain as free and unencumbered
software. For more details, see the [UNLICENSE](./UNLICENSE) file.
