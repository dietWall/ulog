# Set the project name
project(ulog)

# Add a library with the above sources
add_library(${PROJECT_NAME} EXCLUDE_FROM_ALL ulog.c)

include(CMakePrintHelpers)

message(STATUS "Main ulog cmake")
cmake_print_variables(ULOG_ENABLED)


target_include_directories(${PROJECT_NAME} PUBLIC .)
