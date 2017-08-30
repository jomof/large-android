cmake_minimum_required(VERSION 3.6)
add_subdirectory(common)

add_library(main-app SHARED main.cpp)
mathfu_configure_flags(main-app)

target_link_libraries(main-app 
    png
    SDL2
    re2
    png
    lua
)

