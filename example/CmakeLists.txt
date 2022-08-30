add_executable(example example.cpp)

target_compile_options(example PRIVATE "-Wall" "-Werror")

target_link_libraries(example 
    PUBLIC sqlparser
)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin/)