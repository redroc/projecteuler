set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall -Wno-long-long -pedantic")
set( CMAKE_EXPORT_COMPILE_COMMANDS ON )

add_executable(19.out main.c)
add_custom_target(run19
    COMMAND 19.out
    DEPENDS 19.out
    WORKING_DIRECTORY ${CMAKE_PROJECT_DIR}
)
