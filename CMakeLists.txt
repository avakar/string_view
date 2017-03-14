cmake_minimum_required(VERSION 3.0)
project(string_view)

add_library(string_view INTERFACE)
target_include_directories(string_view INTERFACE include)
target_compile_features(string_view INTERFACE cxx_right_angle_brackets)
