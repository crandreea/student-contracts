cmake_minimum_required(VERSION 3.27)
project(Lab10)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

set(CMAKE_PREFIX_PATH "/Users/croitoruandreea/Qt/6.7.0/macos/lib/cmake")

find_package(Qt6 COMPONENTS
        Core
        Gui
        Widgets
        REQUIRED)

add_executable(Lab10 main.cpp
        contract.cpp
        header/erori.h
        repo.cpp
        service.cpp
        validator.cpp
        GUI.cpp
        header/GUI.h
        teste.cpp
        header/observer.h
        header/contractCRUDgui.h
        header/contractREADgui.h
        header/myTable.h)
target_link_libraries(Lab10
        Qt::Core
        Qt::Gui
        Qt::Widgets
)

