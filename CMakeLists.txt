cmake_minimum_required(VERSION 3.9)
project(lab4)

set(CMAKE_C_STANDARD 11)

set(SOURCE_FILES source.cpp source.cpp)
add_executable(Lab1_monteCarlo ${SOURCE_FILES} source.cpp)

find_package(OpenMP)
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
set (CMAKE_EXE_LINKER_FLAGS "${CMAKE_EXE_LINKER_FLAGS} ${OpenMP_EXE_LINKER_FLAGS}")