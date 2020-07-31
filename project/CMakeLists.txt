cmake_minimum_required(VERSION 3.1)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

project(data-augmentation)

find_package(OpenCV REQUIRED)

add_executable(data-augmentation data-augmentation.cpp)

target_link_libraries(data-augmentation ${OpenCV_LIBS})
