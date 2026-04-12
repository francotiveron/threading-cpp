cmake_minimum_required(VERSION 3.20)
project(threading-cpp LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(threading INTERFACE)
target_include_directories(threading INTERFACE include)
target_link_libraries(threading INTERFACE pthread)
