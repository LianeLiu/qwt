file(GLOB_RECURSE cpuplot_SRCS *.h *.cpp)

add_qwt_example(cpuplot "${cpuplot_SRCS}")  