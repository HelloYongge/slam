cmake_minimum_required( VERSION 2.8 )

project( HelloSLAM )

include_directories( "include" )

add_library( libHello src/hello.cpp )

add_executable( sayHello main.cpp )

target_link_libraries( sayHello libHello )