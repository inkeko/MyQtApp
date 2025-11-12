cmake_minimum_required(VERSION 3.16)
project(MyQtApp LANGUAGES CXX)


set(CMAKE_PREFIX_PATH "C:/Qt/6.10.0/mingw_64")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/dist")


find_package(Qt6 REQUIRED COMPONENTS Widgets)

add_executable(MyQtApp main.cpp)
target_link_libraries(MyQtApp Qt6::Widgets)
