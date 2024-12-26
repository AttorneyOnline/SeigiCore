cmake_minimum_required(VERSION 3.14)

project(SeigiCore LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(SeigiCore SHARED
  SeigiCore_global.h
  seigi.cpp
  seigi.h
)

target_compile_definitions(SeigiCore PRIVATE SEIGICORE_LIBRARY)
