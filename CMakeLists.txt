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
add_executable(ex11
	src/main.cpp
	#lib/dnaFindPattern.hpp
	#lib/dnaFindPattern.cpp
)
#target_include_directories(ex11 PUBLIC lib)
#target_link_libraries(ex11 dnaregex)

