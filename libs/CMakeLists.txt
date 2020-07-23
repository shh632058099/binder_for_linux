
project(binder)

include_directories(./include)

enable_language(ASM)


set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -DHAVE_PTHREADS -DHAVE_SYS_UIO_H -DHAVE_ENDIAN_H -DHAVE_ANDROID_OS=1 -std=c++11")

add_subdirectory(binder)
add_subdirectory(cutils)
add_subdirectory(utils)

