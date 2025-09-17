cmake_minimum_required(VERSION 3.16)
project(RetroRoostQT)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt6 REQUIRED COMPONENTS
        Core
        Gui
        Qml
        Quick
        QuickControls2
)

add_executable(RetroRoostQT
        main.cpp
        Resources/qml.qrc
)

target_link_libraries(RetroRoostQT
        Qt6::Core
        Qt6::Gui
        Qt6::Qml
        Qt6::Quick
        Qt6::QuickControls2
)
