cmake_minimum_required(VERSION 3.24)
project(threads)

set(CMAKE_CXX_STANDARD 20)

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

add_compile_options(-Wall -Wextra -pedantic -Werror)

add_executable(threads main.cpp)
target_link_libraries(threads PRIVATE Threads::Threads)
