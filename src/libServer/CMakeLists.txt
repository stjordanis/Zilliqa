add_library(Server Server.cpp JSONConversion.cpp)
target_include_directories(Server PUBLIC ${PROJECT_SOURCE_DIR}/src)
target_link_libraries (Server PUBLIC AccountData ${JSONCPP_LINK_TARGETS} ${JSONRPCCPP_LINK_TARGETS})
