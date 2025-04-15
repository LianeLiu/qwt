file(GLOB_RECURSE radio_SRCS *.h *.cpp)

add_qwt_example(radio "${radio_SRCS}")  