cmake_minimum_required(VERSION 3.13)
project(fmt_test_1)

find_package(fmt REQUIRED)
add_executable(fmt_1 main.cpp)
target_link_libraries(fmt_1 PRIVATE fmt::fmt-header-only)
