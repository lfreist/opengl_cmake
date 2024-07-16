cmake_minimum_required(VERSION 3.1)
project(opengl_cmake)

set(CMAKE_CXX_STANDARD 23)

include_directories(include)

add_subdirectory(external/glfw)
include_directories(external/glfw/include)

add_library(glad external/glad/src/glad.c)
include_directories(external/glad/include)

add_subdirectory(app)
add_subdirectory(src)
