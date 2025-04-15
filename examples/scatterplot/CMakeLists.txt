file(GLOB_RECURSE scatterplot_SRCS *.h *.cpp)

add_qwt_example(scatterplot "${scatterplot_SRCS}")  