cmake_minimum_required(VERSION 4.2.0)

project(DX12-Renderer
    VERSION 0.1.0
    DESCRIPTION "A DirectX 12 renderer project"
    LANGUAGES CXX
)

# Default C++ standard, can be ovewrridden from presets if needed
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# Add per-item subdirectories
add_subdirectory(src)

# Just to prove it works, print something at configure time
message(STATUS "Configuring ${PROJECT_NAME} with C++ standard ${CMAKE_CXX_STANDARD}")