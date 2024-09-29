add_executable(runTests test_example.cpp)

find_package(GTest REQUIRED)
target_link_libraries(runTests GTest::GTest GTest::Main)

add_test(NAME ExampleTest COMMAND runTests)
