cmake_minimum_required (VERSION 3.8.2)
project(CPPTinkerings)

IF(CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)
        SET(CMAKE_INSTALL_PREFIX "../../" CACHE PATH "Build in Lib" FORCE)
ENDIF(CMAKE_INSTALL_PREFIX_INITIALIZED_TO_DEFAULT)

SET(CMAKE_PREFIX_PATH ..)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++17 -Wall -Wextra -Wpedantic -O2")
enable_testing()
add_subdirectory (src)
