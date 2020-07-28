cmake_minimum_required(VERSION 3.10.2)
project(l06-bytes)
set(CMAKE_CXX_STANDARD 17)

find_package(X11)
find_package (Threads)
link_libraries(${CMAKE_THREAD_LIBS_INIT} )
link_libraries(${X11_LIBRARIES})

add_executable(l06-bytes ../main.cpp)