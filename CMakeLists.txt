 
set(PID_SOURCES PID_v1.cpp) 
add_library(Arduino-PID-Library STATIC ${PID_SOURCES})
target_link_libraries( Arduino-PID-Library mbed-os)

set(PID_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR} )
target_include_directories(Arduino-PID-Library PUBLIC ${PID_HEADER_DIR})