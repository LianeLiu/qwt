file(GLOB_RECURSE legends_SRCS *.h *.cpp)

add_qwt_example(legends "${legends_SRCS}")  