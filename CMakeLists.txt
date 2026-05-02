cmake_minimum_required(VERSION 3.15)

project(http_beastie)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Boost REQUIRED COMPONENTS system)
include_directories(include)

add_executable(http_beastie
    src/main.cpp
    src/utils.cpp
)

target_link_libraries(http_beastie Boost::system)
