# OpenGL Starter

Template to get started with OpenGL 

## Building

Tested with cmake 3.20.4 and Visual Studio 2019

### Prerequisites
You need to install the following:
- Visual Studio 2019
- CMake

### Building & Project generation
Generate a Visual Studio Project on Windows:

```
git clone --recursive https://github.com/Latios96/opengl-starter.git
cd opengl-starter
mkdir build
cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
```
If this succeeds, you can open the generated Visual Studio project in Visual Studio. You can also use another IDE like Clion, just make sure to pass the `OptiX_ROOT_DIR` in the Cmake options.

If you prefer to build on the command line, use this command: (As far as I tested, this works only with the Visual Studio generator, not with ninja)
```
cmake --build . --config Release -- /M:%NUMBER_OF_PROCESSORS%
```
