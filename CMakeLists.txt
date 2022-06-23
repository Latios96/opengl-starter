cmake_minimum_required(VERSION 3.22)
project(glfw_starter)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(glfw)
include_directories("glfw/deps")

add_executable(glfw_starter tiny_obj_loader.h main.cpp )
target_link_libraries(glfw_starter glfw )