cmake_minimum_required(VERSION 3.0)
project(base-master C)
set(CMAKE_C_STANDARD 99)

file(GLOB_RECURSE SOURCE "src/*.c" "src/*.h")
add_executable(base-master "${SOURCE}")

include_directories("/usr/include/SDL2")
target_link_libraries(base-master m SDL2 SDL2_gfx)
