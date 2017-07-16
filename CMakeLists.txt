make_minimum_required(VERSION 3.0)
project(cpython)

file(GLOB SOURCE_FILES
        Python/*.c
        Parser/*.c
        Objects/*.c
        Modules/*.c)

include_directories(Include)

add_executable(cpython ${SOURCE_FILES})