cmake_minimum_required(VERSION 3.10)
project(MyProject)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_BUILD_TYPE Debug)

add_executable(TF_256 main.cpp)
target_link_libraries(TF_256 PRIVATE z)
find_package(Threads REQUIRED)
target_link_libraries(TF_256 PRIVATE Threads::Threads)

