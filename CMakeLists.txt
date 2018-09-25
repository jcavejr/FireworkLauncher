cmake_minimum_required (VERSION 2.6)
project (FireworkLauncher)

set (FireworkLauncher_VERSION_MAJOR 0)
set (FireworkLauncher_VERSION_MINOR 1)

configure_file (
    "src/FireworkLauncherConfig.hpp.in"
    "bin/FireworkLauncherConfig.hpp"
)

include_directories("bin")

add_executable(bin/FireworkLauncher src/FireworkLauncher.cpp)