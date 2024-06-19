cmake_minimum_required(VERSION 3.15)
project(Template VERSION 1.0 DESCRIPTION "description")
add_executable(${PROJECT_NAME}
    src/main.cpp
)

include(cmake/CPM.cmake)

#CPMAddPackage("gh:fmtlib/fmt#7.1.3")

target_link_libraries(${PROJECT_NAME} 
#    fmt
)
target_compile_features(${PROJECT_NAME} PRIVATE 
    cxx_std_17
)