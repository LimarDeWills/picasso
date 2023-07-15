cmake_minimum_required(VERSION 3.13)

set(project_name glad)
project(${project_name})

set(glad_src
    src/glad.c
)
include_directories(
    include    
)
add_library(${project_name} STATIC ${glad_src})
