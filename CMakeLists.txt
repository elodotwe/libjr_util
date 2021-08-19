cmake_minimum_required(VERSION 3.20)

project(jr_util)

add_library(jr_util STATIC jr_hex_print.c jr_hex_print.h)
target_include_directories(jr_util PUBLIC .)
set(CMAKE_C_STANDARD 11)
set(CMAKE_C_STANDARD_REQUIRED ON)
# include(FindPkgConfig)
# pkg_search_module(OPUSFILE REQUIRED opusfile)
# include_directories(${OPUSFILE_INCLUDE_DIRS})
# target_link_libraries(${PROJECT_NAME} ${OPUSFILE_LIBRARIES})
set(CMAKE_BUILD_TYPE Debug)