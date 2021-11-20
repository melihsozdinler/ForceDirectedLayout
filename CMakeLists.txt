cmake_minimum_required(VERSION 3.19)
project(force_run)
set(CMAKE_VERBOSE_MAKEFILE ON)
set(CMAKE_CXX_STANDARD 17)

add_subdirectory(src)
add_executable(force_run src/fdl.cpp)
target_link_libraries(force_run forcedirected json rapidxml)