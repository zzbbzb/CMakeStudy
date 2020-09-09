cmake_minimum_required(VERSION 3.10)

#设置项目名称
project(Basic_Starting_Point VERSION 1.0)

# set(Tutorial_VERSION_MAJOR 1)
# set(Tutorial_VERSION_MINOR 0)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

configure_file(TutorialConfig.h.in TurorialConfig.h)

add_executable(Basic_Starting_Point tutorial.cxx)

target_include_directories(Basic_Starting_Point PUBLIC "${PROJECT_BINARY_DIR}")