# CMake 最低版本号要求
cmake_minimum_required (VERSION 2.8)

# 项目信息
project (logTest)
SET(CMAKE_C_COMPILER g++)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)
set(CMAKE_CXX_FLAGS -pthread)
message(STATUS "CMAKE_CXX_FLAGS = ${CMAKE_CXX_FLAGS}")
#link_libraries(ssl)
# 指定生成目标
add_executable(logTest logTest.cpp logger.cpp)
#target_link_libraries(ssl)