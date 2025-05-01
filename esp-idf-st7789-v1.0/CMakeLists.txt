# The following lines of boilerplate have to be in your project's
# CMakeLists in this exact order for cmake to work correctly
cmake_minimum_required(VERSION 3.16)

include($ENV{IDF_PATH}/tools/cmake/project.cmake)
project(esp-idf-st7789-v1.0)

littlefs_create_partition_image(part_fonts device_fonts FLASH_IN_PROJECT)
littlefs_create_partition_image(part_images device_images FLASH_IN_PROJECT)
littlefs_create_partition_image(part_icons device_icons FLASH_IN_PROJECT)
