
INCLUDE(BuildPlugin)
INCLUDE_DIRECTORIES("${CMAKE_CURRENT_SOURCE_DIR}" 
                    "${CMAKE_CURRENT_BINARY_DIR}"
                    "${CMAKE_BINARY_DIR}")
include_directories( "${CMAKE_CURRENT_SOURCE_DIR}/csound/include/csound")

BUILD_PLUGIN(lazerhawk LazerHawk.cpp LazerHawk.h MOCFILES LazerHawk.h EMBEDDED_RESOURCES *.png)
