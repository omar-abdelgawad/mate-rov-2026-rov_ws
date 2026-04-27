# MATE-ROV-2026-rov_ws

> [!WARNING]
> DON'T USE THIS REPOSITORY. it is not the one used in the competition. 

We tried building the environment using pixi for ease of installing ros but there was a conflict between ros-jazzy and the package for opencv compiled with gstreamer and contrib. The conflict was due to a pinned version of libprotobuf in the opencv package and in the end the gui didn't really use ros since the joystick was on another laptop (pilot's laptop was different form gui). Also turned out that the pinned version which caused major conflicts was to fix something in windows so it may be a good idea to compile it ourselvers as a conda package and publish it to prefix.dev.

All of these issues combined with the lack of time forced us to ditch this setup and build the environment the old school way through just pip installing into a venv. we also exposed the virtual environment to the system site packages to allow using the globally install ros-jazzy.
