cmake_minimum_required(VERSION 3.15)
cmake_policy(SET CMP0091 NEW)

include(settings)

make_executable(Editor)

find_package(SDL2 REQUIRED)

target_link_libraries(
    Editor PRIVATE
        Core
        SDL2::SDL2
        SDL2::SDL2main
)
