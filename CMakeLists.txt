cmake_minimum_required(VERSION 3.10)

project(Polylla CXX)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenMP REQUIRED)

add_subdirectory(src)

add_executable(Polylla main.cpp)

target_compile_options(Polylla PRIVATE -O3)
target_link_libraries(Polylla PRIVATE meshfiles OpenMP::OpenMP_CXX)
