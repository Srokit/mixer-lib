cmake_minimum_required(VERSION 3.15)
project(MixerLib)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_EXPORT_COMPILE_COMMANDS TRUE)

set(SOURCE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)
set(PUBLIC_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/public_include)

add_library(mixer STATIC ${SOURCE_DIR}/Mixer.cpp)

target_include_directories(mixer PRIVATE ${SOURCE_DIR})
target_include_directories(mixer PUBLIC ${PUBLIC_INCLUDE_DIR})

add_subdirectory(test)