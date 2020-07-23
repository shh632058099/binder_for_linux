cmake_minimum_required (VERSION 2.8.12)
project (serivce_manager CXX)

include_directories(../libs/include)

enable_language(C)
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

add_executable(serivce_manager service_manager.c binder.c)

install(TARGETS serivce_manager DESTINATION ${CMAKE_CURRENT_BINARY_DIR})