file(GLOB_RECURSE tvplot_SRCS *.h *.cpp)

add_qwt_example(tvplot "${tvplot_SRCS}")  