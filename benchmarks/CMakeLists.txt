add_executable(runBenchmark benchmark_example.cpp)

find_package(benchmark REQUIRED)
target_link_libraries(runBenchmark benchmark::benchmark)

set_target_properties(runBenchmark PROPERTIES
        RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/benchmarks)
