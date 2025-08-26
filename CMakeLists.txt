cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_OSX_ARCHITECTURES "arm64;x86_64")
set(CMAKE_CXX_VISIBILITY_PRESET hidden)

# Set Project name and version
project(CustomGame VERSION 0.0.1)

# Set Executable name (ProjectName(CustomGame)-vVERSION(0.0.1))
add_executable(${PROJECT_NAME}-v${PROJECT_VERSION}
    # C++ Code (.hpp and .h files are linked from these files
    # meaning that they get added even though they aren't 
    # specified here)
    src/executable/main.cpp
    src/libraries/library.cpp
)
