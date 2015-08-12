# file(GLOB_RECURSE LIBSNDFILE_SRC_SOURCES RELATIVE "${CMAKE_CURRENT_SOURCE_DIR}" "*.c")
add_library(sndfile STATIC common.c file_io.c command.c pcm.c ulaw.c alaw.c float32.c 
                double64.c ima_adpcm.c ms_adpcm.c gsm610.c dwvw.c vox_adpcm.c 
                interleave.c strings.c dither.c broadcast.c audio_detect.c 
                ima_oki_adpcm.c ima_oki_adpcm.h chunk.c ogg.c chanmap.c 
                windows.c id3.c)
target_include_directories(sndfile PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}"
    "${CMAKE_CURRENT_BINARY_DIR}")

