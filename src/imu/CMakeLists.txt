cmake_minimum_required(VERSION 2.8.0)
project(imu)

aux_source_directory(. cpp_files)
add_library(${PROJECT_NAME} SHARED ${cpp_files})
target_link_libraries(${PROJECT_NAME} data tools)