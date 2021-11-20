cmake_minimum_required(VERSION 3.19)

add_subdirectory(ext/json)
add_subdirectory(ext/xml)

add_library(forcedirected STATIC
        node.cpp layout.cpp fdl.cpp file-handler.cpp)

target_link_libraries(forcedirected json rapidxml)