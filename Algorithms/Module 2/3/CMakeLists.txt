cmake_minimum_required(VERSION 3.5)
project(Ads)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -static -Wall -std=gnu++11 -lm")

set(SOURCE_FILES main.cpp)
add_executable(Ads ${SOURCE_FILES})
