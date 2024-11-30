cmake_minimum_required(VERSION 3.28)
project(simplewall)

set(CMAKE_CXX_STANDARD 17)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/src)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/routine)
file(GLOB source_c "src/*.c")
file(GLOB routine_c "routine/*.c")
add_executable(simplewall ${source_c} ${routine_c})
