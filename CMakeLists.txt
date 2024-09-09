cmake_minimum_required(VERSION 3.28)
project(rpg)

set(CMAKE_CXX_STANDARD 17)

set(SDL2_PATH "C:\\sdl\\x86_64-w64-mingw32")
find_package(SDL2 REQUIRED)
include_directories( ${SDL2_INCLUDE_DIR} )

add_executable(rpg main.cpp)

target_link_libraries(rpg ${SDL2_LIBRARY} )


