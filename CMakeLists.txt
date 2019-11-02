cmake_minimum_required(VERSION 3.15)
project(MDTabulated C)

set(CMAKE_C_STANDARD 11)

add_executable(MDTabulated main.c timing.c timing.h running.c running.h globaldata.c globaldata.h initializer.c initializer.h)


file(GLOB SOURCES
        *.h
        *.cpp
        *.c
        )
target_link_libraries(MDTabulated m)
