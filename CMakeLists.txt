cmake_minimum_required(VERSION 2.8)
project(hello_world CXX)

set(CMAKE_CXX_FLAGS "-std=c++11 -Wextra -Wall -pedantic")

set(CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}")

add_custom_target(all_examples)

find_package(CAF COMPONENTS core io REQUIRED)

include_directories(${CAF_INCLUDE_DIRS})


add_executable(hello_world hello_world.cpp ${ARGN})
target_link_libraries(hello_world ${CAF_LIBRARIES})



