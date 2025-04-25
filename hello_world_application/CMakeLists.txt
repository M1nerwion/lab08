cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(hello_app)

add_executable(main hello_world.cpp)

target_link_libraries(main formatter_ex)

