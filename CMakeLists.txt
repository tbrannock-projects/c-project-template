cmake_minimum_required(VERSION 3.10)

# Get the name of the current directory and use it as the project name
get_filename_component(PROJECT_NAME ${CMAKE_CURRENT_SOURCE_DIR} NAME)
project(${PROJECT_NAME} VERSION 1.0)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Set C standard
set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED True)

# Define the source files to compile
set(SOURCES
    src/main.cpp
)

add_executable(${PROJECT_NAME} ${SOURCES})