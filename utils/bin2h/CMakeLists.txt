cmake_minimum_required(VERSION 3.0.2)
project(bin2h)
add_executable(bin2h bin2h.c)
# Enforce no dressing for executable names, so the main script can find it
set_target_properties(bin2h PROPERTIES OUTPUT_NAME bin2h)
