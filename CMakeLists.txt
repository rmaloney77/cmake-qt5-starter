cmake_minimum_required(VERSION 2.8.11)

set(CMAKE_AUTOMOC ON)
set(CMAKE_PREFIX_PATH "/opt/QT/5.4/gcc_64")
set(CMAKE_INCLUDE_CURRENT_DIR ON)

project(hello-world)

find_package(Qt5Widgets REQUIRED)

set(HW_HEADER_DIR ${CMAKE_CURRENT_SOURCE_DIR}/include)
set(HW_GUI_DIR ${CMAKE_CURRENT_SOURCE_DIR}/gui)

include_directories(${HW_HEADER_DIR})

subdirs(src)
