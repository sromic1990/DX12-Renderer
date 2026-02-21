# src/CMakeLists.txt

add_library(renderer_lib STATIC
    renderer_lib.cpp)

# Good defaults for your whole codebase
target_compile_features(renderer_lib PUBLIC cxx_std_20)

# Public include root: lets you do #include "core/Log.h"
target_include_directories(renderer_lib
    PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
)

# Pull in modules (each module adds sources to renderer_lib)
# add_subdirectory(core)
# add_subdirectory(renderer)
# add_subdirectory(dx12)

# App (entry point)
add_subdirectory(app)