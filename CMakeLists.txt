cmake_minimum_required(VERSION 2.8.11)

PROJECT(stlalgos)

if (UNIX)
    add_definitions("-Wall")
    add_definitions("-Werror")
endif()

if (WIN32)
    add_definitions(-D_CRT_SECURE_NO_WARNINGS)
endif()

set(FILES 
    main.cc)

add_executable(stlalgos ${FILES})

