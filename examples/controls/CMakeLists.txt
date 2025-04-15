file(GLOB_RECURSE controls_SRCS *.h *.cpp)

add_qwt_example(controls "${controls_SRCS}")  