cmake_minimum_required(VERSION 2.8)

set(TARGET milner)

set(HEADERS )

set(SOURCES ${TARGET}.cxx)

add_executable(${TARGET} ${HEADERS} ${SOURCES})
target_include_directories(${TARGET} PRIVATE ${BUDDY_ROOT_DIR}/src)
target_link_libraries(${TARGET} ${BUDDY_TARGET})
set_target_properties(${TARGET} PROPERTIES FOLDER "Examples")
