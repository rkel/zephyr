message("In sysbuild/CMakeLists.txt")
message("APP_CONFIG: ${APP_CONFIG}")

set(hello_world_APP_CONFIG ${APP_CONFIG} CACHE STRING "Application configuration selection")


find_package(Sysbuild REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(sysbuild LANGUAGES)