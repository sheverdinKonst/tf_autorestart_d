cmake_minimum_required(VERSION 3.26)
project(tf_autorestatrt C)

set(CMAKE_C_STANDARD 11)

add_executable(tf_autorestatrt src/main.c
        src/mainParam.h
        src/mainHandler.h
        src/mainHandler.c
        src/portConfig.h
        src/portConfig.c
        src/utils.h
        src/utils.c
        src/ping.c
        src/ping.h
        src/ping.c
        src/ping.c
        src/uds_socket_module.c
        src/uds_socket_module.h
)

INSTALL(TARGETS tf_autorestatrt RUNTIME DESTINATION /usr/bin/)
