get_filename_component(TEST_NAME ${CMAKE_CURRENT_SOURCE_DIR} NAME)

set(TEST_SOURCES
    ${TEST_NAME}.cpp
    ${TEST_RUNNER}
)

add_executable(${TEST_NAME} ${TEST_SOURCES})

target_link_libraries(${TEST_NAME} PRIVATE CppUTest CppUTestExt ${APP_LIB_NAME})