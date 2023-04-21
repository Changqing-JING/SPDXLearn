cmake_minimum_required(VERSION 3.15)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

project(SPDXLearn)

aux_source_directory(src sourceFiles)

add_executable(${PROJECT_NAME} ${sourceFiles})