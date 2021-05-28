cmake_minimum_required(VERSION 3.5.2)

project(calibrator)

set(BIN_PATH "bin")

# cmake -DCMAKE_BUILD_TYPE=Debug

set_source_files_properties(calibrator.c PROPERTIES COMPILE_FLAGS -lm)
add_executable(calibrator calibrator.c)
set_target_properties(calibrator PROPERTIES RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/${BIN_PATH})