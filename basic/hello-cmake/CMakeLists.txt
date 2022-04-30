# Set the minimum version of CMake that can be used to find the cmake version run
# cmake --version
cmake_minimum_required(VERSION 3.22)

# Set the project name.
project(hello_cmake)

# Add an executable.
# ${} inserts the variable value.
add_executable(${PROJECT_NAME} main.cpp)
