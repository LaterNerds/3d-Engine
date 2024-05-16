cmake_minimum_required(VERSION 3.5)

project(engine LANGUAGES C)

add_executable(engine main.c)

include(GNUInstallDirs)
install(TARGETS engine
    LIBRARY DESTINATION ${CMAKE_INSTALL_LIBDIR}
    RUNTIME DESTINATION ${CMAKE_INSTALL_BINDIR}
)
