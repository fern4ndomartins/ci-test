cmake_minimum_required(VERSION 3.16)
project(MyDistSys)

set(CMAKE_CXX_STANDARD 20)

add_executable(app src/main.cc)

add_executable(test_main tests/test_main.cc)
enable_testing()
add_test(NAME test_main COMMAND test_main)

