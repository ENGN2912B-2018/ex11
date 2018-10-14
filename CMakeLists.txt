cmake_minimum_required (VERSION 3.2)

# compiler settings
set(CMAKE_CXX_COMPILER "g++")

# create the project (must have a name)
project (ex11_stl)

# add compiler flags
set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -p -Wall")
set(CMAKE_CXX_FLAGS_RELEASE "${CMAKE_CXX_FLAGS_RELEASE} -Wall")

# invoke library CMakeLists.txt
#add_subdirectory(lib)

# create the executable
#include_directories(src lib)
add_executable(ex11p1 src/main1.cpp)
add_executable(ex11p2 src/main2.cpp)
