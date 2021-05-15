cmake_minimum_required(VERSION 3.8)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS  "${CMAKE_CXX_FLAGS} -Wall")


add_library(castr INTERFACE )

target_link_libraries(castr INTERFACE cast_media_player cast_channel avahi_wrapper 
                            castr_utils rlog rweb
                            ssl crypto dl  protobuf protobuf-lite
                            avahi-client avahi-common pthread)

