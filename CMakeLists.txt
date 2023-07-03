## 'Google_test' is the subproject name
#project(Google_tests)
#
## 'lib' is the folder with Google Test sources
#add_subdirectory(lib)
#include_directories(${gtest_SOURCE_DIR}/include ${gtest_SOURCE_DIR})
#
## 'Google_Tests_run' is the target name
## 'test1.cpp tests2.cpp' are source files with tests
#add_executable(Google_Tests_run BlackBoxTest.cpp)
#target_link_libraries(Google_Tests_run gtest gtest_main)

cmake_minimum_required(VERSION 3.21)
project(Kosaraju-Sharir-Rebuilt)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(Google_tests)

add_executable(Kosaraju-Sharir-Rebuilt main.cpp
        adjacency_list.h adjacency_list.cpp
        AlgoKS.cpp AlgoKS.cpp
        KosarajuSharir.cpp KosarajuSharir.h
        LinkedList.cpp LinkedList.h
        Node.cpp Node.h
        read_file.cpp read_file.h
        Stack.cpp Stack.h
        )
