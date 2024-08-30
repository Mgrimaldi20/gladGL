cmake_minimum_required(VERSION 3.16)
project(gladGL)

# Add the GLAD library
add_library(gladGL STATIC
	"include/glad/gl.h"
	"include/KHR/khrplatform.h"
	"src/gl.c"
)

# Specify the include directories for GLAD
target_include_directories(gladGL PUBLIC
	${CMAKE_CURRENT_SOURCE_DIR}/include
)
