quelle:

https://www.youtube.com/watch?v=gGxi500Q5uE&t=299s&ab_channel=Code%2CTech%2CandTutorials

---------------------
install CMake:
----------------
sudo apt-get update
sudo apt-get install cmake    ---> install in root dir
cmake --version

2. ctrl + shift +x --> search CMake Tool extension
3. CMakeLists.txt  :  file erstellen

 Diese Datei enthält Anweisungen für den CMake-Build-Prozess. Hier ist ein einfaches Beispiel:
 **** CMakeLists.txt inhalt:

 ------------------------begin
 cmake_minimum_required(VERSION 3.18)
 project(MyProject)

add_executable(MyExecutable main.cpp)

set(CMAKE_CXX_STANDARD 11)
---------------------end

oder :  ctrl+shift +p  (palete command): cmake quick start



4. mkdir build && cd build
5. cmake ..    (statt cmake . -- to znaci u istom folderu)
6. cmake -j4            ----> ovo je linker (when added  files)
7. make "projekt.exe name"       ----> ovo je compiler
8. ./projekt.exe name



---- Step 3. noch einamal längere version: CMakeLists.txt ------

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



----------------------
1. oder wir konnen "CMakeLists.txt" automatisch erstellen
Command Palette :  Ctrl + shift +P  --> quick start (generate CmakeLists.txt)
-- add name
-- add compiler name
-- if we have library, we can add

--ovo se uvijek moze korisiti:
6. cmake -j4            
7. make "projekt.exe name" 
8. ./projekt.exe name





