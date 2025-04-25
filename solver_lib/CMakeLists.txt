cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(solver_lib)

add_library(solver STATIC solver.cpp)# Создание статической библиотеки с именем solver

target_include_directories(solver PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})