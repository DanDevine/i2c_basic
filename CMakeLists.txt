# The following lines of boilerplate have to be in your project's CMakeLists
# in this exact order for cmake to work correctly
cmake_minimum_required(VERSION 3.22)

include($ENV{IDF_PATH}/tools/cmake/project.cmake)

set(
  COMPONENTS
  "main esptool_py i2c icm20948 filters timer"
  CACHE STRING
  "List of components to include"
  )
  
add_compile_options(-fdiagnostics-color=always)

project(i2c_basic)
set(CMAKE_CXX_STANDARD 20)

