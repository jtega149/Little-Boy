cmake_minimum_required(VERSION 3.20)

project(littleboy CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

add_compile_options(-Wall -Wextra -Wpedantic)

add_library(littleboy src/tensor.cpp)
target_include_directories(littleboy PUBLIC include)

add_executable(littleboy_main src/main.cpp)
target_link_libraries(littleboy_main PRIVATE littleboy)