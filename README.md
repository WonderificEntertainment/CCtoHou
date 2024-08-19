# Character Creator Auto Setup for SideFX Houdini

**Note:** This project is in an early, unstable work-in-progress stage with a
lot of experimental testing. **It is NOT production-ready.**

## Project Overview

The aim of this project is to enable automatic Houdini rigging with APEX
(including ragdoll effects) for any model created with Reallusion's Character
Creator. The rigging process is handled within the `cc_auto_setup.hiplc` file.

Eventually this will be turned into a Houdini Digital Asset (HDA) for easier
use.

Motion capture support will be added in the future.

This project is published here to encourage collaboration.

## Houdini File Information

I currently have only a Houdini Indie License, which allows me to produce
Limited Commercial use files (`.hiplc`).

I am seeking sponsorship to acquire a Houdini Commercial License or to
collaborate with SideFX to publish this as an unrestricted `.hip` file.

## Setup Instructions

### Prerequisites

You will need a character model created using Character Creator v4, exported in
FBX format.

### Required Character Creator Export Settings

- **Target Tool Preset:** Maya
- **FBX Options:** Mesh
- Leave the prefix/suffix fields blank.
- Uncheck **Embed Textures**.
- **Default Pose:** A-Pose (CC3+ Bind Pose)
- Uncheck **Use Subdivided Mesh**.

_Note:_ Characters exported with subdivisions are not supported, as the model
will be subdivided within Houdini instead.

You can also use the [free 3D character base models provided by Reallusion](https://www.reallusion.com/character-creator/free-3d-character-base.html).
These base meshes are already correctly set up and compatible.

_Due to Reallusion licensing restrictions, models cannot be distributed in this
repository._

### Directory Setup

1. Save your FBX file with the exact name `character.Fbx` (note the capital "F"
   in `.Fbx`, as this is the default naming convention from Character Creator).
2. Place the `character.Fbx` file in a directory called `geo` within this
   repository.

Your directory structure should look something like this:

```
- geo
    - textures
    - character.Fbx
    - character.json
    - character.fbxkey
- cc_auto_setup.hiplc
- README.md
```

_Note:_ The `geo` directory is included in `.gitignore` for the convenience of
collaborators.

## License

This project is released into the public domain as free and unencumbered
software. For more details, see the [UNLICENSE](./UNLICENSE) file.
