cmake_minimum_required(VERSION 3.10)

include(CTest)

include(FetchContent)


FetchContent_Declare(
  Catch2
  GIT_REPOSITORY https://github.com/catchorg/Catch2.git
  GIT_TAG v3.2.1)

FetchContent_MakeAvailable(Catch2)

include(Catch)

add_subdirectory(cpp_catch2_unittest)
add_subdirectory(cpp_texttest)
