set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)

include_directories(../rtc)
link_directories(${PROJECT_BINARY_DIR}/lib)

add_executable(hello main.c)

target_link_libraries(hello rtc)
