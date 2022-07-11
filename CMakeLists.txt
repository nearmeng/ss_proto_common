cmake_minimum_required (VERSION 3.20)

SET(TARGET_NAME "ss_proto_common")
project(${TARGET_NAME})

add_library(${TARGET_NAME} INTERFACE)
add_library(mango::${TARGET_NAME} ALIAS ${TARGET_NAME})

target_include_directories(${TARGET_NAME} INTERFACE .)
#target_link_libraries(${TARGET_NAME} INTERFACE rstudio::util_define)