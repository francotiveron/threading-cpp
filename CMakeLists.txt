project(cpp-threading LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(threading INTERFACE)
target_include_directories(threading INTERFACE include)
target_link_libraries(threading INTERFACE pthread)