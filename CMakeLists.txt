cmake_minimum_required(VERSION 3.0)

set(PROJECT_NAME DataStructure)

project(${PROJECT_NAME})

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${PROJECT_SOURCE_DIR}/bin)

set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory("Chapter2")
