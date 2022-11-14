add_library(my_library SHARED
    foo.h
    foo.cpp
    )
target_include_directories(my_library PUBLIC
    ${CMAKE_CURRENT_LIST_DIR})
