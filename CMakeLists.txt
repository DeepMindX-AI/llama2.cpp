# This file handles building each task as sub-project.
#
# Each task becomes an independent project in which you can experiment.
#
# Tasks are added as separate sub-projects so as compilation errors in
# one task don't affect another task.
project(llama2.cpp)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_FLAGS "$ENV{CXXFLAGS} -O3 -Wall")

add_executable(run run.cpp)
add_executable(runq runq.cpp)