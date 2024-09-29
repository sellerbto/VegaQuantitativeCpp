cmake_minimum_required(VERSION 3.29)
project(VegaQuantitativeCPP)

set(CMAKE_CXX_STANDARD 20)

add_executable(VegaQuantitativeCPP src/main.cpp)

enable_testing()
add_subdirectory(tests)
add_subdirectory(benchmarks)