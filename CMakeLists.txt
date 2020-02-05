cmake_minimum_required(VERSION 3.8)

# set the project name and version
project(Hermes)

# configure_file(HermesConfig.h.in HermesConfig.h)
file(GLOB_RECURSE fileCollection "src/*.cpp")

add_executable(Hermes ${fileCollection})




target_include_directories(Hermes PUBLIC "${PROJECT_BINARY_DIR}")