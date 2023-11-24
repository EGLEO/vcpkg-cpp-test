cmake_minimum_required(VERSION 3.21)

project(
    vcpkg_cpp_test
    VERSION 1.0
    LANGUAGES CXX
)

find_package(fmt CONFIG REQUIRED)

add_executable(vcpkg_cpp_test src/main.cc)

target_link_libraries(vcpkg_cpp_test PRIVATE fmt::fmt)