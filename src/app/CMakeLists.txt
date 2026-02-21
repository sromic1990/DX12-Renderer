# src/app/CMakeLists.txt
add_executable(renderer_app
    main.cpp
)

target_link_libraries(renderer_app PRIVATE renderer_lib)
