file(GLOB SFUS_Sources
    ${CMAKE_CURRENT_LIST_DIR}/*.h
    ${CMAKE_CURRENT_LIST_DIR}/*.cpp
)

add_executable(SFUS ${SFUS_Sources})
target_link_libraries(SFUS PRIVATE iBoost)
target_link_libraries(SFUS PRIVATE Threads::Threads)

install(TARGETS SFUS DESTINATION ${install_binary_dir})