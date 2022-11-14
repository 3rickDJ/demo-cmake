cmake_minimum_required(VERSION 2.4)
set(CMAKE_CXX_STANDARD 17)

project(hello_world)

add_library(foo STATIC foo/Foo.cpp)
target_include_directories(foo PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/foo/include)

# file(GLOB_RECURSE SRC_FILES src/*.cpp)
add_executable (app main.cpp)
target_include_directories (app PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/include)
