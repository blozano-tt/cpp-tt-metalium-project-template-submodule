cmake_minimum_required(VERSION 3.22)

project(hello_world LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)

add_subdirectory(tt-metal)

add_executable(hello_world_compute_kernel)
target_sources(hello_world_compute_kernel PRIVATE src/hello_world_compute_kernel.cpp)
target_link_libraries(hello_world_compute_kernel PRIVATE TT::Metalium)
