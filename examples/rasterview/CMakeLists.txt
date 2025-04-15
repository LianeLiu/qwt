file(GLOB_RECURSE rasterview_SRCS *.h *.cpp)

add_qwt_example(rasterview "${rasterview_SRCS}")  