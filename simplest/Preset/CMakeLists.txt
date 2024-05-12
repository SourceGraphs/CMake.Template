cmake_minimum_required(VERSION 3.0.0)
project(firstapp VERSION 0.1.0 LANGUAGES C CXX)

include(CTest)
enable_testing()

add_executable(firstapp main.cpp)

set_property(TARGET firstapp PROPERTY CXX_STANDARD 17)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
