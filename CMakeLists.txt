cmake_minimum_required (VERSION 3.1)

project(decr)

add_library(decr STATIC IMPORTED)

set_property(TARGET decr PROPERTY IMPORTED_LOCATION
  ${CMAKE_SOURCE_DIR}/lib64/libdecr.a)

include_directories(${CMAKE_SOURCE_DIR}/include)
