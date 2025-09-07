cmake_minimum_required(VERSION 3.15)

project(NpOscProtocol VERSION 1.0 LANGUAGES CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Create a header-only interface library
add_library(NpOscProtocol INTERFACE)

# Specify the include directories
target_include_directories(NpOscProtocol INTERFACE
    $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/src>
)