
project(libutil)

set(SRC_FILES
    BasicHashtable.cpp 
    BlobCache.cpp 
    CallStack.cpp 
    FileMap.cpp 
    JenkinsHash.cpp 
    LinearTransform.cpp 
    Log.cpp 
    Looper.cpp 
    misc.cpp 
    NativeHandle.cpp 
    Printer.cpp 
    ProcessCallStack.cpp 
    PropertyMap.cpp 
    RefBase.cpp 
    SharedBuffer.cpp 
    Static.cpp 
    StopWatch.cpp 
    String16.cpp 
    String8.cpp 
    SystemClock.cpp 
    Threads.cpp 
    Timers.cpp 
    Tokenizer.cpp 
    Unicode.cpp 
    VectorImpl.cpp)

add_library(binder_utils SHARED ${SRC_FILES})
install(TARGETS binder_utils LIBRARY DESTINATION ${CMAKE_CURRENT_BINARY_DIR})