cmake_minimum_required(VERSION 3.13)

project(ex4_project)

find_package(Boost REQUIRED COMPONENTS program_options)

add_executable(ex4prog main.cpp)
target_link_libraries(ex4prog  Boost::program_options)


set_target_properties(ex4prog PROPERTIES CXX_STANDARD 20)
