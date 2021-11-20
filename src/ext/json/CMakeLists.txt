cmake_minimum_required(VERSION 3.19)

add_library(json STATIC config.h autolink.h config.h features.h forwards.h
        json.h reader.h value.h writer.h json_reader.cpp json_value.cpp
        json_writer.cpp)