# Copyright (c) 2023 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-xxx INTERFACE)

target_sources(mbed-xxx
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-xxx
    INTERFACE
        .
)

target_link_libraries(mbed-xxx INTERFACE mbed-stm32g491xe)
