file(GLOB_RECURSE custom_smart_ptrs_tests_SRC
    "*.cpp"
)

add_executable(custom_smart_ptrs_tests
    ${custom_smart_ptrs_tests_SRC}
)

target_link_libraries(custom_smart_ptrs_tests PRIVATE custom_smart_ptrs_lib)

add_test(NAME custom_smart_ptrs_tests COMMAND custom_smart_ptrs_tests)