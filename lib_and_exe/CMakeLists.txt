cmake_minimum_required(VERSION 3.1)
project(test2 LANGUAGES CXX)

add_library(msg
  STATIC
    src/msg.h
    src/msg.cpp
  )
        
add_executable(test2 src/main.cpp)

target_link_libraries(test2 msg)
