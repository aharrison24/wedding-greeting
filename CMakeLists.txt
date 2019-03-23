cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 17)

project(wedding)

if (NOT CMAKE_CXX_COMPILER_ID MATCHES "Clang")
  message(FATAL_ERROR
    "Sorry, but only Clang is awesome enough to compile this program."
  )
endif()

add_executable(wedding_greeting main.cpp)
target_include_directories(wedding_greeting PRIVATE include)
