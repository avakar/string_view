cmake_minimum_required(VERSION 3.0)
project(string_view)

add_library(string_view INTERFACE)

if (${MSVC_VERSION} GREATER 1909)

target_compile_options(string_view INTERFACE "/std:c++17")

else()

target_include_directories(string_view INTERFACE include)
target_compile_features(string_view INTERFACE cxx_right_angle_brackets)

endif ()
