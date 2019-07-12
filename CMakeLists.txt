cmake_minimum_required(VERSION 2.8)

message("--->Cmake imgui--->")

project(imgui)
include_directories(.)

FILE(GLOB SRC_IMGUI "${CMAKE_CURRENT_SOURCE_DIR}/*.cpp" "${CMAKE_CURRENT_SOURCE_DIR}/*.h")

add_library(imgui STATIC ${SRC_IMGUI})

target_include_directories(imgui PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})