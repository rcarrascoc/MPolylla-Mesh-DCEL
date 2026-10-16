add_library(meshfiles INTERFACE)
target_include_directories(meshfiles INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(meshfiles INTERFACE OpenMP::OpenMP_CXX)
