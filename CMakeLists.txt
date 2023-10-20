project(nv_libdeflate)

file(GLOB_RECURSE NV_LIBDEFLATE_FILES
	"include/*.h"
	"src/*.cpp"
)

source_group(TREE ${CMAKE_CURRENT_SOURCE_DIR} FILES ${NV_LIBDEFLATE_FILES})

add_library(nv_libdeflate ${NV_LIBDEFLATE_FILES})

target_include_directories(nv_libdeflate PRIVATE "lib/")