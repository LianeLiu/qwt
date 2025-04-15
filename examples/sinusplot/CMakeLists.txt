file(GLOB_RECURSE sinusplot_SRCS *.h *.cpp)

add_qwt_example(sinusplot "${sinusplot_SRCS}")  