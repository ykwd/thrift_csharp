cmake_minimum_required(VERSION 2.8)

#include(dsn.ext.csharp.cmake)
project Thrift

set(PROJ_NAME Thrift)

configure_file("${CMAKE_CURRENT_SOURCE_DIR}/${PROJ_NAME}.csproj.template" "${CMAKE_CURRENT_SOURCE_DIR}/${PROJ_NAME}.csproj")

csharp_add_library(
    SimpleITKCSharpManaged
    "${CMAKE_CURRENT_SOURCE_DIR}/*.cs"
  )