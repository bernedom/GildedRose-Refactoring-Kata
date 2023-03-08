cmake_minimum_required(VERSION 3.13)
project(gilded-rose-refactoring-kata-cpp)

include(CTest)

# uncomment this line to enable coverage measurements using gcov
# set(CMAKE_CXX_FLAGS "--coverage")



add_library(GildedRose)
target_sources(GildedRose PRIVATE src/GildedRose.cc)
target_include_directories(GildedRose PUBLIC src)

add_subdirectory(test)
