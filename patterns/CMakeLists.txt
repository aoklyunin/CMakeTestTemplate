cmake_minimum_required(VERSION 3.23)
project(patterns)


set(CMAKE_CXX_STANDARD 14)

include_directories(
        include
)

add_library(
        ${PROJECT_NAME}
        src/patterns.cpp
)

add_executable(SumTest tests/sumTest.cpp)
target_link_libraries(SumTest  ${PROJECT_NAME})
add_test(NAME SumTest COMMAND SumTest)

