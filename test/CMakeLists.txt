################################################################
# CppUTest install
include(FetchContent)
FetchContent_Declare(
    CppUTest
    GIT_REPOSITORY https://github.com/cpputest/cpputest.git
    GIT_TAG        latest-passing-build # or use release tag, eg. v3.8
)
# Set this to ON if you want to have the CppUTests in your project as well.
set(TESTS ON CACHE BOOL "Switch off CppUTest Test build")
FetchContent_MakeAvailable(CppUTest)

################################################################

add_subdirectory(add_test)
add_subdirectory(average_test)