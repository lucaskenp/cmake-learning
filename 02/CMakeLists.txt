cmake_minimum_required(VERSION 3.5)
project(testsome)
add_executable(${PROJECT_NAME} main.cpp)
add_subdirectory(Adder)
add_subdirectory(${CMAKE_SOURCE_DIR}/../external/glfw out/build)
target_include_directories(${PROJECT_NAME} PUBLIC Adder)
target_link_directories(${PROJECT_NAME} PRIVATE Adder)
target_link_libraries(${PROJECT_NAME} adder)

