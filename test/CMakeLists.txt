enable_testing()
find_package(Check REQUIRED)
include_directories(${CHECK_INCLUDE_DIRS})
set(LIBS ${LIBS} ${CHECK_LIBRARIES} ma_lib)
include_directories(. ../include)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/test)
add_executable(test_ma_lib test_ma_lib.c)
target_link_libraries(test_ma_lib ${LIBS})
add_test(test_ma_lib ${CMAKE_CURRENT_BINARY_DIR}/test_ma_lib)


