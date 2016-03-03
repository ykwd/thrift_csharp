cmake_minimum_required(VERSION 2.8)

# Project
project(thrift_csharp c cxx)

if(WIN32)
    add_subdirectory(src)
endif()