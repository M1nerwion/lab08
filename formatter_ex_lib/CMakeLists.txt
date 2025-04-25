cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(format_ex_lib)

add_library(formatter_ex STATIC formatter_ex.cpp)

target_link_libraries(formatter_ex formatter)

target_include_directories(formatter_ex PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
