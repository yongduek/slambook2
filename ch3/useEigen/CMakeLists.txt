# https://www.google.com/search?q=vscode+cmake+c%2B%2B+how+to+build&oq=vscode+cmake+c%2B%2B+how+to+build&aqs=chrome..69i57j0i22i30.15689j0j4&sourceid=chrome&ie=UTF-8#kpvalbx=_-AraYoSzKcfQ2roP0qe-qAs30

cmake_minimum_required(VERSION 3.1)
project(useEigen)

# set(CMAKE_BUILD_TYPE "Debug")
# set(CMAKE_BUILD_TYPE "Release")
set(CMAKE_CXX_FLAGS "-O3 -std=c++14")

message("Generated with config types: ${CMAKE_CONFIGURATION_TYPES}")

# 添加Eigen头文件
include_directories("/usr/include/eigen3")
add_executable(eigenMatrix eigenMatrix.cpp)
