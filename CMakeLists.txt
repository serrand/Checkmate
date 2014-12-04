cmake_minimum_required(VERSION 2.8)
project(checkmate)
add_library(checkmate Board.cpp Common.cpp Move.cpp MoveGenerator.cpp
  MoveList.cpp Output.cpp Parser.cpp Tests.cpp)
add_executable(main main.cpp)
target_link_libraries(main checkmate)
