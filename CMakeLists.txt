# SPDX-License-Identifier: Apache-2.0

cmake_minimum_required(VERSION 3.20.0)

# Custom VIDI X board definition.
list(APPEND BOARD_ROOT ${CMAKE_CURRENT_SOURCE_DIR})

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(ili9341_xpt2046_lvgl)

target_sources(app PRIVATE
    src/main.c
    src/logo.c
)