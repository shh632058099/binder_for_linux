
project(binder)


set(CMAKE_CXX_FLAGS " -std=c++11")

add_subdirectory(libs)
add_subdirectory(servicemanager)
add_subdirectory(test)

