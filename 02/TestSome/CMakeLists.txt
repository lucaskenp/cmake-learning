cmake_minimum_required(VERSION 3.5)
project(testsome)
add_executable(${PROJECT_NAME} main.cpp)
#target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_SOURCE_DIR}/../Adder)
target_link_directories(${PROJECT_NAME} PRIVATE ${CMAKE_SOURCE_DIR}/../Adder/build)
target_link_libraries(${PROJECT_NAME} adder)

