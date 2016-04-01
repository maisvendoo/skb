# cmake minimal version
cmake_minimum_required (VERSION 3.4)

# project name
set (PROJECT skb)

# binary directory
set (BINARY_DIR ../../)
set (EXECUTABLE_OUTPUT_PATH ${BINARY_DIR}/bin)

# source directory
aux_source_directory("./" SRC)

# libs
set (LIBS X11)

# Build
add_executable(${PROJECT} ${SRC})

# link libs
target_link_libraries(${PROJECT} ${LIBS})
