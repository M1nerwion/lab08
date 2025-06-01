cmake_minimum_required(VERSION 3.25.1)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(itog)

add_subdirectory(formatter_lib)
add_subdirectory(formatter_ex_lib)
add_subdirectory(hello_world_application)
add_subdirectory(solver_lib)
add_subdirectory(solver_application)

set(CPACK_PACKAGE_NAME "Lab06")
set(CPACK_PACKAGE_VERSION "1.0.0")
set(CPACK_DEBIAN_PACKAGE_MAINTAINER "M1nerwion")
set(CPACK_GENERATOR DEB RPM WIX DragNDrop TGZ ZIP)
include(CPack)
