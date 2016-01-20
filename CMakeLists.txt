cmake_minimum_required(VERSION 2.8)
INCLUDE(${CMAKE_SOURCE_DIR}/../build-scripts/CMakeDependencies.txt)

set(EXT_LIBS ${CSI_HTTP_SERVER_LIBS})

#compile a http parser library from third party source
ADD_LIBRARY(csi-http-parser STATIC ${HTTP_PARSER_PATH}/http_parser.h ${HTTP_PARSER_PATH}/http_parser.c)

add_subdirectory(csi_http_server)
add_subdirectory(samples)
