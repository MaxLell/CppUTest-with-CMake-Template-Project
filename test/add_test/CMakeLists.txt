set(TEST_NAME add_test)

set(TEST_SOURCES
    ${TEST_NAME}.cpp
    test_runner.cpp
)

add_executable(${TEST_NAME} ${TEST_SOURCES})

target_link_libraries(${TEST_NAME} PRIVATE CppUTest CppUTestExt ${APP_LIB_NAME})