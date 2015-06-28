

cmake_minimum_required(VERSION 2.8)

include_directories(. ../../../OGLCompilersDLL)

add_library(OSDependent STATIC ossource.cpp osinclude.h)

set_target_properties(OSDependent PROPERTIES FOLDER "glslang")

install(TARGETS OSDependent 
        ARCHIVE DESTINATION lib)
