cmake_minimum_required(VERSION 3.16)

project(Gene)
add_executable(${PROJECT_NAME} "demo_main.cpp")
set(lib_DIR /usr/lib/x86_64-linux-gnu)
set(CMAKE_BUILD_TYPE "Debug")
set(CMAKE_CXX_FLAGS_DEBUG "$ENV{CXXFLAGS} -O0 -Wall -g2 -ggdb")
link_directories(${lib_DIR})
target_link_libraries(Gene libjsoncpp.a)
