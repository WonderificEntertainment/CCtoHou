<h1 align="center">
   <br>
   <br>
   <img width="320" src="./media/logos/houdini-cctools_logo.svg" alt="Houdini CCTools">
   <br>
   <br>
   Houdini CCTools
   <br>
   <br>
</h1>

## Integration Tools for [Reallusion Character Creator][cc] in [SideFX Houdini][houdini]

Houdini CCTools is a [Houdini Digital Asset](https://www.sidefx.com/docs/houdini/assets/intro)
designed to streamline working with models exported from Character Creator. Its
primary focus is enhancing animation workflows, offering robust support for
APEX rigging, including dynamic ragdoll effects.

This project is in an early, experimental phase and is currently unstable. **It
is NOT ready for production use, and there is no available documentation or
support at this time.**

### [Join our Discord server](https://discord.gg/VjxAau35tp)

## Requirements

1. A CC3 or CC3+ character model created using Character Creator exported in FBX
   format.
2. SideFX Houdini v20.5 or above.

## Houdini HDA Information

This repository includes the Limited Commercial Use Houdini Digital Asset (HDA).

Starting with the first v1.0 production-ready release, the project will also be
made available for free on [Orbolt](https://www.orbolt.com/), offering an
unrestricted version of the HDA.

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

## License

This project is released into the public domain as free and unencumbered
software. For more details, see the [UNLICENSE](./UNLICENSE) file.

[cc]: https://www.reallusion.com/character-creator/
[houdini]: https://www.sidefx.com/products/houdini/
