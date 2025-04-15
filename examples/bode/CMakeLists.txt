file(GLOB_RECURSE bode_SRCS *.h *.cpp)

add_qwt_example(bode "${bode_SRCS}")  