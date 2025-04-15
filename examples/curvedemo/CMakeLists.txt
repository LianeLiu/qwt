file(GLOB_RECURSE curvedemo_SRCS *.h *.cpp)

add_qwt_example(curvedemo "${curvedemo_SRCS}")  