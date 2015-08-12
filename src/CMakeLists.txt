file(GLOB_RECURSE LIBSNDFILE_SRC_SOURCES RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}" "*.cpp *.c")
add_library(sndfile STATIC ${LIBSNDFILE_SRC_SOURCES))
target_include_directories(sndfile INTERFACE "${CMAKE_CURRENT_SOURCE_DIR}/include")

