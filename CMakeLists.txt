cmake_minimum_required(VERSION 3.10)

project(PES1UG20CS721_hello_world)

find_package(GTest REQUIRED)  # Included for testing

add_executable(hello_world main.cpp)

target_link_libraries(hello_world GTest::gtest)  # Included for testing

add_test(NAME hello_world_test COMMAND hello_world)  # Included for testing
