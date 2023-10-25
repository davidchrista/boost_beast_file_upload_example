file(GLOB FileUpload_Sources
    ${CMAKE_CURRENT_LIST_DIR}/*.h
    ${CMAKE_CURRENT_LIST_DIR}/*.cpp
)

add_executable(FileUpload ${FileUpload_Sources})
target_link_libraries(FileUpload PRIVATE iBoost)
target_link_libraries(FileUpload PRIVATE Threads::Threads)