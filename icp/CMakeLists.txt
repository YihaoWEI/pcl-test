cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
project(pcl-icp)
find_package(PCL 1.2 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS})
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

add_executable(pcl-icp main.cpp)
target_link_libraries(pcl-icp ${PCL_LIBRARIES})

SET(COMPILE_FLAGS "-std=c++11")
add_definitions(${COMPILE_FLAGS})
