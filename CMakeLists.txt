cmake_minimum_required(VERSION 3.2)
project(TinyVGM)

set(CMAKE_C_STANDARD 99)

add_library(TinyVGM TinyVGM.c TinyVGM.h)
target_include_directories(TinyVGM INTERFACE .)

add_executable(TinyVGM_Example example.c)
target_link_libraries(TinyVGM_Example TinyVGM)
