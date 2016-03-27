project(avro_http_server_sample)

SET(SRCS
avro_http_server_sample.cpp

)

add_executable(avro_http_server_sample ${SRCS})
target_link_libraries(avro_http_server_sample csi-http-server csi-http-common csi-avro  ${CSI_BOOST_LIBS})
