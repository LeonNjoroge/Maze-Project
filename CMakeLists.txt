cmake_minimum_required(VERSION 3.0)
project(The Maze)

set(SDL2_INCLUDE_DIR "E:/Coding/SDL2/include")
set(SDL2_LIB_DIR "E:/Coding/SDL2/lib")

# Find SDL2
find_package(SDL2 REQUIRED)

include_directories(${SDL2_INCLUDE_DIR})

# Add your source files
set(SOURCES maze.c)

# Create the executable
add_executable(The_Maze ${SOURCES})

# Link SDL2 libraries
target_link_libraries(The_Maze ${SDL2_LIBRARIES})
