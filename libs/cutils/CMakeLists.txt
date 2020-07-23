
project(libcutil)


set(SRC_FILES
    ashmem-dev.c
    atomic.c
    native_handle.c
    process_name.c
    properties.c 
    safe_iop.c 
    sched_policy.c 
    socket_inaddr_any_server.c 
    socket_local_client.c 
    socket_local_server.c 
    socket_loopback_client.c 
    socket_loopback_server.c 
    sockets.c 
    strlcpy.c 
    threads.c)

add_library(binder_cutils SHARED ${SRC_FILES})
install(TARGETS binder_cutils LIBRARY DESTINATION ${CMAKE_CURRENT_BINARY_DIR})