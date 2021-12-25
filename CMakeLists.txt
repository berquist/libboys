cmake_minimum_required(VERSION 3.2)
project(libboys Fortran)

set(SRC
    libboys.f90
    libboys_data.f90
    )

add_library(boys ${SRC})
set_target_properties(boys PROPERTIES
    COMPILE_FLAGS "-ffixed-line-length-none -ffree-line-length-none")
