cmake_minimum_required (VERSION 2.8.12)
project (serivce_manager CXX)

include_directories(../libs/include)

enable_language(C)
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

add_executable(test binderAddInts.cpp testUtil.c)
target_link_libraries(test binder binder_cutils binder_utils pthread)

install(TARGETS test DESTINATION ${CMAKE_CURRENT_BINARY_DIR})