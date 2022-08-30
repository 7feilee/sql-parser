cmake_minimum_required(VERSION 3.12)
project(sqlparser LANGUAGES CXX)
cmake_policy(SET CMP0077 NEW)

set(sqlparser_SOURCE_ROOT ${CMAKE_CURRENT_SOURCE_DIR})
set(sqlparser_BINARY_ROOT ${CMAKE_CURRENT_BINARY_DIR})

add_subdirectory(src)
add_subdirectory(example)
