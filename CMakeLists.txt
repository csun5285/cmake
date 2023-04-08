# cmake 最低版本要求
cmake_minimum_required(VERSION 3.10 FATAL_ERROR)

# project 信息
project(cmake
    VERSION         0.0.1
    DESCRIPTION     "Cmake Demo"
    HOMEPAGE_URL    "https://github.com/csun5285/cmake"
    LANGUAGES       C CXX
)

list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")
include(BuildInfo)

add_subdirectory(external)

add_subdirectory(src)


add_subdirectory(docs)

add_subdirectory(test)

add_subdirectory(packaging)