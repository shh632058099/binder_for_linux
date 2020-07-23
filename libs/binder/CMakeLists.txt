
project(libbinder)

include_directories(./include)
include_directories(../libutils/include)


set(SRC_FILES
    AppOpsManager.cpp
    Binder.cpp
    BpBinder.cpp
    BufferedTextOutput.cpp
    Debug.cpp
    IAppOpsCallback.cpp
    IAppOpsService.cpp
    IBatteryStats.cpp
    IInterface.cpp
    IMemory.cpp
    IPCThreadState.cpp
    IPermissionController.cpp
    IServiceManager.cpp
    MemoryBase.cpp
    MemoryDealer.cpp
    MemoryHeapBase.cpp
    Parcel.cpp
    PermissionCache.cpp
    ProcessInfoService.cpp
    ProcessState.cpp
    Static.cpp
    TextOutput.cpp
    IProcessInfoService.cpp)

add_library(binder SHARED ${SRC_FILES})
install(TARGETS binder LIBRARY  DESTINATION ${CMAKE_CURRENT_BINARY_DIR})