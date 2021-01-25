cmake_minimum_required(VERSION 3.10)

project(SharedPtr)
enable_testing()

include_directories(
    inc/
)

aux_source_directory(test/ TEST)

add_executable(${CMAKE_PROJECT_NAME}_Test ${TEST})

add_test(NAME SharedPtr COMMAND ${CMAKE_PROJECT_NAME}_Test)

