cmake_minimum_required (VERSION 2.6)
project (bashlibs-templates)

list(APPEND CMAKE_MODULE_PATH
    "/usr/share/cmake-macros/Modules")
list(APPEND CMAKE_MODULE_PATH
    "/usr/share/bashlibs/cmake-macros/Modules")

include(BashLibs)
set(CPACK_DEBIAN_PACKAGE_DEPENDS
    "bashlibs-utils (>= 0.0.6),
    bashlibs-colors (>= 0.0.15),
    bashlibs-directories,
    bashlibs-shunit2-enhancements (>= 0.0.2)")
include(PackageCreator)

