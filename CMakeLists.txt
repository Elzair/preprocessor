cmake_minimum_required(VERSION 3.3)

project(boost_preprocessor)

add_library(boost_preprocessor INTERFACE)

target_include_directories(boost_preprocessor BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_preprocessor DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
