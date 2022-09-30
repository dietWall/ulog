cmake_minimum_required(VERSION 3.5)

add_subdirectory(src)

include(CMakePrintHelpers)

message(STATUS "Main ulog cmake")
cmake_print_variables(ULOG_ENABLED)

if(${CMAKE_SYSTEM_NAME} STREQUAL "Linux" OR "Windows")
	add_subdirectory(tests)
endif()

