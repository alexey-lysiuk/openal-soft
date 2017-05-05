cmake_minimum_required(VERSION 3.0.2)
project(bin2h)
set(CMAKE_BUILD_TYPE Release)
add_executable(bin2h bin2h.c)
# Enforce no dressing for executable names, so the main script can find it
set_target_properties(bin2h PROPERTIES OUTPUT_NAME bin2h)
set_target_properties(bin2h PROPERTIES RUNTIME_OUTPUT_DIRECTORY_Release "${CMAKE_BINARY_DIR}")
message(STATUS "CMAKE_BINARY_DIR = ${CMAKE_BINARY_DIR}")
