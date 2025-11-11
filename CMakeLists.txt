cmake_minimum_required(VERSION 3.16)
project(MyQtApp)

set(CMAKE_PREFIX_PATH "C:/Qt/6.10.0/mingw_64")

find_package(Qt6 REQUIRED COMPONENTS Widgets)

add_executable(MyQtApp main.cpp)
target_link_libraries(MyQtApp Qt6::Widgets)