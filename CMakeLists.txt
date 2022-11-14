cmake_minimum_required(VERSION 2.4)
project(hello_world)
add_subdirectory(my_library)
add_executable (Hello main.cpp)
target_link_libraries(Hello
    my_library)
