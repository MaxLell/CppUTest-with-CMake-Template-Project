cmake_minimum_required(VERSION 3.16.2 FATAL_ERROR)

project(MyProject LANGUAGES CXX)

add_executable(MultiFiles Main.cpp)

add_subdirectory(lib)

target_link_libraries(MultiFiles PRIVATE MathLib MyUtils)
