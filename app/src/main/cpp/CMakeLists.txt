cmake_minimum_required(VERSION 3.22.1)

project(conv)

add_library(conv.eng SHARED ff_interface.c)
find_library(log-lib log)

target_link_libraries(conv.eng ${log-lib})