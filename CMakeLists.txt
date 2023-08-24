cmake_minimum_required(VERSION 3.25)
project(Flat_Shading)

set(CMAKE_CXX_STANDARD 20)
set(SDL2_INCLUDE_DIR C:/Users/DIEAL/OneDrive/Documents/SDL2-2.28.1/include)
set(SDL2_LIB_DIR C:/Users/DIEAL/OneDrive/Documents/SDL2-2.28.1/lib/x64)

include_directories(${SDL2_INCLUDE_DIR})
link_directories(${SDL2_LIB_DIR})

add_executable(Flat_Shading main.cpp color.h Fragment.h print.h shaders.h uniform.h triangle.h)

target_link_libraries(${PROJECT_NAME} SDL2main SDL2)
