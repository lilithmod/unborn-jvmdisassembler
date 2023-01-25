cmake_minimum_required(VERSION 3.19)
project(jvmdisassembler C)

set(CMAKE_C_STANDARD 11)

add_library(jvmd STATIC file.c utils.c class.c)
target_include_directories(jvmd PRIVATE include)