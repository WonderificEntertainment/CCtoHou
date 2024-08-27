# Character Creator Auto Setup for SideFX Houdini

**Note:** This project is in an early, unstable work-in-progress stage with a
lot of experimental testing. **It is NOT production-ready and there is currently
no documentation or support.**

## Project Overview

The aim of this project is to provide a collection of tools contained within a
[Houdini Digital Asset](https://www.sidefx.com/docs/houdini/assets/intro) to
facilitate animation via APEX rigging (including ragdoll effects) for any model
created with Reallusion's Character Creator.

## Discord

This project isn't large enough to justify its own dedicated Discord server.
Instead, discussions take place in a thread on the [Think Procedural](https://thinkprocedural.com/)
Discord server. To join the conversation, navigate to the [Character Creator Auto Setup for Houdini thread](https://discord.com/channels/230123485668573184/1275123376385429556)
in the `#rigs_kinefx_apex` channel, located under the `ANIMATION/RIGGING`
category.

**Note:** I am just a regular member of Think Procedural. I have no special
privileges, and this project is not officially endorsed by Think Procedural or
SideFX.

## Requirements

1. A character model created using Character Creator v4, exported in FBX format.
2. SideFX Houdini v20.5 or above. The Wrinkle Deformer node added in v20.5 is
   utilized so prior versions are not supported.

## Houdini HDA Information

I currently have only a Houdini Indie License, which allows me to produce
Limited Commercial use digital assets (`.hdalc`).

I am seeking sponsorship to acquire a Houdini Commercial License or to
collaborate with SideFX to publish this as an unrestricted `.hda` file.

## Setup Instructions

1. Clone or download this repo.

2. Install the HDA `/otls/sop_cc.ccautosetup.0.0.1.hdalc` by following the
   official docs on how to [install and manage Houdini digital assets](https://www.sidefx.com/docs/houdini/assets/install.html).

3. Open one of the projects in the `/examples` directory.

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

## License

This project is released into the public domain as free and unencumbered
software. For more details, see the [UNLICENSE](./UNLICENSE) file.
