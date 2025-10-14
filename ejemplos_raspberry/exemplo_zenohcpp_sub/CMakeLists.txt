cmake_minimum_required(VERSION 3.16)
project(zenohcxx_examples LANGUAGES C CXX)


add_executable(zc_simple zc_simple.cxx)
target_compile_definitions(zc_simple PUBLIC ZENOHCXX_ZENOHC)
target_link_libraries(zc_simple PRIVATE zenohc)
set_property(TARGET zc_simple PROPERTY LANGUAE CXX)
set_property(TARGET zc_simple PROPERTY CXX_STANDARD 17)
