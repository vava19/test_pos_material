# Mindestversion von CMake
cmake_minimum_required(VERSION 3.00)

# Projektname
project(cmakeube)

# Füge die Quelldateien hinzu
add_executable(cmakeube main.cpp add.cpp getInteger.cpp)

# Verzeichnis für Header-Dateien hinzufügen
target_include_directories(cmakeube PRIVATE ${CMAKE_CURRENT_SOURCE_DIR})

# set(CMAKE_BUILD_TYPE Debug)  # oder Release


# C++-Standard festlegen
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
