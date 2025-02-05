set(LIB_SOURCE_FILES
    ${CMAKE_CURRENT_SOURCE_DIR}/MyUtils/MyUtil.cpp
    ${CMAKE_CURRENT_SOURCE_DIR}/MathLib/add.cpp
)

set(LIB_INCLUDE_DIRS
    ${CMAKE_CURRENT_SOURCE_DIR}/MyUtils
    ${CMAKE_CURRENT_SOURCE_DIR}/MathLib
)

add_library(MyLib STATIC ${LIB_SOURCE_FILES})

target_include_directories(MyLib PUBLIC ${LIB_INCLUDE_DIRS})