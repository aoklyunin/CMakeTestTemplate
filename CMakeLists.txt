cmake_minimum_required(VERSION 3.23)
project(CppPatterns)

set(CMAKE_CXX_STANDARD 14)

enable_testing()

add_subdirectory(patterns)
include_directories(patterns/include)

add_subdirectory(app)