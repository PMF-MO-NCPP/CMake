cmake_minimum_required(VERSION 3.13)

project(ex5_project CXX)
enable_testing()

# Compilation of googletest library #####
include(FetchContent)
FetchContent_Declare(
  googletest
  GIT_REPOSITORY https://github.com/google/googletest.git
  GIT_TAG     v1.14.0
)
# For Windows: Prevent overriding the parent project's compiler/linker settings
set(gtest_force_shared_crt ON CACHE BOOL "" FORCE)
FetchContent_MakeAvailable(googletest)
##########################################

add_subdirectory("src")
add_subdirectory("test")
