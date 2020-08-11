project(mua)

cmake_minimum_required(VERSION 3.16)

find_package(GTest)

enable_testing()

#-------------------------------------------------------------------------------
set(CXX_FLAGS
    -g
    -std=c++20
    -rdynamic
    )
string(REPLACE ";" " " CMAKE_CXX_FLAGS "${CXX_FLAGS}")
#-------------------------------------------------------------------------------
add_subdirectory(src)