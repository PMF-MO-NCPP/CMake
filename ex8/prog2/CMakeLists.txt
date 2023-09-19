cmake_minimum_required(VERSION 3.13)
project(fmt_test_2)

include(FetchContent)
FetchContent_Declare(
  fmt
  GIT_REPOSITORY https://github.com/fmtlib/fmt
  GIT_TAG   10.1.1
)
FetchContent_MakeAvailable(fmt)

add_executable(fmt_2 main.cpp)
target_link_libraries(fmt_2 PRIVATE fmt::fmt-header-only)
