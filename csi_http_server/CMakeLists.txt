SET(LIB_SRCS
	utils/uri_pattern.h
    utils/uri_pattern.cpp
	connection.h
	connection.cpp
	reply.h
	reply.cpp
	request.h
    request.cpp
	server.h
	http_server.h
	http_server.cpp		
	http_connection.h			
	http_connection.cpp				
	https_server.h
	https_server.cpp				
	https_connection.h
	https_connection.cpp					
	)

add_library (csi-http-server STATIC ${LIB_SRCS})

