cmake_minimum_required(VERSION 3.16)
project(sql)

set(CMAKE_CXX_STANDARD 11)

add_executable(sql Part3/table.cpp Part2/compiler.cpp Part1/main.cpp Part4/Test.cpp Part5/persistence.cpp)