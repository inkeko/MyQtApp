
cmake_minimum_required(VERSION 3.16)
project(MyQtApp LANGUAGES CXX)

# Qt telepítési útvonal
set(CMAKE_PREFIX_PATH "C:/Qt/6.10.0/mingw_64")

# Kimeneti mappa az .exe-nek
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/dist")

# Qt modulok keresése
find_package(Qt6 REQUIRED COMPONENTS Widgets)

# Fő program
add_executable(MyQtApp main.cpp)
target_link_libraries(MyQtApp Qt6::Widgets)
