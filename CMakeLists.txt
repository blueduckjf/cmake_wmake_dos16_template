cmake_minimum_required(VERSION 3.26)

set(CMAKE_C_STANDARD 99)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

project(cmake_wmake_dos16_template C)

set(SRC_DIR ${CMAKE_CURRENT_LIST_DIR}/src)

set(SOURCES
    "${SRC_DIR}/main.c"
)
add_executable(cmake_wmake_dos16_template ${SOURCES})

target_include_directories(cmake_wmake_dos16_template
    PUBLIC "${CMAKE_CURRENT_LIST_DIR}/include"
)
