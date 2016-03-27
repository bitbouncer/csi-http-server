cmake_minimum_required(VERSION 2.8.1)
include_directories(${CSI_INCLUDE_PATH} ${CMAKE_SOURCE_DIR})
add_subdirectory(csi_http_server)
add_subdirectory(samples)
