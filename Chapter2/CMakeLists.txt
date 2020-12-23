cmake_minimum_required(VERSION 3.0)

set(PROJECT_NAME Chapter2)

project(${PROJECT_NAME})

if (WIN32)
    if (DEFINED ENV{DEV_LIB_DIR})
        message("Found DEV_LIB_DIR=$ENV{DEV_LIB_DIR}")
    else()
        message(FATAL_ERROR "No Found DEV_LIB_DIR, Please specify DEV_LIB_DIR by environment variable DEV_LIB_DIR")
    endif()
    message("WINDOWS")
    include_directories(

    )
    
    link_directories(

    )
    
    link_libraries(

    )
else()
    message("UNIX")
endif()


aux_source_directory("src" SRC_DIR)
add_executable(${PROJECT_NAME} ${SRC_DIR})