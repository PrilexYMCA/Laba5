cmake_minimum_required(VERSION 3.10)
project(tourist)

set(CMAKE_CXX_STANDARD 17)

add_executable(tourist tourist.cpp)

find_package(GTest REQUIRED)
include_directories(${GTEST_INCLUDE_DIRS})
target_link_libraries(your_target_name ${GTEST_LIBRARIES} pthread)
