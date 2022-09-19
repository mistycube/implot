cmake_minimum_required( VERSION 3.7 )

project(implot)
file(GLOB implot_SRCS "*.cpp" "*.h")
add_library(implot STATIC "${implot_SRCS}" )
target_include_directories(implot PUBLIC
  "../implot"
	"../imgui"
)