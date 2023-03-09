cmake_minimum_required(VERSION 3.23)
project(App)

set(CMAKE_CXX_STANDARD 14)

include_directories(
        ../patterns/include
)

link_directories(
        patterns
)

add_executable(App main.cpp)

target_link_libraries(App patterns)
