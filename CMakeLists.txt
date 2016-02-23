cmake_minimum_required(VERSION 3.3)
project(SampleUSBAudioPlugin)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(SOURCE_FILES
    English.lproj/InfoPlist.strings
    AppleUSBAudioPlugin.h
    Info.plist
    ProcessFloatSamples.c
    ProcessFloatSamples.h
    Readme.txt
    SampleUSBAudioPlugin.cpp
    SampleUSBAudioPlugin.h
    version.plist)

add_executable(SampleUSBAudioPlugin ${SOURCE_FILES})