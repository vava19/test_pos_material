---------------------
install CMake:
----------------
sudo apt-get update
sudo apt-get install cmake
cmake --version

2. ctrl + shift +x --> search CMake Tool extension
3. CMakeLists.txt  :  file erstellen

 Diese Datei enthält Anweisungen für den CMake-Build-Prozess. Hier ist ein einfaches Beispiel:
 **** CMakeLists.txt inhalt:
 project(MyProject)

add_executable(MyExecutable main.cpp)

set(CMAKE_CXX_STANDARD 11)
