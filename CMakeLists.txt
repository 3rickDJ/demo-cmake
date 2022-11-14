cmake_minimum_required(VERSION 2.4)
set(CMAKE_CXX_STANDARD 17)

project(hello_world)
add_subdirectory(my_library)
add_executable (Hello main.cpp)
target_link_libraries(Hello
    my_library)
