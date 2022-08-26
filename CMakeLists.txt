cmake_minimum_required(VERSION 3.13)

project( test_cmake CXX )

add_subdirectory( mod1 )
add_subdirectory( mod2 )
add_executable( a.out main.cpp )
target_link_libraries( a.out Mod1 Mod2 )