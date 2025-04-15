file(GLOB_RECURSE realtime_SRCS *.h *.cpp)

add_qwt_example(realtime "${realtime_SRCS}")  