file(GLOB_RECURSE barchart_SRCS *.h *.cpp)

add_qwt_example(barchart "${barchart_SRCS}")  