file(GLOB_RECURSE custom_smart_ptrs_lib_SRC
    "*.cpp"    
)

add_library(custom_smart_ptrs_lib
    ${custom_smart_ptrs_lib_SRC}
)

target_include_directories(custom_smart_ptrs_lib PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})