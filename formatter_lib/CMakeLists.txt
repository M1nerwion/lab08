cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(format_lib)

add_library(formatter STATIC formatter.cpp)# Создание статической библиотеки с именем formatter

target_include_directories(formatter PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})