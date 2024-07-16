# OpenGL CMake Projekt
Simple project setup using OpenGL, C++ and CMake

## Prerequisites
- git
- C++ compiler: gcc, clang, msvc
- OpenGL runtime
- CMake

## Initialize
```bash
git clone https://github.com/lfreist/opengl_cmake.git
git submodule update --init --recursive
```

## build
```bash
mkdir build
cmake -B build
cmake --build build --config Release
```
This builds an executable (from `app/main.cpp`) in `build/app/Release/`

## Run
```bash
cd build/app/Release
./main
```