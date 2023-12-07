cmake_minimum_required(VERSION 3.28)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

project(Asteroids VERSION 0.0)

add_executable(Asteroids src/main.cpp)


configure_file(include/AsteroidsConfig.h.in include/AsteroidsConfig.h @ONLY)

target_include_directories(Asteroids PUBLIC "${PROJECT_BINARY_DIR}/include")
