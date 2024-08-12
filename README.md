# Virtuoso Engine
<img src="https://github.com/user-attachments/assets/f954bf75-07e8-4741-9008-fc52df5a76c0" width="320"/>

## Description and Philosophy
Virtuoso Engine is my personal game and app development framework that I've been working on for about a decade or so in various iterations, and have shipped multiple apps on.  The latest version is being used in the development of "Killing Baby Hitler."

The philosophy of the engine is to be a lightweight framework style engine, sort of like [RayLib](https://www.raylib.com/), but more focusing on C++20, 3D, and physics rather than C99/2D.  I wanted to make this because it's the language / paradigm under which I'm most productive as a very experienced C++ programmer with lots of graphics programming and graphics driver experience.

I also am a really strong booster of the ["STB"](https://github.com/nothings/stb) style of library - of making components or functionality that can be forked off without dependencies into a single header, permissive license "library."

The "full" engine will be posted here on this page with an easy build / install and documentation... eventually :).  For now see the public components, third party libraries, and screenshots below.

## Public Components
Several components of the engine can be seen publicly on my GitHub:

[YarnMachine](https://github.com/VirtuosoChris/YarnMachine) - A standalone C++ virtual machine for [YarnSpinner](https://www.yarnspinner.dev/), a narrative scripting language I use in KBH for dialogue and game scripting.

[Quake Style Console](https://github.com/VirtuosoChris/VirtuosoConsole) - Debug console and IMGUI widget.  The first version of this was written 11 years ago as an experiment but I've been maintaining and using this ever since.

[GLSugar](https://github.com/VirtuosoChris/GLSugar) - Graphics framework for modern / AZDO style OpenGL development with nicer syntax.  This has code for basic texture and shader handling, as well as struct annotation to easily make VAO's and [UBOs](https://github.com/VirtuosoChris/GL_UBO/) with correct memory alignments.  Built on GLHPP (discussed below), a library written by a colleague to which I am a contributor.

[uJNI](https://github.com/VirtuosoChris/uJNI) - Helper functions and classes to wrangle JNI / NDK things.  Not used in KBH, but was rapidly developed for the 2016/2017 iteration of the engine to ship a Fireworks Show VR app on the GearVR platform (Android).

[Spherical Harmonics](https://github.com/VirtuosoChris/SphericalHarmonics) - Utility code for environment map filtering.  Used for glossy HDR environment rendering in unreleased prototypes, and diffuse probe convolution in Fireworks Show VR.

[Noise](https://github.com/VirtuosoChris/Noise) - Perlin Noise Generation : Used in unreleased prototypes.

[Autoreduce](https://github.com/VirtuosoChris/AutoReduce) - Frequency space texture analysis and reduction

[VirtuosoImage](https://github.com/VirtuosoChris/VirtuosoImage/) - Templated multidimensional array with views, customizable backing store, and some common algorithms.  Used for CPU-side algorithm prototyping.  Older.

## 3rd Party Libraries
A lot of the work on the engine is curating which third party libraries to use vs which things to write myself.  The engine puts together and builds on top of lots of third party open source libraries, including but not limited to:

[glhpp](https://github.com/Steve132/glhpp/) - Object oriented, DSA OpenGL header by a colleague, to which I am a contributor.

[PhysX](https://github.com/NVIDIA-Omniverse/PhysX/) - General purpose physics, collision, math, and simulation library

[Eigen](https://eigen.tuxfamily.org/index.php?title=Main_Page) - For matrix and linear algebra

[Dear ImGUI](https://github.com/ocornut/imgui) - For user interfaces and tools prototyping.  Also several other 3rd party repo's for adding gizmos, markdown, and file dialogs to IMGUI.

[MiniAudio](https://miniaud.io/) - For 3D sound playback and music streaming

[Yarn Spinner](https://github.com/YarnSpinnerTool/YarnSpinner) - For dialogue and narrative scripting.  I use their VSCode plugin and their compiler, but built my own C++ runtime discussed above.

[Debug Draw](https://github.com/glampert/debug-draw) - For wireframe primitive visualization

[GLFW](https://github.com/glfw/glfw) and [GLFWPP](https://github.com/Steve132/glfwpp) - for cross platform windowing system and input

[STB](https://github.com/nothings/stb) - Image loading and other miscellanea

[nlohmann's JSON](https://github.com/nlohmann/json) - For data serialization

[MiniZ](https://github.com/richgel999/miniz/) - for compression and bundling of map data

[protobuf](https://github.com/protocolbuffers/protobuf) - dependency for YarnMachine VM

[Vince's CSV parser](https://github.com/vincentlaucsb/csv-parser) - dependency for YarnMachine VM

[GLAD](https://glad.dav1d.de/) - OpenGL function loader

## Made with Virtuoso

https://github.com/user-attachments/assets/77d3f63f-70c5-4d7e-8026-a8b3d5da427a

![fwgif](https://github.com/user-attachments/assets/8d931ee5-a879-4dd9-9510-eb06d53e7db1)

HDR Stereo Reflection Maps (Virtuoso, GearVR 2016)

![HDR Mobile VR 2016](https://github.com/user-attachments/assets/eb760afc-2706-41dc-8555-2f7b8872b3f5)

Water Shader (Virtuoso, GearVR 2016)

![GLES Mobile Water Shader 2016](https://github.com/user-attachments/assets/4b38adad-a7de-492b-943d-b478295f9659)

Bloom, HDR, Emissive Mapping (2012)

![Bloom HDR Emissive 2012](https://github.com/user-attachments/assets/a61549a3-50e8-4731-a993-172cfa38cbd7)

Spherical Harmonics Convolutions (2010)

![Spherical Harmonic Lighting Probe Convolutions](https://github.com/user-attachments/assets/5a50ba4c-e26d-4fc6-b661-91d796aae4ed)

Shadowmaps, Bloom, LOD, HDR (Virtuoso, 2017)

![ShadowMaps Bloom LOD HDR](https://github.com/user-attachments/assets/6f88d5d3-3fcb-4c18-8575-c63203f1dd1e)

Shadowmaps, Bloom, HDR (Virtuoso Engine, 2017)

![Shadowmaps Bloom HDR](https://github.com/user-attachments/assets/e1755a54-dc48-44b5-b906-08e45a69b41a)

