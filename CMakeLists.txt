cmake_minimum_required(VERSION 3.19)
project(SFMLTest)

set(CMAKE_CXX_STANDARD 14)

add_executable(SFMLTest main.cpp)


set(SFML_STATIC-LIBRARIES TRUE)
set(SFML_DIR C:/SFML/lib/cmake/SFML)

find_package(SFML COMPONENTS system window graphics audio network REQUIRED)

include_directories(C:/SFML/include)

target_link_libraries(SFMLTest sfml-system sfml-window sfml-graphics sfml-audio sfml-network)
