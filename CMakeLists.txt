cmake_minimum_required(VERSION 3.11)
project(hello)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wpedantic -Wextra -Wunused -pthread")

add_executable(hello hello.cpp)
