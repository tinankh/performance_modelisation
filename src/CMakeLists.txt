
#However, the file(GLOB...) allows for wildcard additions:
file(GLOB SOURCES "*.c")


#include_directories(${CMAKE_SOURCE_DIR}/include)
#add_executable(main_programme mainapp.c misc.c)
#add_library(lib_misc misc.cxx)


#add_executable(tool_kernel_generator tool_kernel_generator.c misc.c)
#add_executable(tool_cacheLineSize tool_cacheLineSize.c misc.c)
#add_executable(tool_cacheSize tool_cacheSize.c misc.c)



# CHANGE THIS
add_subdirectory (tool_hw_description)
add_subdirectory (tool_kernel_generator)
add_subdirectory (tool_oprofile)
add_subdirectory (common)
add_subdirectory (benchmark_multiply)
add_subdirectory (tool_monitoring_bandwidth)
