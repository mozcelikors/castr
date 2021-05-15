cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -Wall")

include_directories( ./include )

add_library(rlog STATIC RLog.cxx)

target_include_directories(rlog INTERFACE 
                           ${CMAKE_CURRENT_SOURCE_DIR}/include )
