cmake_minimum_required(VERSION 3.5)

project(ZED_Explore)

set(CMAKE_INCLUDE_CURRENT_DIR ON)
set(CMAKE_PREFIX_PATH "C:/Qt/Qt5.9.9/5.9.9/msvc2015_64")

set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt5 COMPONENTS Core Gui Widgets Qml Designer REQUIRED)

add_executable(ZED_Explore
    main.cpp
    mainwindow.cpp
    mainwindow.h
    mainwindow.ui
  )

target_link_libraries(ZED_Explore Qt5::Widgets Qt5::Core Qt5::Gui Qt5::Qml)
