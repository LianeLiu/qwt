file(GLOB_RECURSE friedberg_SRCS *.h *.cpp)

add_qwt_example(friedberg "${friedberg_SRCS}")  