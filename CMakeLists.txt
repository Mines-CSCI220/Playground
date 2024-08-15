# CMakeLists.txt

# This configuration file informs the CMake tool how to build
# software in this directory.  We will use CMake to generate a 
# Makefile for each project, but it can be used in other ways 
# as well. Learn more here: https://cmake.org/getting-started/

# Re-run CMake whenever you modify this file.

cmake_minimum_required(VERSION 3.14)

# Ensure we can use gdb
set(CMAKE_BUILD_TYPE Debug)

project(playground)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

# These options turn on additional warnings to help detect
# potential problems in your code.
add_compile_options(-pedantic -Wall -Wextra)

# This line says that our code produces a program named "run-main"
# from the source code in main.cpp.  You can add additional source
# files and header files after main.cpp, e.g.,
# "add_executable(run-main main.cpp foo.h foo.cpp)"
add_executable(run-main main.cpp)
