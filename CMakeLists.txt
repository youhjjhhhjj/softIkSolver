cmake_minimum_required(VERSION 2.8)

set(PROJECT_NAME softIkSolver)
project(${PROJECT_NAME})

include($ENV{DEVKIT_LOCATION}/cmake/pluginEntry.cmake)

set(SOURCE_FILES
    addTcSoftIkSolverCallbacks.cpp
    pluginMain.cpp
    tcSoftIkSolverNew.cpp
)

set(LIBRARIES
    OpenMaya
    Foundation
    OpenMayaAnim
)

build_plugin()