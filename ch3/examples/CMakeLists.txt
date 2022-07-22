cmake_minimum_required(VERSION 3.0)
project(ch3_examples)

set(CMAKE_CXX_FLAGS "-O3 -std=c++14")

include_directories("/usr/include/eigen3")
add_executable(coordinateTransform coordinateTransform.cpp)

find_package(Pangolin REQUIRED)
include_directories(${Pangolin_INCLUDE_DIRS})

include_directories("/usr/include/eigen3")
add_executable(plotTrajectory plotTrajectory.cpp)

target_link_libraries(plotTrajectory ${Pangolin_LIBRARIES})
