cmake_minimum_required(VERSION 3.16)
project(fuzzing_example)


find_package(cifuzz NO_SYSTEM_ENVIRONMENT_PATH)
enable_fuzz_testing()


add_fuzz_test(my_fuzz_test my_fuzz_test.cpp)
