# CMakeLists.txt file for tinyxml library

project( tinyxml )

# collect a list of all source files
file( GLOB LIB_SRCS ${PROJECT_SOURCE_DIR}/../../src/*.cpp )

# collect a list of all header files (to be used in MOC compiler)
file( GLOB LIB_HDRS ${PROJECT_SOURCE_DIR}/../../src/*.h )

include_directories(
	${PROJECT_SOURCE_DIR}/../../src
)

# add build target for library
add_library( ${PROJECT_NAME} STATIC
	${LIB_SRCS}
)




