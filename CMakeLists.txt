cmake_minimum_required(VERSION 3.16.2 FATAL_ERROR)

set(APP_NAME MultiFiles)

project(${APP_NAME} LANGUAGES CXX)

set(APP_SOURCE_FILES
    ${CMAKE_CURRENT_SOURCE_DIR}/app/app.cpp
)

add_executable(${APP_NAME} ${APP_SOURCE_FILES})
add_subdirectory(lib)
target_link_libraries(${APP_NAME} PRIVATE MyLib)
