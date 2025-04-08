# Minimum required CMake Version for compatibility
cmake_minimum_required(VERSION 3.30)

# Project name
project(oop_sample)

# Set the C++ standard to C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS ON)

# Include the directories containing the header files
include_directories(${PROJECT_SOURCE_DIR}/include)

# Source files
set(SOURCES
        main.cpp)

# Define the executable target
add_executable(oop_sample main.cpp
        src/Resource.cpp
        src/ConsumableResource.cpp)
