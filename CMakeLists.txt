 
set(PID_SOURCES PID_v1.cpp) 
add_library(mbed_PID_Library STATIC ${PID_SOURCES})
target_link_libraries( mbed_PID_Library mbed-os)

set(PID_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR} )
target_include_directories(mbed_PID_Library PUBLIC ${PID_HEADER_DIR})