cmake_minimum_required(VERSION 3.15)
project(MixerLibTest)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_EXPORT_COMPILE_COMMANDS TRUE)

add_executable(mixer_test main.cpp)

include(..)

target_link_libraries(mixer_test mixer)
