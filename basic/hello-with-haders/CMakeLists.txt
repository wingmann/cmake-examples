# Set the minimum version of CMake that can be used to find the cmake version run
# $ cmake --version
cmake_minimum_required(VERSION 3.22)

# Set the project name
project(hello_headers)

# Create a sources variable with a link to all cpp files to compile
set(PROJECT_SOURCES src/hello.cpp src/main.cpp)

# Add an executable with the above sources
add_executable(${PROJECT_NAME} ${PROJECT_SOURCES})

# Set the directories that should be included in the build command for this target when running g++
# these will be included as -I/directory/path/
target_include_directories(${PROJECT_NAME} PRIVATE
    ${PROJECT_SOURCE_DIR}/include)
