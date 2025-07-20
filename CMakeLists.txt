cmake_minimum_required(VERSION 3.15)
project(Snake VERSION 1.0) 

find_package(ZLIB REQUIRED)
find_package(GLFW3 REQUIRED)

message("Building with CMake vesrion: ${CMAKE_VERSION}")

add_executable(${PROJECT_NAME} src/main.cpp)
target_link_libraries(${PROJECT_NAME} ZLIB::ZLIB glfw)
