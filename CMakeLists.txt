cmake_minimum_required(VERSION 3.0.2)
project(hello)
#set(SRC_LIST main.c)
message(STATUS "This is binary dir " ${PROJECT_BINARY_DIR})
message(STATUS "This is soure dir " ${PROJECT_SOURCE_DIR})
#add_executable(hello ${SRC_LIST})

add_subdirectory(src)
add_subdirectory(rtc)


