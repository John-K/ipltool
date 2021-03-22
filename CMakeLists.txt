cmake_minimum_required(VERSION 3.17)

project(ipltool VERSION 1.0 LANGUAGES C)

set (CMAKE_C_STANDARD 99)

add_compile_options(-O2)

add_executable(ipltool)

target_sources(ipltool PRIVATE amctrl.c aes.c bn.c crypto.c ec.c ec_ipltool.c kirk_engine.c ipltool.c sha1.c utils.c)
