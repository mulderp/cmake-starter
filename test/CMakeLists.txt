message(STATUS "tests")


include_directories(${GTEST_INCLUDE_DIRS})
add_executable(testrunner main.cc)

target_link_libraries(testrunner gtest gtest_main)
