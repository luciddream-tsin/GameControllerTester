cmake_minimum_required(VERSION 3.26)
project(GameControllerTester)

set(CMAKE_CXX_STANDARD 20)
add_executable(GameControllerTester main.c init.c input.c )


find_package(SDL2 REQUIRED)


target_link_libraries(GameControllerTester  ${SDL2_LIBRARIES} )
