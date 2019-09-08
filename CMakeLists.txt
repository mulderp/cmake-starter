cmake_minimum_required(VERSION 3.0)

project(runner)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib") 
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")

# the -I flag in gcc
include_directories(
  ${PROJECT_SOURCE_DIR}/include/
) 

add_subdirectory(src)
