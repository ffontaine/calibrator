cmake_minimum_required(VERSION 3.5.2)

project(calibrator)

set(BIN_PATH "bin")

# cmake -DCMAKE_BUILD_TYPE=Debug

add_executable(calibrator calibrator.c)
target_link_libraries(calibrator -lm)
set_target_properties(calibrator PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/${BIN_PATH})