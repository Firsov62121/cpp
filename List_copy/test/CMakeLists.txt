cmake_minimum_required(VERSION 3.8)

set(This ListCopyTests)

set(Sources 
    ListCopyTests.cpp    
)

add_executable(${This} ${Sources})
target_link_libraries(${This} PUBLIC
    gtest_main
    List_copy
)

add_test(
    Name ${This}
    COMMAND ${This}
)