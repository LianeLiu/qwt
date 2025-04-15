file(GLOB_RECURSE simpleplot_SRCS *.h *.cpp)

add_qwt_example(simpleplot "${simpleplot_SRCS}")