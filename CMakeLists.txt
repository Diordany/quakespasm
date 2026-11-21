cmake_minimum_required(VERSION 4.5)

project(QuakeSpasm)

add_executable(quake)

add_subdirectory(src)
target_include_directories(quake PRIVATE /usr/include/SDL2 include)

target_compile_definitions(quake PRIVATE DEBUG USE_SDL2 USE_CODEC_WAVE USE_CODEC_VORBIS USE_CODEC_MP3 _GNU_SOURCE=1 _REENTRANT)
target_compile_options(quake PRIVATE -Wall -Wno-trigraphs -g)
target_link_libraries(quake PRIVATE GL m vorbisfile vorbis ogg mad SDL2)