cmake_minimum_required(VERSION 3.10)

project(sdl_first)

add_executable(sdl-first src/main.cpp)

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

target_link_libraries(sdl-first ${SDL2_LIBRARIES})
