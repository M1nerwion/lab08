cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(solver_app)

add_executable(solver_app equation.cpp)

target_link_libraries(solver_app formatter_ex solver)


