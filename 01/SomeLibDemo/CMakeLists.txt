cmake_minimum_required(VERSION 3.5)

project(mathadd)

add_library(mathadd adder.cpp)

set_target_properties(mathadd PROPERTIES PUBLIC_HEADER adder.h)

install(TARGETS mathadd LIBRARY DESTINATION lib 
        PUBLIC_HEADER DESTINATION include
        )