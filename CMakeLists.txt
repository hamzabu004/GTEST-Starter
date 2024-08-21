cmake_minimum_required(VERSION 3.29)
project(Gtest_Proj)

set(CMAKE_CXX_STANDARD 20)


add_subdirectory(googletest)
include_directories(googletest/include)  # Include the Google Test headers


add_executable(Gtest_Proj main.cpp)

target_link_libraries(Gtest_Proj gtest gtest_main)  # Link Google Test libraries
