project(Toplex_map_benchmark)

add_executable(Toplex_map_benchmark benchmark_tm.cpp)

if(TARGET TBB::tbb)
  target_link_libraries(Toplex_map_benchmark TBB::tbb)
endif()
