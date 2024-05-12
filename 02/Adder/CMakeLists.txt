cmake_minimum_required(VERSION 3.5)

project(adder)

add_library(${PROJECT_NAME} adder.cpp)

set_target_properties(${PROJECT_NAME} PROPERTIES PUBLIC_HEADER adder.h)

#install(TARGETS Adder LIBRARY DESTINATION lib 
#        PUBLIC_HEADER DESTINATION include
#        )